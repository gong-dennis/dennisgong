---
title: Linear Mixed Effect Modeling for Fantasy Football
date: "2019-09-13T12:00:00.000Z"
template: "post"
draft: false
slug: "/blog/Fantasy_Football/"
category: "Programming"
tags:
  - "Modeling"
description: "Applying Statistical Modeling to Fantasy Football"
---

Over the Summer, I interned at the NIA Computational Biology Core, doing analysis on a large longitudinal study of clinical health data. The goal here was to search for correlations between different traits, measured by their correlation coefficient and the number of observations between them. While this very interesting tome, I had a more pressing problem nearing the end of the Summer. Fantasy football season was coming and I had no idea what I was doing.

Fantasy football and I have had a short but also long history. I started in middle school and really got into it the first two years of high school. However, I was very bad, and all the teams I ever built were either destroyed by injury or filled with under-performers. It culminated towards the end of the 2015-16 where I was the league commissioner of a league with my high school friends and I went 5-8-1 and finished last overall. I went on to write a 1,045 word resignation from fantasy sports.

But here's the thing. I added a double major in math, did a statistical modeling internship at the NIH, and now I'm competing against my same friends who are studying history and political science. I knew there has to be a way to apply the statistics I have learned to win with the wealth of sports data available on the internet to predict outcomes and minimize risk. This is what I learned.

I began by scraping ten years of past data from Pro Football Focus, using what I learned about web scraping with the Requests package in Python. Here, I have imported the necessary libraries, and stored the structural components of the url into variables for easier code readability.

```Python

import pandas as pd
import requests
import numpy as np

header = {
  "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/50.0.2661.75 Safari/537.36",
  "X-Requested-With": "XMLHttpRequest"
}

base = "https://www.pro-football-reference.com/years/"

passing = "/passing.htm"
rushing = "/rushing.htm"
receiving = "/receiving.htm"
team = ""
fantasy = "/fantasy.htm"
segments = [passing, rushing, receiving, team, fantasy]
years = np.linspace(start=2009, stop=2018, num=10).astype(int).astype(str)

```

Then, I simply loop through all the combinations that I am interested in, downloading them straight to my downloads folder. Then using UNIX scripting commands,
I move them to my project directory.

```Python
for year in years:
    for data in segments:
        url = base + year + data
        print(url)
        r = requests.get(url, headers=header)
        dfs = pd.read_html(r.text)
        for i in range(len(dfs)):
            if data != "":
                csv_name = data[1:-4] + "_" + year + ".csv"
                dfs[i].to_csv(csv_name, sep = ",")
            else:
                csv_name = str(i) + "_team_" + year + ".csv"
                dfs[i].to_csv(csv_name, sep = ",")
```

After the data is read in, we are able to process it into my favorite data analysis language: R. While Python is just as good, I used R during my Summer internship and have the best command over it when manipulating data.

After I move the data to the analysis directory, I partition it into the various football positions I want to model.

```
library(tidyverse)
library(ggplot2)
library(broom)
library(lme4)

count_NA <- function(row_vec) {
  sum(is.na(row_vec))
}

files <- list.files(path="Files",
                    pattern="*.csv", full.names=TRUE, recursive=FALSE)

fantasy <- files[grep("fantasy", files)]

```

For each position, I read data into a table, with each position from each year getting their own table with various statistics including yards, attempts, efficiency, touchdowns, and more. I then combine them into a master table with ten years of past data for the top 100 players. Sometimes, we need to ensure that the data types are represented as what they are by converting them. This ensures integers are not represented as characters.

```
read_fantasy <- function(file) {
  table <- read_csv(file, skip = 1)
  header <- scan(file, nlines = 1, what = character(), sep = ",")
  header2 <- scan(file, skip = 1, nlines = 1, what = character(), sep = ",")
  colnames(table) <- paste(header, header2, sep = "_")
  colnames(table)[2:6] <- header2[2:6]
  colnames(table)[1] <- "Season"
  table[,1] <- as.numeric(substr(file, 15, nchar(file)-4))
  table <- table %>% filter(Rk != "Rk")
  table <- table[1:150,]
  table[,3] <- lapply(table[,3], gsub, pattern = "[*+]", replacement = "")
  table
}

fantasy_tibbles <- lapply(fantasy, read_fantasy)
all_fantasy <- do.call(rbind, fantasy_tibbles)

all_fantasy[,6:ncol(all_fantasy)] <- sapply(all_fantasy[,6:ncol(all_fantasy)],as.numeric)
all_fantasy[,2] <- lapply(all_fantasy[,2], as.numeric)

```
Next, I introduce a few new variables that I think are important based upon my limited knowledge of fantasy sports. First I add a linear weighting system. More recent years should be more indicative of player performance, so I make recent data count 10 times as much as data from 10 years ago. I also introduce per game averages by dividing the fantasy points a player scores over the entire season by the number of games they play. Sometimes players get injured midway through the season and miss games, so having a per game statistic is an improvement over cumulative statistics. Finally, I partition that players by position to create custom models for each position type.

