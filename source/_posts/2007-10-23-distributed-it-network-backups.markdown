---
comments: true
date: 2007-10-23 22:07:13
layout: post
slug: distributed-it-network-backups
title: Distributed IT Network Backups?
wordpress_id: 26
categories:
- Work
tags:
- backups
- rackspace
- rsync
---

I am currently building the foundation of my companies new IT network, its looking very open source heavy, very cisco based and also very distributed. Think five sites and only little old me to do most of the "heavy lifting".

I have a great second but sometimes we need time off - thats fine and good but what happens to our backups? Well at the moment there really is only one server of any importance that we need to backup & so I gave this job (mainly becuase the server is in his office) to my assistant. Well what happens when he goes on holiday and the worst of the worst comes I cant get to the site to change tapes?

Well becuase its a one tape backup - the backup just keeps on writing to the same tape - backuped ok, good course not!

We use Rackspace for our customer facing servers & so I keep tabs on them. Their CTO of webmail.us recently [blogged](http://billboebel.typepad.com/blog/2007/10/amazons-larger-.html) that they use [Amazon's EC2](http://www.amazon.com/b/ref=sc_fe_c_0_370375011_1/104-7582466-3819946?ie=UTF8&node=201590011&no=370375011&me=A36L942TSJ2AJA) for backup & it got me thinking. Thats quite a nice solution for me too - all the backups of various things in all the various offices can all just backup straight to EC2.

Um.. going to chew on that for a while
