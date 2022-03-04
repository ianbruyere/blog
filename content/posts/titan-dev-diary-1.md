---
title: "Titan Dev Diary #1" 
date: 2022-02-21T23:48:44-05:00
draft: false
---
[Project Repo|https://github.com/ianbruyere/titan-army-tracker]

## Day 1
**Commit: ad3e49bb532ebca99a332defa2a84e9b230f9e00**  
Now I'm on my own; I'm beyond the scope of the blog post. 
I floundered for a bit on where to start; feverishly typing out ideas as a balm.
My starting point though has been determined: the setup screen.   
What a session this turned out to be.  
I made headway quickly getting dropdowns created, populated, and an image loaded in.
With the basic elements in place, the stage was set for trouble to manifest:
* visually separate drop downs would change to match the other
* image wouldn't change in response to dropdown changing
	* during callback event, label information wasn't present --> major sticking point
* general UI plague  

It was a ~6 hour effort this time. I wasted time by failing
to note that SO answers were 8+ years old referring to Python 2 tkinter implementation.  
This compounded my unfamiliarity with `tkinter` and hamstrung me for a while.  
Refactoring my code helped greatly though, reducing the surface area of errors.   
I was able to have a complete Setup Screen to show off.
To see my progress in action run `python3 client.py` from the commit hash given aove.