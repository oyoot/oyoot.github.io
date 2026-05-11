---
layout: page
title: notes
permalink: /notes/
---

{% assign sorted = site.notes | sort: "date" | reverse %}
{% for post in sorted %}
  {% include post-list-item.html post=post tag_base_url="/notes/tags/" %}
{% endfor %}