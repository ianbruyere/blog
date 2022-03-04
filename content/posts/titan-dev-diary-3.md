---
title: "Titan Dev Diary #3"
date: 2022-02-23T14:49:52-05:00
draft: false
---
## Day 3
**Commit Hash**: 28d4de8ac878570bca991ccc63e3eead3fdaea23  
Made a lot of progress, however one measures progress when "finished" is of nebulous  
determination. It's ugly as sin but the UI is there for Opponents and Players, and  
also a pop out menu for the Player Armies. We'll see if prettifying is ever a thing.  
Now I need to make the central feature of splitting one army into two.  
A quick search before sign-off reveals that `tkinter` doesn't explicitly support drag-drop.  
Of course this search bubbled an alternate GUI for Python to the surface, called `wxPython`.  
Allegedly support is more robust, and it's easier to make the application "pretty".  
  
As long as functionality is not threatenedI'll stick with `tkinter` for now;  
I like Python's "batteries included" approach, and minimal external libraries appeals to me.  
  
~4  days of effort on UI remain: 2-3 on major features, then 1-2 days on polish.  
  
Tenative Road Map:
Version 1: base game functionality and works with good will of user
Version 2: bad will users accounted for
Version 3: gussy it up, either switching GUI manager or working within existing
Version 4: depending on feasibility work on virtual board.