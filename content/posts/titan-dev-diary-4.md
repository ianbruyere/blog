---
title: "Titan Dev Diary #4"
date: 2022-02-24T14:49:47-05:00
draft: false
---
## Day 4
**Commit Hash**: baea475c7ccb548842ecc022ec44c8e05fd7e444  
No significant stumbling blocks, other then stumbling from fatigue.
I got mustering "working"; the unit list doesn't refresh unless you close-reopen.  
Also the main overview doesn't update accordingly.
  
I refactored Characters/Creatures - Titan calls them 'Characters', I like 'Creatures',  
but lets be real in code I need to call them units -to use a csv and a namedtuple. 
The writing of took 5 minutes, and troubleshooting took 40.  
Witness.  
  
Incorrect
```Python
from collections import namedtuple
import csv

Character = namedtuple('Creature', ('type', 'name', 'power', 'skill', 'range_strength', 'can_fly', 'ruleset'))

with open("./game_data/character_data.py", 'r') as f:
    r = csv.reader(f)
    next(r) # skipping header
    Characters = {Character(*i).name: Character(*i) for i in r}
```  
  
Correct Code
```Python
from collections import namedtuple
import csv

Character = namedtuple('Creature', ('type', 'name', 'power', 'skill', 'range_strength', 'can_fly', 'ruleset'))

with open("./game_data/characters.csv", 'r') as f:
    r = csv.reader(f)
    next(r) # skipping header
    Characters = {Character(*i).name: Character(*i) for i in r}
```

Perils of coding at 4am.
