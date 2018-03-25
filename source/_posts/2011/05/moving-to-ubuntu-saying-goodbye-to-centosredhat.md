---
date: 2011-05-31 14:51:38
title: Moving to Ubuntu, Saying goodbye to CentOS/Redhat
categories: Linux
---

I have been a fan of Redhat for a very long time I bought my first copy of Redhat back in 1997 - it was in a boxset, I kept it for years even after I upgraded! Redhat has been stable and reliable (well ok, most of the time) - just what you need for a server distribution but this month marks the first time I cheat on Redhat by installing a copy of Ubuntu on one of my production servers.

In the beginning when I first had company production machines we also used Redhat because a couple of hundred dollars a year for support for one box seemed reasonable. Then as less and less things broke and we as sysadmins grew and learned what was needed to fix things that couple hundred dollars seems more and more expensive. Our collection of servers grew and we started switching over to CentOS as the support contracts ran out.  At the same time we also became a customer of Rackspace and we used Redhat 5 on the servers because well it was "free" with each server and it complimented the existing Redhat/CentOS we had in the office.

We were happy with our lot - things were at peace, CentOS boxes got point upgrades fairly quickly but it never really mattered too much they were not facing the outside world or targets of external hacks.

After leaving my last company I started out with my own hardware which I bought and put into a datacenter in the UK. I stuck CentOS on it and things again were all good. Then Redhat released 5.6 and CentOS started working on the upgrade and they kept working and working and working. Then Redhat started patching security holes but still no upgrade came from CentOS.

For a long time using CentOS was a pleasure but now after sitting with a bunch of unpatched servers that were targets of hacking attempts for several months while they work out the upgrade process to 5.6 left me with a very bitter taste in my mouth. While I totally understand that they cant change the OS they are building, that defeats the point of binary compatibility with Redhat, the amount of time that it took to get a dot point release upgrade was just too long. Think about how many web hosting companies were sitting there with unpatched servers waiting for the upgrade - scary!

I toyed with the idea of moving to Fedora but they dont officially support a yum version upgrade route and physically upgrading all the physical machines from media is crazy, so instead Ubuntu jumped to my mind. Its has been on the up for the last few years and more projects seem to be using it as a starting point for releasing software.

Ubuntu ticks all the right boxes, it has a free server version, apt based version upgrades and paid support if I ever really need it. I have had the server now online for 2 weeks and things have been rather smooth, everything works as expected. Some config files are in a different location but thats no biggie and the system is getting regular security updates.

The only negative I have with Ubuntu is that PostgreSQL 9 is not in the default distribution even though they have had it out for a couple of Ubuntu releases now, but if that is all I have to gripe about then things are defiantly ok.

Somehow I think CentOS is going to keep having an uphill battle to keep up with Redhat who seem intent to try and disrupt other companies making a buck off their software like Oracle and even though they have the best of intentions I now don't think that CentOS is the distro of choice for a internet facing server, sad times.
