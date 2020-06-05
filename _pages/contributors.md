---
layout: default
title: Longtown Descendants
permalink: /descendants/
comments: false
---

{% for descendant in site.descendants %}
  <h2><a href="{{ descendant.url }}">{{ descendant.name }}</a></h2>
{% endfor %}

