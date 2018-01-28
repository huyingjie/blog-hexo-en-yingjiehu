---
layout: post
title: "100 Days Of Data Challenge (Round 1)"
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

**Modification** (2018-01-05): I found `The 5-Day Data Challenge
` in Kaggle today . I like `Data Challenge` better than `Data Analysis with R`. The title of the post was changed from `100 Days Of Code: Data Analysis with R (Round 1)` to `100 Days Of Data Challenge (Round 1)`. Even though no one tweets `#100daysOfData`, I want to use it.

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

5. I will tweet my progress every day, with the hashtag `#100DaysOfCode`, `#100daysOfData` and `#100DaysOfDataScience` and note which day of the challenge I’m on.
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
### Day 1: 2017-12-17 Sunday
**Today's Progress (achievements and frustrations)**: 

* import data into R


**Thoughts and Emotions**

The column name is messy after the data was imported into R. Thinking of the idea that I have to rename all columns one by one, I feel scared.

Today I learned parts of `tidyverse` package in Lynda.com. I thought it was a good package. When I start using it, I missed the old method. But when I saw base R converted all character variables into factor variable after import, I missed `tidyverse`. I had mixed feelings about both base R and `tidyverse`.

<hr>

### Day 2: 2018-01-03 Wednesday
**Today's Progress (achievements and frustrations)**: 

One hour work

* Cleaned the dataset column by column 
* Wrote a Markdown table to record

**Thoughts and Emotions**

I did not finish the cleaning. I know cleaning is faster if I use SAS. 

I know the one hour work is not productive. But it gave me less pressure.

I set a one-clock timer. I can feel that when it was approaching one hour, the stress level increased.

Every time I work long hour until burning out, it will make it harder to start work next time. My goal is not the speed or productivity but consistency.

**Tomorrow's plan**

* [ ]Clean data
* [ ]Make descriptive data of variables left in the cleaned data
* [ ]Write report
* [ ]Run simple logistic analysis of batch effect and `Reasons`

### Day 3: 2018-01-05 Friday

**Today's Progress (achievements and frustrations)**: 

