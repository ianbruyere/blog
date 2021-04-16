---
title: "The Weekly Commit #17"
date: 2021-04-15T23:18:45-04:00
draft: false 
---
I learned the power of Perl this week .
I was writing a script to move some text files between servers, and a co-worker showed me how with bash as the frame and a perl one-liner doing the lifting he could accomplish what was taking me ~15 lines of Python. A lesson in the quick and clean writing of scripts; needless to say I was impressed.  
For the curious it was something like this:
```bash
perl -ne 'print if filename\..\----'
``` 
A quick explainer the n flag makes it a while loop, the e flag means it's an expression, the backslashes separte the pattern, so filename is a variable given to the first line, .. is regex anything/everything until it comes up to the '----' which was simply our chosen delineator.  
I don't plan on formally learning perl but it's in the toolbox so it's handle will become worn before long.
### The Doing
Still working through Linux Admminstration learning. Mainly I've only had time to setup the Virtual Environment but that still lands me about 25% through the 1st volume.
