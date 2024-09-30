---
title: Making your first website
date: "2019-08-12T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/How-I-Made-My-Website/"
category: "Programming"
tags:
  - "Programming"
description: "How I made this personal website"
---

The summer following my Freshman year in college, one of the things I often did (not proudly) was look through peoples LinkedIn profiles, just in order to see what other people had going on in their lives. I wanted to know all the possibilities for internships, jobs, and programs that were possible for me to do as a fellow college student in a similar position. The college internship process seemed unreasonably fast paced to me, and I wanted to get a head start on knowing at least what companies frequently recruit college students and which places I would prioritize applying to.

While this was very insightful and a great way to grow my connection count on LinkedIn (who needs Instagram when there's LinkedIn), an unexpected consequence was coming across people's personal websites! As a high school student in a more humanities inspired school, I had never been exposed to web development aside from Weebly pages, so it was shocking that so many kids my age would be able to set up professional looking websites. I was impressed with them, so I knew that at some point, I would need to set one up as well.

My first attempt was attending a workshop held at Hopkins titled "Creating a Personal Portfolio". This seemed useful and connected to what I wanted to do, so I signed up, thinking at the very least I could create a bare bones web page with my personal information. While I learned a bit about the importance of marketing oneself, the workshop essentially amounted to a very simple introduction to Wordpress. I had also tried looking at [about.me](about.me) a site designed for people like me to easily put oneself on the internet. However, I didn't like the fact that you had to pay for premium features such as additional pages, customizability, and a domain without their branding.

I figured, it was time to learn how to write and host my own website. I learned some basic HTML, CSS, and looked into the most common domain hosting websites like [godaddy.com](godaddy.com). Definitely wasn't experienced or dedicated enough to make that happen, unfortunately.

My savior was Github. I found out about [Github pages](https://pages.github.com/) which surprised me with how easy, free, and simple it was to set up. All things considered, the whole process only took a few hours to get everything published and how I wanted it. You can find my old website [here](https://gong-dennis.github.io/). This was awesome! I accomplished my goal and it didn't look that bad to me either.

It was only by chance that I learned about a Github repo that basically builds a beautiful website for you [gatsby-starter-lumen](https://github.com/alxshelepenok/gatsby-starter-lumen). This was exactly what I was looking for: customizability, multiple pages, blogging capability, and a custom domain. While a bit more complicated than Github pages to set up, this resource made the whole process way simpler and way faster than it ever would have been doing it by myself. Just follow the provided instructions to get started.

###Here are a couple resources to help you create a website of your own!

The first thing to get a grasp of is the structure of files contained within the repository. The most important file is the config.js file, where you will edit your personal information, set up your thumbnail, and other customizing information down the line. Make sure if you change anything, make sure that other files are not affected, otherwise your website will not compile. The way I did this was my using the bash command `grep` to search all the directory files and ensure consistency with regards to variable names and syntax.

For the most part, whatever small things you want changed on your website, you can search through the website files with grep and change the source code. For blog posts, they will be written in a markup language called markup, which I will explain below. It is very similar to typing in a more common text processor like Word or Google Docs, just a bit different.

To start, I would recommend going to the gatsyby-starter Github page and reading up on the details regarding hosting the website with Netlify. Once you have your domain set up, it's just a matter of customizing the relevant information to best suit your needs.

###The skills:

1. Markdown

Markdown is a markup language that allows you to format text in a markdown file (ends in .md) which can be used to be displayed
on webpages.

Here are a couple resources to get going with it. The most comprehensive [guide](https://www.markdownguide.org/getting-started), and a markdown to text [translator](https://dillinger.io/), is basically all you need.

2. Git

To navigate hosting with Netlify and Github like the instructions say, I found it useful to have a basic grasp of Git version control in Github. THe first thing I would do is download [Github for Desktop](https://desktop.github.com/) and watch some tutorial videos on how it works and how to connect it to your Github account. Once you clone and download the starter repo, editing offline on your computer should be very easy.

That's it! As you can see, creating your own personal website does not require any specialized skills, just some time to spend figuring things out and creating some accounts. I'm sure the developers of the lumen starter would love to hear your feedback or questions, and so would I. Feel free to contact me at <gong.dennis@gmail.com>.

I hope this was useful!

Dennis Gong
