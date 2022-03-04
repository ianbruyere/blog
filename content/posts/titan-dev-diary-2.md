---
title: "Titan Dev Diary #2"
date: 2022-02-22T02:46:47-05:00
draft: false
---
## Day 2
**Commit: ad3e49bb532ebca99a332defa2a84e9b230f9e00**    
This was the day where I bit off more than I could chew.
Or at least I felt that way. When I don't fully understand something, it can feel daunting.  
I wasn't sure how `tkinter` was behaving or would behave between multiple window states.  
1. How would information flow between different client-side components of the GUI?  
2. How would I maintain state of the other players?  
3. How would each player get a GUI element in the same app but update discretely?  

Good questions to frame, and would eventually lead to good answers. 
Typically I'd RTFM but more pressing to me was I had no clear design for the app, 
since all `tkinter` was doing was presenting information, and I didn't know how I was going
to create and organize the information itself.
Most of my day I spent __thinking__ as I took care of other concerns: 
chores, working out, being a bum(it was the weekend).  
I'd code intermittenly as thoughts crystallized, but paralysis would soon strike.  
What helped was thinking of `tkinter` as MVC, from web developement, which I __am__ familiar with.  
With that mental model, and isolating my code from my previous work thus skirting Question 1,
I was able to hack out the basis of functionality for the whole project. 

  

