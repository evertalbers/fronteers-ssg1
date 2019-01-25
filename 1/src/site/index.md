---
layout: layouts/base.njk
title: My meetup is amazing
---


## A small step for a man, a large chunk of the space budget

Yes it is. Look at the different editions!


## Editions
<ul>
{% for edition in collections.editions | reverse %}
{% set item = edition %}
{% include "edition-details.njk" %}
{% endfor %}
</ul>


## Subscribe

Never miss out. You can subscribe to an [RSS feed](/feed.xml) of the meetups.
