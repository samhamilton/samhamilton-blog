---
layout: post
title: "Non-www to www nginx redirect"
date: 2012-08-24 14:36
comments: true
categories: Linux
---
Add this small block of code into your server{} block to redirect all non-www to the www version of your website.

	{% codeblock %}
if ($host != 'www.samhamilton.co.uk' ) {
	rewrite  ^/(.*)$  http://www.samhamilton.co.uk/$1  permanent;
 }
 {% endcodeblock %}
