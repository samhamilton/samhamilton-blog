---
layout: post
title: "Google Analytics Funnel Setup for Spree Commerce"
date: 2012-08-28 15:34
comments: true
categories: 
---

During the setup of any new ecommerce system you will need to monitor your checkout for cart abandonment to find the drop off points and carefully fix them, here is how I setup analytics for Spree Commerce 1.1.x.

* Goal Type: URL Destination
* Goal URL: /orders/R[0-9]{1,8}
* Use funnel: Ticked
* Required Step: Ticked
* Step 1: /checkout
* Step 2: /checkout/delivery
* Step 3: /checkout/payment

{% img /images/spree-funnel.png %}

Thanks to [Ryan](https://groups.google.com/d/topic/spree-user/_gPjQKEwug4/discussion) for the RegEx