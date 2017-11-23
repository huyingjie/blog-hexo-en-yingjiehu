---
layout: post
isquiz: Yes
title:  "Tutorials to add/edit problems in quiz"
date: 2017-11-22
tags: []
categories: []
permalink: Tutorials-to-add-edit-problems-in-quiz
description:	""
papersummaryurl: 
filename: 
---
After reading a paper, if you think of some interesting questions that can be used to test the understanding of the paper, you can add questions and their solutions. Or If you find an error or own a better way to the solution, you definitely should add them. <!-- more -->

## Examples

### Example 1
#### Result

<fieldset>
Which of these is an example of a categorical variable?

1. flavor of soft drink ordered by each customer at a fast food restaurant.
2. height, measured in inches, for each student in a class
3. points scored by each player on a team

<div class="clickanswer">Show Answer</div><div class="answer">1
2 & 3 are continous variables.
</div>
</fieldset>

#### Code

```html
Which of these is an example of a categorical variable?

1. flavor of soft drink ordered by each customer at a fast food restaurant.
2. height, measured in inches, for each student in a class
3. points scored by each player on a team

<div class="clickanswer">Show Answer</div><div class="answer">1
2 & 3 are continous variables.
</div>
```

### Example 2
#### Result
<fieldset>
Let $X_1, ..., X_n$ be a random sample from an exponential($\beta$) population. 

What is the joint pdf of the sample?

<div class="clickanswer">Show Answer</div><div class="answer"> 
$f(x\_1, \dots, x\_n|\beta) = \sum\limits\_{i=1}^n f(x\_i|\beta) = \sum\limits\_{i=1}^n \frac{1}{\beta}e^{-x\_i/\beta}=\frac{1}{\beta^n}e^{-(x\_1+\dots+x\_n)/\beta}$
</div>
</fieldset>

#### Code
```html
Let $X_1, ..., X_n$ be a random sample from an exponential($\beta$) population. 

What is the joint pdf of the sample?

<div class="selection">Show Answer</div><div class="response"> $f(x_1, \dots, x_n|\beta) = \sum\limits_{i=1}^n f(x_i|\beta) = \sum\limits_{i=1}^n \frac{1}{\beta}e^{-x_i/\beta}=\frac{1}{\beta^n}e^{-(x_1+\dots+x_n)/\beta}$

</div>
```

## Syntax

Quizes in this website are created by `LaTex`, `Markdown`, `HTML`, `CSS` and `Javascript`. 

* Basic understanding of `MarkDown`, `HTML`, `CSS` is sufficient to write questions and answers that can be run by the website. 
* `LaTex` is a tool to write mathematics formulas. Every `_` should be escaped. For example, `x_i` is written as `x\_i`.
* You do not need to know anything about `Javascript`. Because it is run in the back-end and we write questions and answers in the front-end.


### Template

```html
<fieldset>
Questions are placed here

1. option one
2. option two
3. option three

<div class="clickanswer">Show Answer</div><div class="answer">Write answer here
</div>

</fieldset>
```
You can copy this template as a starting point when you start creating a question-answer group.

### fieldset

Each question starts with `<fieldset>` and ends with `</fieldset>`

They are required tags.

If they are not included, clicking `Show Answer` will open answers to all problems.

### Question Description

Question Description uses Markdown. It can include LaTex math formulas.

### Math formulas

Math formulas are supported by `MathJax`. They begin and end with `$`. 

Note: Every `_` should be escaped. For example, `x_i` is written as `x\_i`.

### "Show answer"

```html
<div class="clickanswer">Show Answer</div><div class="answer">Write answer here
</div>
```
* The text `Show Answer` should not be changed.
* Except last HTML tag `</div>`, all tags do not have space between them. For example, there is no space between two `div` tags, `</div><div class="answer">`.
* `Write answer here` is a place to put your answer. There is no space between the beginning of the answer and the beginning tag `<div class="answer">`
