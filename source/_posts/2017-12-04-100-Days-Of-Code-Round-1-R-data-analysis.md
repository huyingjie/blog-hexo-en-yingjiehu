---
layout: post
title: "100 Days Of Code: Data Analysis with R (Round 1)"
date: 2017-12-11
tags: 
	- 100 Days Challenge
	- R
	- data analysis
categories: 
	- [100 Days Challenge, Data Science]
	- [Programming Language, R]
permalink: 100-Days-Of-Code-R-data-analysis-Round-1
---
Main Commitment: I will code to do data analysis for at least an hour every day for the next 100 days.

Start Date: 2017-12-11

A companion project to [100 Days of Reading Paper](100-Days-Of-Reading-Paper-Round-1).

<!-- more -->

## Rules

1. I will code using R or do data analysis with other software (such as Python) for at least an hour every day.
2. Projects are counted towards the challenge:
	* statistical analysis projects in my work
	* projects from dissertation
	* competitions, such as Kaggle

3. Activties are counted towards the challenge:
	* understand datasets in excel
	* import data into R
	* clean data
	* write codes to do exploratory analysis and apply statistical model
	* write statistical reports

4. Activities are not counted towards the challnege:

	* write emails to clients
	* meet with clients/supervisors

5. I will tweet my progress every day, with the hashtag `#100DaysOfCode` and `#100DaysOfDataScience` and note which day of the challenge I’m on.
6. I will encourage and support at least two people each day in the `#100DaysOfDataScience` challenge on Twitter. I can read at most 5 tweets about `#100DaysOfDataScience` every day. Less is more. Don't spend more than enough time on the social networking website.

    3 Options
    
    * Like tweets
    * Leave a comment
    * (optional) Looking at their projects and giving them feedback (no more than 10 minutes per day)
7. I will track my progress here and push to GitHub.
8. I will only count the days where I spend at least some of my time building projects — not the days where I spend all my coding time working through lessons and tutorials.

9. I will only skip a day if something important comes up. And when I resume, I won’t count the day I skipped as one of my 100 days.

## Some important additional considerations

* Don't skip two days in a row, and try not to skip more than 1 day in 2 weeks.

## Reference
[How to effectively scope your software projects from planning to execution](https://medium.freecodecamp.org/how-to-effectively-scope-your-software-projects-from-planning-to-execution-e96cbcac54b9)

### The planning phase

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
	
### The scoping phase

1. Divide the project into small tasks, **each taking two days or less**. 
1. Define measurable milestones to get to the project goal. Schedule each with a specific calendar date representing when you expect this milestone to be reached. Then, establish some sort of external accountability on these milestones by, for example, committing them to your manager and setting up milestone check-ins.
1. Think of project time estimates as probability distributions, not best-case scenarios. Instead of telling someone that a feature will be finished in 6 weeks, tell them something like “there’s a 50% likelihood of finishing the feature in 4 weeks, and a 90% chance we’d finish it in 8 weeks.” This tends to force people to be more realistic.
1. Add buffer to account for: (1) Dev time != calendar time, due to meetings, interviews, and holidays. I usually multiply the dev time by 1.5 to get to the calendar time. (2) Unexpected project tasks time, since there are always tasks that you didn’t realize you need to do until much later. These tasks could include refactoring old code, debugging strange behaviors, or adding tests. The more experienced you are at scoping, the smaller this multiplier will get.
1. Resist the temptation to under-scope. Be honest about how long tasks will take, not how long you or someone else (such as your manager or the Go To Market team) wants them to take.
1. Use historical data. Keep track of whether you’ve tended to over scope or under scope projects in the past (most people tend to under scope). Adjust your scoping accordingly.
1. Consider timeboxing open-ended parts of the project. Instead of “find the best stream processing framework for this system,” which can take months of research and prototyping, timebox it to “find a suitable streaming processing framework in a week.” Use your judgment here to balance this against incurring long-term operational overhead.

### The execution phase
* Re-scope regularly during the project execution. 

	For each task, track how much time you estimated the task would take, then how long it actually took you to complete it. 
	
	Do this for every measurable milestone. 
	
	If your scoping is off by 50% for the first parts of the project, odds are your scoping will also be off by 50% for the rest of the project.

* Use milestones to answer “how’s the project going?” 

	As engineers, it’s tempting to answer “it’ll be done by next week” or “until end of this month.” But these types of vague answers tend to create projects that are always 2 weeks away from being finished. Instead, use the (re-scoped) milestones to give a concrete answer based on how much work is left.

## Template for Log
```
### Day : 

**Link**: [Github Repo]() | [Project :]()

**Today's Progress (achievements and frustrations)**: 

**Thoughts and Emotions**

**Tomorrow's plan**

<hr>
```

## LOG
### Day 1: 2017-12-17
**Today's Progress (achievements and frustrations)**: 

* import data into R


**Thoughts and Emotions**

The column name is messy after the data was imported into R. Thinking of the idea that I have to rename all columns one by one, I feel scared.

Today I learned parts of `tidyverse` package in Lynda.com. I thought it was a good package. When I start using it, I missed the old method. But when I saw base R converted all character variables into factor variable after import, I missed `tidyverse`. I had mixed feelings about both base R and `tidyverse`.

<hr>

### Day 2: 2018-01-03
**Today's Progress (achievements and frustrations)**: 

One hour work

* Cleaned the dataset column by column 
* Wrote a Markdown table to record

**Thoughts and Emotions**

I did not finish the cleaning. I know cleaning is faster if I use SAS. 

I know the one hour work is not productive. But it gave me less pressure.

I set a one-clock timer. I can feel that when it was approaching one hour, the stress level increased.

Every time I work long hour until burning out, it will make it harder to start work next time. My goal is not the speed/productivity but consistency.

**Tomorrow's plan**

* [ ]Clean data
* [ ]Make descriptive data of variables left in the cleaned data
* [ ]Write report
* [ ]Run simple logistic analysis of batch effect and `Reasons`

<hr>

**Future's plan**