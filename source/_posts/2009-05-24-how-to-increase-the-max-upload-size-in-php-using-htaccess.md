---
comments: true
date: 2009-05-24 11:13:53
layout: post
slug: how-to-increase-the-max-upload-size-in-php-using-htaccess
title: How to increase the max upload size in php using .htaccess
wordpress_id: 186
categories: Linux
---

So if you are like me using [Mosso](http://www.mosso.com) and cant edit the php.ini file then if you want to increase the default upload size you need to edit your .htaccess file and add the following (adjust as needed):

    {% codeblock %}
    php_value post_max_size 16M
    php_value upload_max_filesize 16M
    php_value max_execution_time 600
    {% endcodeblock %}
