---
layout: page
title: thoughts
permalink: /thoughts/
---

{% assign sorted = site.thoughts | sort: "date" | reverse %}
{% for post in sorted %}
  {% include post-list-item.html post=post tag_base_url="/thoughts/tags/" %}
{% endfor %}