I created [a R package project for beginners](http://rsnippets.com/r/create-a-package-of-personal-toolbox/) on RSnippets.com. It is to build a utility package for personal usage.

I started to make one.

**Thoughts and Emotions**

I did not do this challenge again. The small project can get me started. This is the reason I did a project for beginners, not a big project.

I feel good at the end of one-hour session. 

**Tomorrow's plan**

* [x]Clean data
* [ ]Make descriptive data of variables left in the cleaned data
* [ ]Write report
* [ ]Run simple logistic analysis of batch effect and `Reasons`


<hr>

### Day 4: 2018-01-06 Saturday

**Today's Progress (achievements and frustrations)**: 

* Read the post about how changing location will affect the linear regression result.
* Reproduce the example from `Sean`

I created 2 toy examples: 

1. $y = 0.2x$
1. $y = 0.2x+x^2$

$x$ is uniform(-0.5,0.5). $x$ in the program means uniform(0,1).

* If the true model is linear
	![](location affects coefficients linear.png)
		
	The above graph shows fitted models look almost the same when the location of $x$ is changed.
	
	![](location affects coefficients linear2.png)
	
	The above graph shows the intercept will decrease when the location of $x$ becomes bigger. This conforms to the mathematical proof.
	
	$$y = 0.2x = (0.2-0.2a) + (x+0.2a)$$ 
	
	$0.2-0.2a$ is the intercepts after $x$ moves. It has the linear relationship with $a$. 
	
	However, in theory, the coefficient of $x$ remains the same. In fact, it changes a little bit.

* If the true model is non-linear
	![](location affects coefficients quadratic.png)

	![](location affects coefficients quadratic2.png)
	
	The above two graphs show that the location has big impact on cofficients for non-linear models.
	
	1. Around 800 and -800, `lm` fails to estimate a coefficient for the quadratic term, & gives a warning about a singular design matrix. 
	2. The relationship between intercept and location is not linear anymore.

In summary, if the scale of predictors is big, such as over 800, it is a good choice to center them first before performing any data analysis.

R code

```r
set.seed(1)
n <- 100
x <- sort(runif(n))
y <- .2*(x-.5)+(x-.5)^2 + rnorm(n)*.1
y_linear <- .2*(x-0.5) + rnorm(n)*.1

# x100 <- x+100
# b100 <- lm(y ~ x100 + I(x100^2))
# plot(x100,y)
# lines(x100, predict(b100), col='red')

# x is gerenated outside function
locale <- function(x, y, a, is_graph = TRUE){
  x_locale <- x+a
  b <- lm(y ~ x_locale + I(x_locale^2))
  if(is_graph){
    plot(x_locale,y, main = paste("locale = ", a))
    lines(x_locale, predict(b), col='red')
  }
  return(b)
}

par(mfrow = c(2,2))
locale(x, y, 0)
locale(x, y, 100)
locale(x, y, 500)
locale(x, y, 1000)

b_vector <- matrix(nrow=0, ncol=3)
for (i in -1000:1000){
  b_vector <- rbind(b_vector, locale(x, y, i, is_graph = FALSE)$coefficient)
}
rm(i)
colnames(b_vector) <- c("intercept", "x", "x^2")
par(mfrow = c(3,1))
plot(-1000:1000, b_vector[,"intercept"], ylab = "intercept")
plot(-1000:1000, b_vector[,"x"], ylab = expression(beta[1]))
plot(-1000:1000, b_vector[,"x^2"], ylab = expression(beta[2]))

############################

locale_linear <- function(x, y, a, is_graph = TRUE){
  x_locale <- x+a
  b <- lm(y ~ x_locale)
  if(is_graph){
    plot(x_locale,y, main = paste("locale = ", a))
    lines(x_locale, predict(b), col='red')
  }
  return(b)
}

par(mfrow = c(2,2))
locale_linear(x, y_linear, 0)
locale_linear(x, y_linear, 100)
locale_linear(x, y_linear, 500)
locale_linear(x, y_linear, 1000)

b_vector_linear <- matrix(nrow=0, ncol=2)
for (i in -1000:1000){
  b_vector_linear <- rbind(b_vector_linear, locale_linear(x, y_linear, i, is_graph = FALSE)$coefficient)
}
rm(i)
colnames(b_vector_linear) <- c("intercept", "x")
par(mfrow = c(2,1))
plot(-1000:1000, b_vector_linear[,"intercept"], ylab = "intercept")
plot(-1000:1000, b_vector_linear[,"x"], ylab = expression(beta[1]))

```

**Thoughts and Emotions**

I feel good that I finished the toy examples.

I feel bad that they were supposed to take less time.

**Tomorrow's plan**

* [ ]Read online posts about normalized data
* [ ]Make descriptive data of variables left in the cleaned data
* [ ]Write report
* [ ]Run simple logistic analysis of batch effect and `Reasons`

<hr>

### Day 5: 2018-01-15 Monday 

**Today's Progress (achievements and frustrations)**: 

* Data analysis for over 3 hours.

**Thoughts and Emotions**

The most accomplished thing is to find how to reduce variables required to be created or reduce the number of global variables.

When fitting each model, I have to create intermediate variables, such as a variable `fit` to keep the information of fitted models. Every time, I have to think hard to give each variable a different name, or make sure I run all code if the same variable names are reused.

The intermediate variables are all global variables. It is the user's responsibility to delete unused variables. 

It is worse that variables like `i` or `j` created at the beginning of the loop are not temporary variables! 

Now I found a solution: use `with` function.

Let me use `iris` dataset as an example. By the way, `iris` is a global variable name for the dataset. Very bad practice.

```r
> head(iris)
  Sepal.Length Sepal.Width Petal.Length Petal.Width Species
1          5.1         3.5          1.4         0.2  setosa
2          4.9         3.0          1.4         0.2  setosa
3          4.7         3.2          1.3         0.2  setosa
4          4.6         3.1          1.5         0.2  setosa
5          5.0         3.6          1.4         0.2  setosa
6          5.4         3.9          1.7         0.4  setosa
```

For example, I want to fit two logistic models. They include different independent variables. Model 1 uses `length` and `width` while Model 2 uses `width` only. 

```r

# Model 1
fit <- glm(Species ~ Sepal.Length + Sepal.Width, 
	family=binomial(link='logit'), 
	data = iris,
	control = list(maxit = 50))
summary(fit)

# Model 2
fit <- glm(Species ~  Sepal.Width, 
	family=binomial(link='logit'), 
	data = iris, 
	control = list(maxit = 50))
summary(fit)
```

Two models used the same variable to `fit` to save the information from `glm`. `fit` is a global variable. In fact, `fit` is an intermediate variable and is not useful at the end of data analysis. This is also the reason to reuse it in a different model. It is a poor coding style. I have several choices.

1. Use a different name for `fit` for different models. 

    Usually, I will fit a lot of models during data analysis. Keeping track of the model fit requires patience.
    
2. Set `fit` as a local variable in a function
    
    Write a function for each model? The same problem exists as above: keeping track of the function requires patience.
    
3. Set `fit` as a local variable within `with` function.

    My choice.
    
Let me rewrite the code.

```r
with(iris, {
  fit <- glm(Species ~ Sepal.Length + Sepal.Width, 
  	family=binomial(link='logit'), 
  	data = iris, 
  	control = list(maxit = 50))
  print(summary(fit))
}
)

with(iris, {
  fit <- glm(Species ~  Sepal.Width, 
  	family=binomial(link='logit'), 
  	data = iris, 
  	control = list(maxit = 50))
  print(summary(fit))
})
```	

The `fit` variable in each `with` function will not affect each other. It will disappear when `with` ends. Excellent!

**Tomorrow's plan**

* [ ]Meeting
* [ ]Refine

<hr>


**Future's plan**

* [ ]Read source code of Relaxed Lasso's R package