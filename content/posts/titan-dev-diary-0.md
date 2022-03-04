---
title: "Titan Dev Diary #0" 
date: 2022-02-20T14:50:19-05:00
draft: false
---

## Background
Titan(1980) is a fun board game with significant flaws.  
Some flaws charming, some unwieldly. With digital aid Titan can rise above.  
Making army movement easier, distributing public army information,  
and doing bookeeping will be the main goals. Additional  
benefits are preserving game state since Titan can last  
upwards of 4 hours, takes significant table real estate,  
and relocating is tenous at best.  


## Day -1
I made some false starts since my original vision was for a phone app.  
Phones take up minimal table space, people typically have one handy etc.  
However I've never made a phone app, and the despair of starting from scratch  
on a technical level with a project of this ambition swallowed me whole whenever I ventured  
into Android Studio. I decided to lower the barrier by making a desktop app in Python:  
logic, organization, and technical ability of Python itself  would be familiar,  
leaving the GUI and network as a learning curve. I like to use projects to learn new things and  
refine existing skills, and lately Python's lacked eligible suitors: most things falling 
well within my threshold. A skill atrophying because it makes things **too** easy.  

## Day 0
I started with a Google query along the lines of "Game Session with Python".  
I'd never done GUI or network programming with Python; I was on familiar
ground syntax-wise, but these libraries I'd never touched. I didn't even know 
Python had an in-built GUI library called `tkinter`. Using the blog post linked 
below as a guide, I did an ad hoc learn/remix session:  
* skim post, mainly looking at code
* copy code via manually typing it out changing things as needed
* a lot of start-stop-read-repeat going on.
* stubbing out things in the form of empty functions, file names, and comments.  

End result: Client/Server code in the Blog post written out,
a skeleton of directories and functions that would guide me 
on the morrow. Finally, a start. This was as far as I had gotten 
on the phone version, but in hours as opposed to days.  
[Blog Post](https://levelup.gitconnected.com/program-a-networked-tic-tac-toe-game-in-python-30f8826e591d "Blog Post")