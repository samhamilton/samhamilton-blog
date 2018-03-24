---
comments: true
date: 2007-10-02 14:32:29
layout: post
slug: getting-redhat-virtualization-up-and-running
title: Getting Redhat Virtualization Up and Running
wordpress_id: 23
categories: Linux
---

So today I started the companies migration to Linux - Redhat EL 5 Linux to be exact from our entirely Microsoft based systems into a 99% Linux run IT system.

Heres the plan:



	
  1. Servers all Redhat

	
  2. Desktops 99% Ubuntu - Accounting needs Windows for internet banking :-(

	
  3. All networking Cisco


Why RHEL5 - well because it offers commercial support of virtualization and great support of HP server hardware out the box. Basically it just needs to work & work properly. I feel that I can get the best of all these with Redhat.

For the desktops Ubuntu simply because its a quick install, minimal software in-fact its almost perfect for a company desktop PC.

So where to start - well first I need to setup one of the Redhat servers with virtualization.

After reading the Fedora wiki and then the first thing to do is copy the install media to the hard drive and share via NFS - I dont like NFS so install I opt for the HTTP installed option and copy everything (excluding CD6) on to my MacBook Pro and setup a web server.

After everything is copied over then time to run the install wizard

on the RedHat machine run the command

virt-install

This starts a very simple and easy to follow wizard that will baby you through the whole installation process.

Reading:

	
  * [NFS Howto](http://tldp.org/HOWTO/NFS-HOWTO/)

	
  * [Fedora Wiki about Xen](http://fedoraproject.org/wiki/FedoraXenQuickstartFC6)


