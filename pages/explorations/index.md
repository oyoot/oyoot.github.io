---
layout: page
title: explorations
permalink: /explorations/
---

{% assign sorted = site.explorations | sort: "date" | reverse %}
{% for post in sorted %}
  {% include post-list-item.html post=post tag_base_url="/explorations/tags/" %}
{% endfor %}
