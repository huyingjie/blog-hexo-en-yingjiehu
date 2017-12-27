---
layout: post
title: Awesome Shiny Apps for Statistics
date: 2017-12-25
tags: 
	- Shiny
	- R
	- gulp
categories: 
	- [Projects]
permalink: Awesome-Shiny-Apps-for-Statistics

---
![](/img/Awesome-Shiny-Apps-for-Statistics.png)
<!-- more -->
This project was done in the middle of [100 Days of Web Develpoment challenge](/100-Days-Of-Web-Development-Round-1/).

[Github Repo](https://github.com/huyingjie/Awesome-shiny-apps-for-statistics) | [Project 9: Awesome Shiny Apps for Statistics](http://asas.yingjiehu.com/)

Yesterday's night, I suddenly had an idea to make a GitHub awesome list of Shiny Apps. The apps are specific for learning statistics, not showing results from data analysis. It is better if there will be a website automatically generated from `README.md` file from the GitHub repo, then the effort to keep the website and `README.md` being same will be zero. Usually, people contribute to an awesome list by editing `README.md`. It is the  owner's responsibility of the GitHub repo to sync between GitHub and the website. 

How to sync automatically is the most difficult part for me. My blog is using Netlify to automatically deploy. I need to learn one templating engine to combine data in `README.md` and templates created by a templating engine by Netlify. I started to learning `Go` on the YouTube. I realized that `Go` was a completely new language and if I wanted to use it, I had to learn a lof things. Then I recalled [Front-End-Checklist](https://github.com/thedaviddias/Front-End-Checklist#table-of-contents) using `gulp`. Initially, I thought `gulp` was a template engine. After reading one tutorial, I knew it was not and can use it to create a web page without styling through `gulp-markdown`. `gulp-rename` is used to change the filename from `README.md` to `index.md`, then `gulp-markdown` generated `index.html`. The HTML codes inside `index.html` do not contain `head` and `body` elements. It turns out to be an advantage. `gulp-wrapper` adds `head` and `body` elements before and after the codes. The resulting website was successfully deployed by Nelify. I achieved to sync between `README.md` and the website.

Today, I spent time in changing the website style and gathered Shiny apps.

I worked more than 10 hours today. I am satisfied with the result. One thing needed to improve in the future is the styling of the site.

## Update 2017/12/26 Tuesday

![](2017-12-26-GitHub-Data.png)

![](2017-12-26-Twitter-Data.png)

After one day of publishing, some numbers

* GitHub

	* 16 stars
	* 3 forks
	* 3 watchers

* Twitter
	* 31 Tweeted
	* 77 likes

This is the first for me to get over 10 stars on GitHub and the first to get over 10 likes on Twitter. I am happy that people like the idea of the project.