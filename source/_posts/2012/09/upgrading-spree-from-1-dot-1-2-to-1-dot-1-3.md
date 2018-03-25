---
title: "Upgrading Spree from 1.1.2 to 1.1.3"
date: 2012-09-03 17:22
categories: Ecommerce
---

If you upgraded Spree from 1.1.2 to 1.1.3 and found that the checkout didn't work with some error about zones

{% codeblock %}
ActiveRecord::StatementInvalid (PG::Error: ERROR:  column "zone_members_count" does not exist
LINE 1: ...LECT "spree_zones".* FROM "spree_zones"  ORDER BY zone_membe...
                                                             ^
: SELECT "spree_zones".* FROM "spree_zones"  ORDER BY zone_members_count, created_at):
{% endcodeblock %}


Then perhaps you missed that you needed to run some migrations

{% codeblock %}
rake railties:install:migrations
rake db:migrate
{% endcodeblock %}
