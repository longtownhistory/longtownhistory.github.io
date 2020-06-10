---
layout: page
title: Oral Histories
comments: false
permalink: /oralhistories/
---

<div class="row listrecent"> 
<ul>
{% for oralhistory in site.oralhistories %}
{% if oralhistory.folder == undefined %}
	{% assign interviewee = oralhistory.interviewee %}
{% else %}
	{% assign contributor = site.descendants | where: "folder", oralhistory.folder  | first %}
	{% assign interviewee = contributor.title%}	
{% endif %}
<li><a href="{{ oralhistory.url }}">{{interviewee}}</a></li>
{% endfor %}
</ul>
</div>    
