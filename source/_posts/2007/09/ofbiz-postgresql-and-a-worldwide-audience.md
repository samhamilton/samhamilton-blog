---
date: 2007-09-19 09:39:31
title: OFBiz, PostgreSQL and a worldwide audience
categories: Work
tags:
- Netsuite
- OfBiz
- Oracle
- PostgreSQL
---

So we were starting to talk to [Netsuite](http://www.netsuite.com) about replacing our systems with theirs, I have to admit I do like the idea of one complete system from one person. It was just before they were going public so they wanted all the business they could muster and we had a "good" price until we got into extra storage space. I mean what does 1GB of storage space cost these days even if you do run [Oracle](http://www.oracle.com) databases like they do to at Netsuite. Well it just made the whole deal crazy the scale out plans made the deal practically blow up and this is with me supporting the integrated system totally and really thinking about the cost savings, it just no longer made sense.

Well fortunate as luck would have it we bumped into someone using OFBiz to run their warehouse here in China. To cut a long story short we then started working out how we could use it including getting me up to speed on Java which is a technology I have never touched. The fun begins we hire our first developer, we think which databases to use and we work out if this thing scales.

The database is an easy choice after a short amount of reading, [PostgreSQL](http://www.postgresql.org) is a clear winner - why? Well really it comes down to data integrity. We are not building a social media site so really we are not going to end up with huge amounts of database writes after all, instead we are going to end up (in a few short years) with TB's of data.

The interesting part of the mix is that we need to have multiple database sites which include USA, UK, Hong Kong and China. The USA, UK and HK sites will be the ecommerce backbones and then also China as we need to ship the goods - the packing stations in the warehouse get PDF files of the address which can be quite large so a local server there keeps the speed and productivity up.

Let me explain why three data centers - first you always have a primary data centre so for us this will be Hong Kong as this is physically closest to Shanghai so for any internal tool this need to be as fast as possible. We build out tools such as [Alfresco](http://www.alfresco.com) and [Clearspace](http://www.jivesoftware.com/products/clearspace) in Hong Kong plus also a copy of OFBiz as all the customer and order information is inside, this node can also provide service to any Asian ecommerce customers.

The US and UK sites are the main points of ecommerce so these sites primary function is to host anything customer facing and provide services using [global load balancing](http://www.cisco.com/warp/public/117/css_glb_sticky.html) to ensure that each customer is getting just about the fastest response from our servers.

Having customers in 9+ primary and 50+ secondary countries really makes delivering a great experience to them all hard.

Thats all for now - lets see how this gets on.
