---
title: "Getting RVM"
date: 2013-01-24 17:19
categories: Ruby
---

I'm not sure where to put this, but I wanted to share this tidbit of info.

I was having an issue where I would see all these hanging /bin/bash processes calling runner and rake that were being fired off by cron. Turns out my .rvmrc file in my app folder was causing the problem. Rvm by default will prompt to trust or not trust the file. This causes bash to hang. The solution I used was to disable the prompt by adding this line to my user rvm file in ~/.rvmrc

``rvm_trust_rvmrcs_flag=1``

Have a read of the [RVM Wiki](https://github.com/javan/whenever/wiki/RVM-Notes)
