---
layout: post
title: "Gumroad Plan Calculator"
date: 2018-01-08
tags:
	- calculator
	- gumroad
	- javascript
categories:
	- [Projects]
permalink: Gumroad-Plan-Calculator
---

<img src="../img/Gumroad-Plan-Calculator.png"> 
<!-- more -->

This project was done in the middle of [100 Days of Web Develpoment challenge](/100-Days-Of-Web-Development-Round-1/).

[Github Repo](https://github.com/huyingjie/gumroad-plan-calculator) | [Project 13: Gumroad Plan Calculator](http://gumroadplancalculator.yingjiehu.com/)

Link: [http://gumroadplancalculator.yingjiehu.com/](http://gumroadplancalculator.yingjiehu.com/)

## Motivation

Gumroad is a website to sell digital products or give out for free. The design of sales pages is convenient for customers to purchase products and the appearence of pages are comfortable to eyes.

Gumroad has two plans, free plan and premium plan.

* Free plan: 8.5% + 30 cents per sale
* Premium plan: 3.5% + 30 cents per sale

Gumroad did a trick on their website.

Here is the [pricing page](https://gumroad.com/features/pricing).

![gumroad pricing](gumroad-pricing.png)

"Starts at $\$10$ a month" means there are other plan(s) to charge more. Then I clicked "Learn more" and [it gave me](https://gumroad.com/discover):

![gumroad pricing learn more](learn-more.png)

"Learn more" pages does not give me more information. After searching online, I found the ["billing ties" page](https://help.gumroad.com/billing-tiers). Some users wrote the explanation of the billing tiers in details. They asked Gumroad to define "the number of customers". Gumroad replied that it was the cumulative number of customers!!!!

![](gumroad-billing-ties.png)

It is not a good premium plan. For example, you create a game and allow other people to download for free. If there are over 5,000 downloads, your premium monthly fee is at least $\$75$. (It is easy to pass 5,000 downloads for a free game.) Then you create another game and charge fees before downloading. You have to calculate which plan will charge less.

The calculation is not hard. However, it is nice if there exists a calculator we can use immediately.

P.S.: The other solution: You can create two Gumroad accounts, one for free stuff and the other for paid products.

## Milestone

1. The website was published to internet. ([2018-01-08 Monday](#2018-01-08-Monday))

## Support open source projects

<a href="https://www.patreon.com/bePatron?u=8604867" data-patreon-widget-type="become-patron-button">Become a Patron!</a><script async src="https://c6.patreon.com/becomePatronButton.bundle.js"></script>

## 2018-01-08 Monday

I spent 3 hours on the project today. I planned to do it for one hour per day, but cannot stop coding. 🤣
