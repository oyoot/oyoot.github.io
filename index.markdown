---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: notes
permalink: /
---

{% assign sorted = site.notes | sort: "date" | reverse %}
{% for post in sorted %}
  {% include post-list-item.html post=post tag_base_url="/notes/tags/" %}
{% endfor %}
