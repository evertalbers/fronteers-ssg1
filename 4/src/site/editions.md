---
layout: layouts/base.njk
title: Editions
---

## Blue <span style="color: blue">Listings</span>

All the editions past and future

### Coming up
<ul>
{% for edition in collections.futureEditions %}
{% set item = edition %}
{% include "edition-details.njk" %}
{% endfor %}
</ul>

### Previously
<ul>
{% for edition in collections.previousEditions | reverse %}
{% set item = edition %}
{% include "edition-details.njk" %}
{% endfor %}
</ul>
