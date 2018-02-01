---
layout: post
title: "A-RSnippet Hexo Theme"
date: 2018-01-24
tags:
	- Hexo
categories:
	- [Projects]
permalink: a-rsnippet-hexo-theme
---

<img src="/img/2018-01-24-A-RSnippet.png"> 
<!-- more -->

This project was done in the middle of [100 Days of Web Develpoment challenge](/100-Days-Of-Web-Development-Round-1/).

[Github Repo](https://github.com/huyingjie/hexo-theme-A-RSnippet) | [Project 15: Hexo theme A-RSnippet](http://arsnippet.yingjiehu.com/)

Link: [http://arsnippet.yingjiehu.com/](http://arsnippet.yingjiehu.com/)

## Motivation

I wanted to build/customize a theme for saving my solution to leetcode algorithm challenges. 

First, I chose Hugo because of its speed. There is a big drawback that made me gave it up. Hugo will updates automatically when users write posts; it deploys constantly. To achieve this, Hugo saves the contents in the memory. It is the best choice for people who write posts only. It becomes a big pain for developers since Hugo will delay to update if files of themes are changed. I cannot tell immediately whether my code is working or not and have to wait for Hugo for an unknown length of time.

Then I tried Hexo. My blog was made from Hexo and I like it very much. After hours of searching, I finally chose [hexo-theme-Anisina](https://github.com/haojen/hexo-theme-Anisina). I read the code and thought it was messy. I deleted some code and added more features.

I spent 12 hours 😵 (eating time included) to read 184 themes one by one. There are some features I put in my future's todo list.


On January 19, 20, 21, 22, 23, and 24 (six days), I released the version 0.1.0 and submitted it [Hexo website](https://hexo.io/themes/).

Though minimalism is good and simplicity seems nice, I want to have more features. The goal of the theme is to include as many features as possible. 


## A-RSnippet Theme community

I hope this open source project is sustainable and can last for a long time. This is the reason I created Discord, Patreon, an email newsletter, and a forum. Together with GitHub issues, they serve all purposes.

1. [Forum](https://arsnippet.freeflarum.com/)

	The community can help each other. New users can search all tutorials and former problems here.
	
2. [Discord](https://discord.gg/CB6CPzq)

	I am accessible in person on Discord. I set a limitation.
	
	In the public channels on Discord, people are forced to speak English only because I want to build an international community, not just for Chinese. (95% of themes on official Hexo website were made by Chinese). Hexo is so powerful that I hope it can attract more people.
	
	After the problems are solved, people are required to create new posts on the forum to describe the solution.
	
	A private channel is for users from Patreon.
	
	A private channel is for sponsors if I can have one.
	
3. [Patreon](https://www.patreon.com/arsnippet)
	
	I appreciate people who support the development by giving me money. They are the people to whom I should pay attention and give more service.
	
	When people become a backer, they will be automatically added to Discord and assigned special badges. They can access a private channel. In the channel, they can ask me questions in Chinese and write posts for them if questions are answered.
	
	After each release, I will create a poll of potential new features for the next release. It is how I take care of people on Patreon within my limited time. 

4. [GitHub issues](https://github.com/huyingjie/hexo-theme-A-RSnippet/issues)

	New issues and features I decide to develop for the next release.

5. Email newsletter

	GitHub will notify users if a new version is released. This bothers me a lot when I use some open-source projects. I have to check their repos regularly or do not update anymore. 
	
	Users can subscribe to the email newsletter to get updated for each new release.
		
6. If I have over 10 backers on Patreon, I will try streaming to answer users' questions on Twitch.

## Milestone

1. Submit A-Rsnippet theme to Hexo website and release v0.1.0. ([2018-01-24 Wednesday](#2018-01-24-Wednesday))
2. [The first star](#2018-01-25-Thursday)

## 2018-01-24 Wednesday

* v0.1.0
	* 2018-01-23 Make an `exampleSite` folder included in the theme folder
	* 2018-01-24
		* Write documentation
		* Found more bugs when writing documentation
		* Adjust the example site
		* Create a Discord Channel
		* Create a Patreon page
		* Connect Patreon to Discord
		* Create a cover photo for the theme
		* Build a brand new website to test the example website
		* Upload to GitHub
		* Use Netlify
		* Add a subdomain name
		* Google site verification
		* Submit the theme to Hexo

This is my first time to pull request!!!

This is my frist time to release!!!

![](2018-01-24-A-RSnippet-hexo-my-first-commit.png)

My theme is the frist one on Hexo theme page because of alphabetical order 😂

![](2018-01-24-A-RSnippet-hexo-official-website.png)


## 2018-01-25 Thursday

### the first star

The first star is from [nogajun](https://github.com/nogajun), a Japanese guy. Thank you!! ありがどう

![](2018-01-25-first-star.png)

### Setup a new forum

I searched online and found [flarum](http://flarum.org/). It is a forum app that uses PHP. I like discord and NodeBB. Because both of them require cloud server, I have to pay an additional fee if I use them. 

Luckily, I found a website [freeflarum.com](http://freeflarum.com) that hosts Plarum forum for free. Their business model is to show some ads on the free forums. So far, I do not see any ads and am not sure when and what ads will show.

Making open source project is really time-consuming. If there is no sustainable business model, most of good open-source repos will not update regularly.

![](2018-01-25-forum.png)

### Create guidelines on the forum

I copied some guidelines from official flarum forum and added instructions for each type of posts. I took me hours to finish. Maintaining open-source project is time-consuming.

	### Thank you for choosing A-RSnippet theme. 
	
	This forum was built on freeflarum.com for free. freeflarum.com will show some ads to maintain the free service. I cannot control the content of ads or whether ads will show or not.
	
	You can use MarkDown to write posts.
	
	## 1. All discussion on the forum uses English only.
	If you want to use languages other than English, please use the following format:
	[your language in English] xxxx
	[English] yyy
	
	Example:
	
	[Chinese] 除了一个Discord私人频道(你可以通过[Patreon](1)加入), 在论坛和Discord里发言只允许使用英文.
	[English] Except a private Discord channel (you can join in via [Patreon][1]), all discussions on the forum and Discord must use English only.
	
	## 2. Ask-For-Help 
	
	1. Please read the [tutorial][2] first
	2. Search the forum for your question
	3. If you cannot find answers using the above two methods, you can create a new post under the tag `Ask-For-Help` using following format. After the question is solved, you must change the tag from `Ask-For-Help` to `Solved`.
	
	IF YOU DON'T FILL OUT THE FOLLOWING INFORMATION WE MIGHT CLOSE YOUR POST WITHOUT INVESTIGATING.
	
	````
	### Expected behavior 
	### Actual behavior
	### Steps to reproduce the behavior 
	1. N/A
	2. N/A
	3. N/A
	
	* Link to demo site with this issue: N/A
	* Link(s) to source code or any usefull link(s): N/A
	
	### Hexo Information (Paste info from `hexo -v`)
	
	### A-RSnippet Information
	
	**A-RSnippet Version: (Check one with "x)**
	
	[] Latest Master branch.
	[] Latest Release version.
	[] Old version - 
	
	### Other Information (Like Browser, System, Screenshots) 
	
	````
	## 3. Solved
	There are two types of posts here.
	1. Posts are moved from `Ask-For-Help` tag to `Solved` tag
	2. People ask questions in the Discord. After questions are solved, they will create posts here. If you belong to this category, please use the above template to write posts, too.
	
	## 4. Suggest new feature
	Please describe the feature you like in detail. If possible, please provide the link to the websites and source code which contain the feature. Screenshots are also welcomed.
	
	## 5. Resources
	Please make sure the resource is useful to the A-RSnippet Theme Community. The contents can be
	
	* Tutorials to use the A-RSnippet theme
	* Tutorials to use Hexo
	
	## Off-topic
	Say anything you like if you follow the follwing section rules. 
	
	## Post #1 in Welcome to the A-RSnippet Theme Community! | Guideline to post
	
	ABOVE ALL, BE COOL!
	
	We're all here to talk about A-RSnippet theme, and to work together toward making it an even better. Criticizing ideas (by means of reasoned arguments, of course) is an important part of that. But let's not get carried away and devolve into personal attacks, because negativity only gets in the way. We also ask that you avoid the following:
	
	* Offensive or abusive language, as well as any kind of hate speech
	* Posts intended to harass, impersonate, or defame others
	* Unnecessary deletion of posted content
	* Attempts to abuse or expose the private information of others
	* Obscene or sexually explicit content
	* Spam, phishing posts, and any actions intended to deface this site
	* Discussion of software piracy and similar topics
	* All the above are grounds for moderator action. If you have an issue with another member, we ask that you please don't confront them yourself. Please just use the Report command on the post in question, then leave it up to the staff to deal with the situation.
	
	Our moderators may edit or delete any content that is offensive or disruptive to the flow of communication. Serious or repeated offenses may lead to suspension of the offending user's account. So, you know, be cool. 😎
	
	  [1]: https://www.patreon.com/arsnippet
	  [2]: http://arsnippet.yingjiehu.com/tutorial/

## 2018-01-28 Sunday

* Add Internationalization for A-RSnippet theme
   * en
   * cn-Hans
* Create a test post when title is empty
* Delete the website subtitle
* Release [v0.1.1](https://github.com/huyingjie/hexo-theme-A-RSnippet/releases/tag/v0.1.1)

<iframe width="560" height="315" src="https://www.youtube.com/embed/Amy3lj3D-4U" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

You can see how I added the feature on Youtube video.

## 2018-01-30 Tuesday

1. The bug was solved. It was deleted from the [tutorial](http://arsnippet.yingjiehu.com/tutorial/) and  README.md on GitHub.
	
	```
	Existing Bugs
	
	-* list-category-leetcode layout
	
		I used `site.categories.findOne({name: page["search_word"]}).posts.sort('title', 1).each(function(post) {}` to get the posts for a specified categories. There are two bugs that I don't know how to solve.
	
		* You must use `["language", "python"]` format for the `categories` in the front matter. Otherwise, the post does not appear in the list.
		* Hyphen (`-`) cannot be included in the category names.
	
	```
2. Use `sort_by_update` in `_config` file to decide how to sort posts on homepage, by publish date or by update date.

![](2018-01-30-sort-post-by-update-date-on-homepage.png)

