---
layout: post
title:  "Add disqus comment system in Jekyll"
date:   2017-02-06
tags: [Jekyll]
categories: [Mix]
---

The following steps are to add disqus comment system in all posts. It requires global setting in the `_config.yml` file. In comparison, the official disqus tutorial adds front matter to each post to indicate whether comments are shown or not. <!-- more -->

1. Add following codes to the `_config.yml` file:

	```
	# Disqus settings
	disqus_username: DISQUSNAME
	layout: default
	comments: true
	```

2. Click the  `Universal Embeded Code` text in the `Jekyll install instructions` page in disqus website.

3. Copy codes in the first step on the page.
4. Open and edit `post.html` below the `_layouts` folder.
5. Find the place where you will put comments.
6. Paste codes from Step 3.
