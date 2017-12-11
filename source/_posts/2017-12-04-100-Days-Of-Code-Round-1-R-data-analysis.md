---
layout: post
title: 100 Days Of Code Round 1 (R, data analysis)
date: 2017-12-11
tags: 
	- 100 Days Challenge
	- R
	- data analysis
categories: 
	- 100 Days Challenge
	- R
permalink: 100-Days-Of-Code-Round-1-R-data-analysis
---
A companion project to [100 Days of Reading Paper](100-Days-Of-Reading-Paper-Round-1).

Main Commitment: I will code to do data analysis for at least an hour every day for the next 100 days.

Start Date: 2017-12-11
<!-- more -->

Reference: [How to effectively scope your software projects from planning to execution](https://medium.freecodecamp.org/how-to-effectively-scope-your-software-projects-from-planning-to-execution-e96cbcac54b9)
## Rules

1. I will code using R or do data analysis with other software (such as Python) for at least an hour every day.
2. I will tweet my progress every day, with the hashtag `#100DaysOfCode` and `#100DaysOfDataScience` and note which day of the challenge I’m on.
3. I will track my progress here and push to GitHub.
4. If I code as part of my job, I will still count that time towards the challenge.
5. I will only count the days where I spend at least some of my time building projects — not the days where I spend all my coding time working through lessons and tutorials. (If you’re new to coding, Free Code Camp’s curriculum quickly ramps up to building projects, and you will have built dozens of projects by the time you finish it).
6. I will encourage and support at least first two people each day in the `#100DaysOfCode` challenge on Twitter. I can read at most 5 tweets about `#100DaysOfCode` each day. Less is more. Don't spend more than enough time on the social networking website.

	3 Options
	
	* Like tweets
	* Leave a comment
	* (optional) Looking at their projects and giving them feedback (no more than 10 minutes per day)
7. I will only skip a day if something important comes up. And when I resume, I won’t count the day I skipped as one of my 100 days.
7. Working on competitions like Kaggle will definitely be counted towards the challenge.

Note: Projects from dissertation do not belong to `work` mentioned above.

## Some important additional considerations

* If you can, try not to use tutorials, but build real projects — they can range from simple pages to full-fledged web apps.
* Don't skip two days in a row, and try not to skip more than 1 day in 2 weeks.


The projects that you’ll build will be small in scope, so by the time you finish, you’ll have completed several of them — and gained a wide range of experience.

## The planning phase

* Define very specific goals for the project

	example: improve X by adding unit tests, supporting 20K queries per second, and reducing capped mean of user latency to <= 200ms
	
* Explicitly define anti-goals, and separating must-haves and nice-to-haves.
* Minimize the batch size of the project by

	1. set up clear milestones and checkpoints for the project
	1. make it easy to launch only part of the project. 

		Not only does this help break down the project, but it will also allow the team to pause or cut the project early if another, higher priority task comes up.
		
* De-risk the project as soon as possible. 

	Two common ways of de-risking a project include
	
	1. working on the riskiest parts upfront
	1. prototyping the riskiest parts using dummy data and/or scaffolding. 

	Whenever a new open-source system or external service is used, that usually represents a big risk.
* Don’t optimize for the total amount of work done. Instead, optimize for the total amount of impact over time. Once you’ve gotten the riskiest part out of the way, prioritize working on the part of the project that would result in the highest amount of impact immediately.
	
	Here’s one way to think about this: plot the impact of a project over time, where the Y-axis is impact, and the X axis is time. At the start of the project, the impact is 0%, and at the end of the project, the impact is 100%. You want to maximize the area under the curve by doing high ROI tasks first.

* Try to avoid rewriting big systems from scratch as much as possible. When doing a rewrite, we tend to 

	1. underestimate how much work it would be
	1. be tempted to add new features and improvements
	1. build an overly complicated system because we are too focused on all the shortcomings of the first system.

	Instead of doing a big rewrite, consider incrementally replacing subsystems. Have good abstraction layers that support swapping out one part of the old system at a time, so you don’t need to wait for everything to be done to test the new system.
	
## The scoping phase

1. Divide the project into small tasks, **each taking two days or less**. 
1. Define measurable milestones to get to the project goal. Schedule each with a specific calendar date representing when you expect this milestone to be reached. Then, establish some sort of external accountability on these milestones by, for example, committing them to your manager and setting up milestone check-ins.
1. Think of project time estimates as probability distributions, not best-case scenarios. Instead of telling someone that a feature will be finished in 6 weeks, tell them something like “there’s a 50% likelihood of finishing the feature in 4 weeks, and a 90% chance we’d finish it in 8 weeks.” This tends to force people to be more realistic.
1. Add buffer to account for: (1) Dev time != calendar time, due to meetings, interviews, and holidays. I usually multiply the dev time by 1.5 to get to the calendar time. (2) Unexpected project tasks time, since there are always tasks that you didn’t realize you need to do until much later. These tasks could include refactoring old code, debugging strange behaviors, or adding tests. The more experienced you are at scoping, the smaller this multiplier will get.
1. Resist the temptation to under-scope. Be honest about how long tasks will take, not how long you or someone else (such as your manager or the Go To Market team) wants them to take.
1. Use historical data. Keep track of whether you’ve tended to over scope or under scope projects in the past (most people tend to under scope). Adjust your scoping accordingly.
1. Consider timeboxing open-ended parts of the project. Instead of “find the best stream processing framework for this system,” which can take months of research and prototyping, timebox it to “find a suitable streaming processing framework in a week.” Use your judgment here to balance this against incurring long-term operational overhead.

## The execution phase
* Re-scope regularly during the project execution. 

	For each task, track how much time you estimated the task would take, then how long it actually took you to complete it. 
	
	Do this for every measurable milestone. 
	
	If your scoping is off by 50% for the first parts of the project, odds are your scoping will also be off by 50% for the rest of the project.

* Use milestones to answer “how’s the project going?” 

	As engineers, it’s tempting to answer “it’ll be done by next week” or “until end of this month.” But these types of vague answers tend to create projects that are always 2 weeks away from being finished. Instead, use the (re-scoped) milestones to give a concrete answer based on how much work is left.

## Template for Log
```
### Day : 
**Today's Progress (achievements and frustrations)**: 
**Thoughts and Emotions**
**Github Repo**: 
```

## LOG
### Day : 
**Today's Progress (achievements and frustrations)**: 
**Thoughts and Emotions**
**Github Repo**: 