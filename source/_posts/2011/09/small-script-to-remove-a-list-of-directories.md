---
date: 2011-09-22 20:13:38
title: Small Script to Remove a List of Directories
categories: Linux
---

{% codeblock %}
cat list-of-directories.txt|while read f; do
if [ -e "$f" ]; then rm -rf "$f"; fi; done```
{% endcodeblock %}

thanks [unSpawn](http://www.linuxquestions.org/questions/programming-9/scripting-problem-rm-filelist-460910/#post2320128)!
