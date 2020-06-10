---
layout: page
title: Longtown Descendants
comments: false
permalink: /descendants/
---

<h2>Oral Histories</h2><ul>
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

<h2>Descendants' Historical Collections</h2>
<div class="row listrecent"> 
{% for descendant in site.descendants %}
<div class="col-lg-4 col-md-6 mb-30px card-group">
    <div class="card">
        <div class="maxthumb">
            <a href="{{ descendant.url }}">
						<img class="img-fluid" src="{{ site.baseurl }}/assets/collections/{{ descendant.folder}}/{{descendant.mainitem}}_th.jpg" alt="{{ descendant.title }}">
            </a>
        </div>
        <div class="card-body">
            <h2 class="card-title">
                <a href="{{ descendant.url }}">{{ descendant.title }}</a>
            </h2>
                <h4 class="card-text">View items from the collection of <a href="{{ descendant.url }}">{{ descendant.title }}</a></h4>            
        </div>
        <div class="card-footer bg-white">
            <div class="wrapfooter">
                <span class="author-meta">
                </span>
                <div class="clearfix"></div>
            </div>
        </div>
    </div>
</div>
<!-- end post -->

{% endfor %}
</div>    
