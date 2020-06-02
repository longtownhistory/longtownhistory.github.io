---
layout: default
title: History Harvest Artifacts
permalink: /contributors/index.html
comments: false
---

<ul>
{% assign typesort = site.data.contributors | sort: 'type' %}
{% for contributor in typesort %}
  <li>
    {{ contributor.name }} stored in {{ contributor.name }}
  </li>
{% endfor %}
</ul>
