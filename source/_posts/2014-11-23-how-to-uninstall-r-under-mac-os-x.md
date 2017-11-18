---
layout: post
title:  "How to Uninstall R underMac OS X"
date: 2014-11-23
tags: [R]
categories: [Programming Language, R]
permalink: how-to-uninstall-r-under-mac-os-x
---

When updating R on Mac,  we can uninstall the old version and install the new version. Uninstalling R is very easy on Mac. <!-- more -->

During installation of R,  at least 2 folders are involved.
<ol>
	<li><code>/Applications/R.app</code> folder: contains GUI</li>
	<li> <code><span class="lang:r decode:true crayon-inline">/Library/Frameworks/R.framework</span></code> folder: contains R framework</li>
	<li> <code>(unkown) <span class="lang:default decode:true crayon-inline ">/usr/bin</span></code> : contains some links</li>
</ol>
When uninstalling, R under Mac OS X will delete all of them.

Uninstallation steps as follows:
<ol>
	<li>open terminal in Mac OS X</li>
	<li>run <code>rm -rf /Library/Frameworks/R.framework /Applications/R.app \ /usr/bin/R /usr/bin/Rscript</code></li>
</ol>
Done!

Reference: <http://cran.r-project.org/doc/manuals/r-release/R-admin.html#Uninstalling-under-OS-X>
