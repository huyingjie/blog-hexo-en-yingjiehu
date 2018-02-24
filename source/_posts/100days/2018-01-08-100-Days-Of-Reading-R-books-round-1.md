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
3. [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

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

### Day 5: 2018-01-18 Wednesday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* Page ~ 9

**Thoughts and Emotions**

I spent most of the time taking notes; I input syntax into my big programming sheet.

**Tomorrow's plan**

* [ ]Chapter 1

<hr>

### Day 6: 2018-02-03 Saturday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* Page 12, 13

**Thoughts and Emotions**

I spent most of the time taking notes; I input syntax into my big programming sheet.

No choice. If notes are not taken now, I will spend more time to search online to find them.

It is the choice between spending time now or spending more time in the future.

**Tomorrow's plan**

* [ ]Chapter 1

<hr>

### Day 7: 2018-02-04 Sunday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* Page 13-16

**Thoughts and Emotions**

Page 15 recommended several good functions to list packages installed on the computer and loaded in the session, and so on.

They are useful if I want to clean packages. One drawback of all R books I read so far is that none of them provide functions how to uninstall and unloaded packages.

I guess most of the R users do not uninstall packages after installing them. The same thing happened to load packages.

**Tomorrow's plan**

* [ ]Chapter 1

<hr>

### Day 8: 2018-02-06 Tuesday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* page 17 - 22
* Finished Chapter 1

**Thoughts and Emotions**

Page 18 

There are 7 steps in the example on "Section 1.8 Working through an example". I remember when I read the Chapter first time, I did not know how to do

```
3. List the functions and datasets available in the package
6. Run the example that comes with the Arthritis dataset
```

This time, I took notes during the reading and knew why this happened.

For the question 3, the book said you could find the functions of packages using the function `help(package="packageName"). The book used the different language between the content and the question

For the question 6, the book never said `example()` could accept a dataset name as the argument. It mentioned that examples of packages could be run by `example()`. Maybe the author hoped readers looked for answers by themselves by using `?example`.

**Tomorrow's plan**

* [ ] Chapter 2

<hr>

### Day 9: 2018-02-14 Wednesday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* Page 23 - 29

**Thoughts and Emotions**

* vector
* matrix
* array
* data frame
* factor

These were the most friction when I learned R at the beginning. R has the biggest number of data type among programming languages I learned so far. It is tough to change the mindset from C to R.

**Tomorrow's plan**

* [ ] Chapter 2

<hr>

### Day 10: 2018-02-16 Friday 

**Book**: [R in Action: Data Analysis and Graphics with R 2nd Edition](http://amzn.to/2DLB2xX)

**Today's Progress (achievements and frustrations)**: 

* Page 30 - 38

**Thoughts and Emotions**

There are a lot of types datasets. Each one has a different way. I am happy that inputting these into the programming language syntax table.

I input a lot of methods before. R in Action provided more. It is frustrating when every book gives a different subset of all possible types of datasets. 

Importing `xlsx` files requires `Java`. I used package `XLConnect` several years. I re-ran the code again last year, and there were some errors with `Java`. Searching online did not give me an effective solution. 

Again, the more stuff one package depends on, the less possibility of code that can be reproduced in the future.

Reducing dependencies is the key to reproducibility. The importance of reproducible reports is much lower than dependencies.

**Tomorrow's plan**

* [ ] Chapter 2

<hr>