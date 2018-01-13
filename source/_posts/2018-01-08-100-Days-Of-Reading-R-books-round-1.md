---
layout: post
title: "100 Days Of Reading R books (Round 1)"
date: 2018-01-08
tags: 
	- 100 Days Challenge
	- R
	- data analysis
categories: 
	- [100 Days Challenge, Data Science]
	- [Programming Language, R]
permalink: 100-Days-Of-Reading-R-books-Round-1
---
Main Commitment: I will read books about R at least 30 minutes per day for the next 100 days.

Start Date: 2018-01-08

A companion project to [100 Days of Reading Paper](100-Days-Of-Reading-Paper-Round-1).

<!-- more -->

## Rules

1. I will read books about R at least 30 minutes every day.
2. I will [tweet my progress every day](https://twitter.com/yingjieYJH), with the hashtag `#100DaysOfReading #100DaysOfX #rstat #DataScience` and note which day of the challenge I’m on.
2. I will track my progress here and push to GitHub.
3. I will only skip a day if something important comes up. And when I resume, I won’t count the day I skipped as one of my 100 days.
4. I will encourage and support at least two people each day in the `#100DaysOfReading` challenge on Twitter. I can read at most 5 tweets about `#100DaysOfReading` each day. Less is more. Don't spend more than enough time on the social networking website.

	3 Options
	
	* Like tweets
	* Leave a comment
	* (optional) Looking at their projects and giving them feedback (no more than 10 minutes per day)


## Some important additional considerations

* Don't skip two days in a row, and try not to skip more than 1 day in 2 weeks.

## Motivations

I had read some R books in the past. At that time, I input the knowledge into [Anki](https://apps.ankiweb.net/) and hoped that I could remember it in the future. 

My goal of reading books changes. I made some big tables of programming languages and input the R syntax into the tables. There are some other programming languages in it, such as Python and JavaScript. 

I will not memorize any R syntax anymore. Every time I want to use something, the tables are the first place to check. Besides, it is convenient to compare different languages.

It is tough to memorize syntax if multiple programming languages are used in the same period.

For example, all languages have boolean, the most basic variable type. There are two values, true or false.

* Python: True, False
* R: TRUE, FALSE
* JavaScript: true, false

You can get it. There are 3 ways to present boolean. My brain is reluctant to memorize which language uses which method.

Other examples:

* How to define a function?
* Whether variables should be declared before usage?
* Whether variables types should be written when we create variables
* Whether there is a keyword to declare a variable?
* and more

If you can memorize details of all programming languages you have learned, you are genius in my eyes.


## Books

1. [An R Companion to Applied Regression 2nd Edition](http://amzn.to/2DmDISd)
2. [Using R and RStudio for Data Management, Statistical Analysis, and Graphics (second edition)](http://amzn.to/2CRckuJ)

## Milestone

* [1 Day: 2018-01-08 Monday](#Day-1-2018-01-08-Monday)
* 7 Days
* 30 Days
* 60 Days
* 90 Days
* 100 Days
	
## Template for Log
```
### Day : 

**Book**: []()

**Today's Progress (achievements and frustrations)**: 

**Thoughts and Emotions**

**Tomorrow's plan**

<hr>
```

## LOG
### Day 1: 2018-01-08 Monday

**Book**: [An R Companion to Applied Regression 2nd Edition](http://links.yingjiehu.com/R-Companion-Applied-Regression-2nd-ed)

**Today's Progress (achievements and frustrations)**: 

* Read from xvii to page 8

**Thoughts and Emotions**

I had read the first two chapters before. At that time, I input the knowledge into [Anki](https://apps.ankiweb.net/) and hoped that I can remember it in the future. 

My goal of reading this book changes. I will input the syntax into the programming language table.

**Tomorrow's plan**

* [ ]Read Chapter 1

<hr>

### Day 2: 2018-01-10 Wednesday 

**Book**: my R notes

**Today's Progress (achievements and frustrations)**: 

30 minutes

* Review R notes taken in the past

**Thoughts and Emotions**

My book is not beside me. I reviewed R notes taken in the past to continue the challenge.

I am happy to do that. 

1. Some old notes were deleted
2. I input notes to the large programming language sheet.

Statistical analysis programming languages have some unique data type that other languages do not have. 

For example, R has a `vector` data type. Elements in a vector have the same atomic data type, such as string or integer. 

Python has a `list` while JavaScript has an `array`. Both of them can create a vector of data, but their elements can be a mix of string and integer.

A more specific example:

JavaScript: `var ourArray = ["John", 23];`

Python: `things = [“shoes”, 85, 8.8, “ball”]`

R converts a vector of a mix of string and integer into a vector of string automatically. 

```r
> ourArray = c(23, "John")
> ourArray
[1] "23"   "John"
> things = c("shoes", 85, 8.8, "balls")
> things
[1] "shoes" "85"    "8.8"   "balls"
```

**Tomorrow's plan**
																		
* [ ]Read Chapter 1

<hr>

### Day 3: 2018-01-11 Thursday 

**Book**: [Using R and RStudio for Data Management, Statistical Analysis, and Graphics (second edition)](http://amzn.to/2CRckuJ)

**Today's Progress (achievements and frustrations)**: 

* Chapter 1: page 1-6

**Thoughts and Emotions**

The book is like a dictionary but is worse than a dictionary. 

It is not suitable for beginners. I am not a beginner and can try it. 

I spent most of taking notes: input the functions into my large programming language sheet.

**Tomorrow's plan**

* [x]Chapter 1

<hr>

### Day 4: 2018-01-12 Friday

**Book**: [Using R and RStudio for Data Management, Statistical Analysis, and Graphics (second edition)](http://amzn.to/2CRckuJ)

**Today's Progress (achievements and frustrations)**: 

* Page 7-14

**Thoughts and Emotions**

Most of time I did copy and paste from the book to my big sheet.

**Tomorrow's plan**

* [ ]Chapter 2

<hr>