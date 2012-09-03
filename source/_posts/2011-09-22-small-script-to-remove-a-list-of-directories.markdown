---
comments: true
date: 2011-09-22 20:13:38
layout: post
slug: small-script-to-remove-a-list-of-directories
title: Small Script to Remove a List of Directories
wordpress_id: 564
categories: Linux
---

{% codeblock %}
cat list-of-directories.txt|while read f; do
if [ -e "$f" ]; then rm -rf "$f"; fi; done```
{% endcodeblock %}

thanks [unSpawn](http://www.linuxquestions.org/questions/programming-9/scripting-problem-rm-filelist-460910/#post2320128)! 
