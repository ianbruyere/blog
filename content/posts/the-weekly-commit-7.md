---
title: "The Weekly Commit #7"
date: 2021-02-04T20:41:15-05:00
draft: false
---
I spotted a wild Big O application!; exciting as I’ve only experienced it in a controlled-environment. I’ll post the outline here so knowledgeable people can say how close(or far off) I was.
#### Naive
`for i in x:
	for j, k in enumerate(y):
		if i == k:
			result.append(i)
#### More Performant at Scale(Big O)
`for i in x:
	index = 0
	for j, k in enumerate(y):
		if i == k:
			index = j
			result.append(i)
			break 
	del y[index] # important
`
The naive is n^2(nested for loop, easy), and the improved implementation I **think** is `n log n`, since y becomes smaller. An exciting moment since I **thought** unprompted while coding about Big O. Right or wrong, I’m excited to learn more.  
Respect the little gains, they prompt bigger ones.
### The Doing
* did some sftping, which I’ve never done; it’s simple in scope, easy to use, and useful: the pinnacle of tool design.
* Wrote a python script that takes inputs: a csv, a json file; updates json information with data from csv; than writes updated json to an output file.
	* cleans up csv - which is a cut/paste job from a spreadsheet. Troublesome formatting had to be accounted for.
		* **Fun Fact**: excel columns delineate via \009 pasted into plain text
	* data validation to ensure all expected json fields present.
	* future work is:
		* make it general(within reason), parts of it(most of it) are coded specifc to one files needs.
		* more functional: it can automate even more steps of the process for the application I’m writing it for
* wrote a test case for my personal project! I’m picking up steam :).
### The Learning
After only a brief absence **The Learning** is back for a limited tenure. Reasons why:
* Wes Bos updated his Advanced React course. I was about to brush up on React, Wes said a major update was incoming so I waited; 3 months later here we are.
* learning basic ETL concepts.

### The Future
* Finishing up learning
* writing more test cases for my backend.

