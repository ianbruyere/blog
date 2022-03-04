---
title: "Titan Dev Diary #6"
date: 2022-02-26T14:50:03-05:00
draft: false
---

## Day 6
**Commit Hash**: e873ea2a82e09165a8a6297977f0698169e0e854  
I've mostly brushed the rust off my Object-Oriented programming for Python.
Refactored code to have classes coresponding to the current action, as opposed to 
lumping them all into one area. Doesn't matter so much on the UI side but easier  
from a development perspective.  

**The Breakdown**  
Features Added:    
* Resolve battle now updates Overview Correctly
* A "Turn" function is in-process: will guide a player through valid actions per army.  
  
Some UI Errors:  
* Units removed after Resolve Battle will persist on army screen until close-reopen
* Newly mustered units will not recieve tick-box until close-reopen on Resolve Battle Screen
* When Army is reduced to 0, does not come off Overview
  
Upcoming:
* Resolve above errors
* Add score allocation for resolve battle, and surrender tick-box
* Skip button for actions you don't want to take
* Get Started on the Big Daddy: Splitting Army
  
Nice-to-Haves:
* Lineage: only units that you can populate with given units populate ddl for muster
* Incorporate colors of units into text