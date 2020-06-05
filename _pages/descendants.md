---
layout: page
title: Longtown Descendants
comments: false
permalink: /descendants/
---

{% for descendant in site.descendants %}
  <h2><a href="{{ descendant.url }}">{{ descendant.title }}</a></h2>
{% endfor %}
