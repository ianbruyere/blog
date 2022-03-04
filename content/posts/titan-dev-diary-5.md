---
title: "Titan Dev Diary #5"
date: 2022-02-25T14:50:00-05:00
draft: false
---
## Day 5
**Commit Hash**: 83f45e68913d98b37de982954d3af609d3af9788  
Iteratively hitting walls, walking down wrong paths, but still finding a way forward.
I understand `tkinter` enough to be my own guiding light. At points of hard contention
I'd beseech external resources only to find I'd independently implemented their 
sage suggestions. This happened ad nauseam multiple times giving rise to new
tantilizing perceptions of my abilities: either simple things bamboozle me or I'm 
at the bleeding edge of a problem space.  
A new binary emerges: should I be ashamed or proud?    
  
Features Added:
* Player overview now updates according to muster
* Army overview also updates in response to mustering event
    
Upcoming:
* Removing units from an army due to game event of battle.
* final boss of Splitting the Armies.  
  
Then the network awaits.

Showcase
```Python
# TODO
# refactor into:
# Base State
# muster state
# upkeep(split) state
# resolve conflict state
# so there can be a forced flow for turn
# and a clear delineation when it's your turn vs someone elses
# but this works for first pass
```
Thinking while coding...how novel.
  
Questionable
```Python
def open_menu(self, event, army, player):
    window = PlayerArmyMenu(self, self.army, player)
```
Should I be passing the army variable everywhere or via self?  
Probably the former, easier to tell origin as I pass from class to class. 
It works either way, but death via spaghetti is impending.  