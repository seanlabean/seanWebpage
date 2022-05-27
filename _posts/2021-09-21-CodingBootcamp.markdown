---
layout: post
title: Drexel Coding Bootcamp
date: 2021-09-21 00:00:00
description: Introduction to coding with Python
---

## Overview
With this post, I hope you will be able to set yourself up with an up-to-date Python environment as well as gain some experience with `Git` to obtain the DrexelCodingLessons repository in which we will be going through daily lessons/reviews throughout the next week. 

## Operating System
I’m only familiar with MacOSX and using the Unix command line to navigate filesystems. If you are using Windows, you could download Windows Subsystem for Linux (WSL) from the Microsoft store as it will allow you to follow along with the Terminal commands I do (Ubuntu is the recommended one, it’s free and should do the job). This is not required at all, but just something to think about. If you haven’t used the command line at all, I recommend watching some beginners videos on Youtube and following along before we meet next week.

For the Lesson you will need a few things installed.
1.   A python3 environment (I think any 3.x version will do, I am using 3.7). Check your current python environment by typing the following command on the command line: `python –-version`
2.  An installation of Jupyter Notebook.
3.  Install the Python packages: numpy, matplotlib, pandas, scipy

For those that don’t have these, you have a few choices in how you want to proceed. I recommend Anaconda, a package manager that is pretty easy to use and is expandable to include management of other languages like Julia and R if you ever decide to use them: [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual) scroll to the bottom for install options. Otherwise, you can install everything independently, installing a python3 version ([https://www.python.org/downloads/](https://www.python.org/downloads/)) and jupyter notebooks using the pip command: `pip install jupyter notebook` (see here: [https://jupyter.org/install](https://jupyter.org/install)). To install the python packages, you can do this on the command line by issuing the pip command: pip install numpy for example. Please do this for each package I have listed.

## Download the Lessons from Github
I have uploaded all of our lessons to github, please go to your command line (Terminal on Mac) and do:
`git clone` [https://github.com/seanlabean/DrexelCodingLessons](https://github.com/seanlabean/DrexelCodingLessons)

This will pull down all the lessons including code and pdfs and put it into a directory (folder) called ‘DrexelCodingLessons’. If this isn’t working for you for whatever reason, you can go to [https://github.com/seanlabean/DrexelCodingLessons](https://github.com/seanlabean/DrexelCodingLessons) and download everything as a ZIP. If you’re more savvy with git, feel free to fork the repository. We’ll have a git overview towards the end of the week where I’ll introduce basic concepts as it’s a vital skill in today’s age!

## A Quick Navigation Test
1.  Go into the directory, look inside it to see directories called Lesson(1-7), Info, and two textbook pdfs on Python Programming. To do this on the command line, do:
	-  cd DrexelCodingLessons
	- ls
2.  Go into the Info directory:
	-  cd Info
3.  Open the text file called UnixSystem.txt (you can use the text editor of your choice here):
	-  nano UnixSystem.txt

## A Quick Python Test
1.  While still inside the Info directory, call python on the file names [python_test.py](http://python_test.py/)
	- python [python_test.py](http://python_test.py/)
This will execute what’s written in the file (which you can take a look at if you want the same way we did the text file) which is some print statements so you can see it’s working, and imports of the python packages we will need throughout the Lessons. This is basically just a rough way to check if you have installed the python packages correctly.

#compsci #drexel