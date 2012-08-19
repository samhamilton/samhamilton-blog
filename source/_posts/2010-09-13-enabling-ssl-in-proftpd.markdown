---
comments: true
date: 2010-09-13 21:27:07
layout: post
slug: enabling-ssl-in-proftpd
title: Enabling SSL in ProFTPD
wordpress_id: 459
categories:
- Linux / Apple
---

If you need to enable SSL in ProFTPD, try this out:

{% codeblock %}
<IfModule mod_tls.c>
TLSEngine on
TLSRequired off
TLSRSACertificateFile /etc/httpd/conf/ssl.crt/server.crt
TLSRSACertificateKeyFile /etc/httpd/conf/ssl.key/server.key
TLSVerifyClient off
</IfModule>
{% endcodeblock %}