```
weights <- data.frame(seq(1:10), unique(all_fantasy$Season))
colnames(weights) <- c("Weight", "Season")
all_fantasy <- all_fantasy %>% full_join(weights, by = "Season")

all_fantasy <- all_fantasy %>% mutate(PPR_PPG = Fantasy_PPR/Games_G)
all_fantasy <- all_fantasy %>% mutate(TargetPG = Receiving_Tgt/Games_G)
all_fantasy <- all_fantasy %>% mutate(RushAttPG = Rushing_Att/Games_G)
all_fantasy <- all_fantasy %>% mutate(PassAttPG = Passing_Att/Games_G)
all_fantasy <- all_fantasy %>% mutate(Age2 = Age^2)

RB <- all_fantasy %>% filter(all_fantasy$FantPos == "RB") %>% group_by(Player) %>% arrange(Rk)
QB <- all_fantasy %>% filter(all_fantasy$FantPos == "QB") %>% group_by(Player) %>% arrange(Rk)
WR <- all_fantasy %>% filter(all_fantasy$FantPos == "WR") %>% group_by(Player) %>% arrange(Rk)
TE <- all_fantasy %>% filter(all_fantasy$FantPos == "TE") %>% group_by(Player) %>% arrange(Rk)

```

And finally, we reach the models. I train a mixed linear effect model for each player, with their fantasy points per game as the target endpoint and various statistics including Age, Age<sup>^</sup>2, and touches from the previous year. In essence, each player gets their own individual y intercept, and the slopes for each of these variables are the same for each player. This means that while Le'veon Bell (a superstar) should have a higher starting point (y intercept) the effect of additional carries and age will affect him just as much as T.J. Yeldon, who no one should be drafting.

```
RB_age_age2_model <- lmer(PPR_PPG ~ Age + Age2 + RushAttPG + TargetPG + (1|Player), weights = Weight, data=RB)
WR_age_age2_model <- lmer(PPR_PPG ~ Age + Age2 + TargetPG + (1|Player), weights = Weight, data=WR)
TE_age_age2_model <- lmer(PPR_PPG ~ Age + Age2 + TargetPG + (1|Player), weights = Weight, data=TE)
QB_age_age2_model <- lmer(PPR_PPG ~ Age + Age2 + PassAttPG + (1|Player), weights = Weight, data=QB)
```

Using their age (incremented by 1) and touches from the previous year, I feed them into the model to predict the 2019-2020 season performance. I take the average player in each position and subtract off their point projection from everyone else in their position to achieve the Value Added of each player on top of the average player in their position. This is to correct for the top 30 players all being quarterbacks, since QBs score on average more than other positions. Finally, we export the results for draft day.

Surprisingly, the model's predictions are not far off from the top 100 of Fantasy Pros. The top names including Ezekiel Elliot, David Johnson, Antonio Brown, and other superstars are all at the top of the list. The scrubs are still scrubs. For example, Adrian Peterson, who is going to the Hall of Fame but was good about 7 years ago, is near the bottom of the list. Not bad for a couple linear models. On draft night, I used this as an outline to draft a team that is currently 1-0. Let's hope for the best.

5/1/20 EDIT: Turns out, I am just bad at this. Aaron Rodgers didn't turn out to have a great statistical season, David Johnson got injured and benched, Keenan Allen started really hot but got stone cold _very_ quickly. I won't even mention Sammy Watkins and Brandin Cooks. TLDR: Don't trust me to manage your fantasy football team.

Thanks for reading!

Dennis Gong

QB: Aaron Rodgers/Tom Brady
RB1: David Johnson
RB2: James White
WR1: Julio Jones
WR2: Keenan Allen
WR3: Sammy Watkins
TE: George Kittle
FLEX1: Brandin Cooks
FLEX2: Chris Carson
