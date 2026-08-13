---
layout: default
title: Joshua Hia
---

# Joshua Hia — Data Science Portfolio

*One-line intro about yourself — edit this in index.md.*

{% assign sorted_writeups = site.writeups | sort: "order" %}
{% for writeup in sorted_writeups %}
## [{{ writeup.title }}]({{ writeup.url | relative_url }})

{{ writeup.summary }}

{% if writeup.image %}
![]({{ writeup.image | relative_url }})
{% endif %}

{% endfor %}
