---
layout: default
title: Home
permalink: /tour
---

<div class="row listrecent"> 
{% for static_file in site.static_files %}
{% if static_file.path contains "tour" %}

<div class="col-lg-4 col-md-6 mb-30px card-group">
    <div class="card">
        <div class="maxthumb">
            <!--<a href="{{ site.baseurl }}{{ item.url }}">-->
						<img src="{{ site.baseurl }}{{ static_file.path }}" alt="{{ page.title }}">
            <!--</a>-->
        </div>
    </div>
</div>

{%endif%}
{% endfor %}
</div>
