---
title: My Guide to Bash Shell
date: "2019-08-08T12:00:00.000Z"
template: "post"
draft: False
slug: "/blog/My-Guide-to-Bash/"
category: "Programming"
tags:
  - "Programming"
description: "My favorite uses for Bash"
---

My first programming class at Johns Hopkins was __Introduction to Computing__ taught by Dr. Ana Damjanovic in the Fall
semester of 2018. The goal of the class was to teach the basics of three scripting languages: Bash, Python, and Matlab.
This is considered an __easy A__ class at Hopkins and as a student primarily interested in biology, I decided to use
it to fill out my computing requirement. Turns out, the class was pretty fun (and as advertised, very easy).

Computers can do a lot of cool things and now I'm a CS student :). Here is a quick tutorial on the most powerful scripting
capabilities of Bash scripting. <sub><sup>(This is what terminal is on Mac. Don't ask about Windows. Windows is sad)</sub></sup>

First let's talk about what inspired me to write this tutorial. I think a lot of students will start with Python, or Java,
or if you are an engineer, even Matlab. Clearly those are also amazing tools with a lot of functionality, but when I first
started learning them, I didn't really know the _structure_ of how code runs and how scripts need to access different files.
I kind of thought that the code itself was all you needed to worry about when in fact, the correct data structures and access
permissions of different files is equally important. What kicked this line of thinking off was actually me building this
website. This was forked from a Github repository named Gatsby-Starter-Lumen and of course was filled with placeholder
information about "John Doe". I could see these values on the webpage hosted online, but I needed to be able to change values
in the source code. Instead of clicking and reading through each file, I knew there had to be a better way to search for strings.

I know macOS has a finder tool, but it is pretty lacking as a pseudo control + f.
It doesn't support regex and usually gives me some sort of safari search. Bash is a perfect tool to do exactly
what we want here.

Here's how it's done:

```Bash
grep -R "your search" *
```

Incredibly simple.

What if you want to write a script that will all execute at once?

We have a built in editor called vim that we can use to create scripting files. Scripting files
end in .sh and can be run in the terminal.

Type `vi fileName.sh` and you can start writing your script.

Bash is only one type of scripting shell interpreter available to use.
Each interpreter may have different syntaxes and functions but they are generally the same.
To specify that we are using bash, we can either include what is known as a _shebang_ to the top of each script, or when
calling the script, run it with __bash__ specified beforehand.

The shebang to include: `#!/bin/bash`
To run a script with bash: `bash script.sh`

Bash scripting is not my strong suit, although it is still an incredibly useful tool. I still prefer to use Python for
most scripting tasks and Bash as a special tool to navigate the files on my computer. To each their own though.

Here are a couple tools that I have found to be most useful.

Type `ls` to view all the files in a directory (folder).
Type `cd newDirectory` to change your directory. You can specify the entire path name so for example to change my
directory to my Documents folder, I would write `cd /Users/dennisgong/Documents`. Or, by default we are set in the
`/Users/dennisgong` directory so I could change my directory using the local path `cd Documents`.

To print which directory you are in, type `pwd`.

To create a new directory, use `mkdir newDirectory` to create the directory "newDirectory"
To move a file or directory, use `mv sourcePath destinationPath`. For the source and destination paths, you can use either
relative or full path names. This one has a couple useful options that you can provide. `mv sourcePath destinationPath -i`
makes sure the shell asks you whether to overwrite existing files or skip moving them (type Y or y to overwrite). The `-v`
option prints out the names of all files that you move so you can see your computer doing work for you.

Similarly, `cp` copies files instead of moving them. Add the `-r` option to recursively copy each of the subfolders and files.

To remove files, use `rm`, but be careful in specifying the path. If you're not careful, more files than you want will be
deleted. Thankfully, deleted files are still in the trash folder.

Finally, the command that inspired this tutorial: `grep`. It's super simple and I usually use the syntax I used before
`grep -R "search" *` -R for recursive, and * to print out the whole line of all occurrences.

Whatever commands you come across and don't immediately know how to use, you can use the `man` command which will
give you a manual of how to use certain commands.

For example, `man date` will describe the date command.

For more specific (or general) problems, StackExchange is almost always the answer.

In conclusion, understanding where your files are, which directories you are in, and where to store your files is important if you ever want to write scripting files because you need to be able to tell your computer where your files are to access them.
Having good command of the simple Bash commands was very useful in helping me with my code and hopefully it will help you
with yours also!

Hope you enjoyed!

Dennis
