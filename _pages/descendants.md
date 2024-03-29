---
layout: page
title: Longtown Descendants
comments: false
permalink: /descendants/
---


> "By memory, those fond associations and ties of love which unite us together on earth, will be preserved in eternity...Memory should be cultivated. Like all other faculties of the mind and body, its vigor and activity depend on its exercise. The more the memory is exercised the stronger it becomes." -J. B. Harrison, Greenville Settlement, 1864

<div class="row">
<div class="col-s-12 col-md-8">
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
                <p style="line-height:1.1em;">View items from the collection of <a href="{{ descendant.url }}">{{ descendant.title }}</a></p>            
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

</div>
<div class="col-s-6 col-md-4">
<h2>The voices of Greenville and Longtown</h2><ul>
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
</DIV>
