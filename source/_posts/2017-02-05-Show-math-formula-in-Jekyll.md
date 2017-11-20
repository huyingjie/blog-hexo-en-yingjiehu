---
layout: post
title:  "How to show math formula in Jekyll"
date:   2017-02-05
tags: [Jekyll]
categories: [Mix]
permalink: Show-math-formula-in-Jekyll
---

There are only two steps to add functionality of showing math formular in Jekyll. MathJax is the engine to achive it. <!-- more -->

1. open the file `default.html` in the folder `_layouts`
2. add the following codes before `</head>


	```js
	  <script type="text/x-mathjax-config">
	  MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
	  </script>
	  <script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
	  <link href="/assets/css/syntax.css" rel="stylesheet" >
	```

## Test:

Add the following codes to your posts to test whether MathJax is working.

### 1. the **inline** mode

	**Code:**

	```latex
	In physics, the mass-energy equivalence is stated
by the equation $E=mc^2$, discovered in 1905 by Albert Einstein.
	```

	**Desired result:**

	In physics, the mass-energy equivalence is stated
by the equation $E=mc^2$, discovered in 1905 by Albert Einstein.

### 2. the **display** mode

	**Code:**

	```latex
	The mass-energy equivalence is described by the famous equation

	$$E=mc^2$$

	discovered in 1905 by Albert Einstein.
	In natural units ($c$ = 1), the formula expresses the identity

	\begin{equation}
	E=m
	\end{equation}
	```
	**Desired result:**

	The mass-energy equivalence is described by the famous equation

	$$E=mc^2$$

	discovered in 1905 by Albert Einstein.
	In natural units ($c$ = 1), the formula expresses the identity

	\begin{equation}
	E=m
	\end{equation}
