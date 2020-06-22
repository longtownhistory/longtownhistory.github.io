---
layout: default
title: Home
permalink: /event
headerimage: https://scontent-ort2-1.xx.fbcdn.net/v/t31.0-8/1622546_610203625726859_1053089703_o.jpg?_nc_cat=110&_nc_sid=e3f864&_nc_ohc=27UWyhLUnBQAX-Oh948&_nc_ht=scontent-ort2-1.xx&oh=e9bc6a448383e3f21da77c9c38baa767&oe=5F14AE31
headerimagecredit: 
headeroverlaycolor: "45, 20, 0" # RGB value
headeroverlaypercent: 0.75 # on a decimal scale of 0 - 1
headerexcerpt: When I went to Palestine [Ohio] in junior high, it was so prejudiced, and then, you know, we’re free here at home. This is home. This is safety. This is free.... No matter where you go, how old you are, when you go home, you’re home. That’s here. That’s Longtown.
headerexcerptcredit: Patricia Hope, Longtown resident
---

An initial contact between one of our academic historians, Jazma Sutton, one of the community partners, Lori Archey (who runs the Facebook page), and [Roane Smothers](https://www.wyso.org/post/longtown-descendants-breathe-new-life-historic-mixed-race-settlement), whose tours of the settlement are a core part of an annual homecoming event, became a series of conversations about the community need to have an easy-to-use centralized platform that anchored a stable archive. We asked permission to participate in the homecoming, working with Brenda Jett, the homecoming organizer. She, in turn, asked permission from the pastor of the church at which the homecoming's main event happens, and from there, Jazma and Lori worked to post event info Longtown/Greenville descendants.

Homecoming events like the one at which the history harvest took place are evidence of how the community sees its past as a source of identity and a guide for future conduct. The oral histories rooted in the built environment itself, in an ancestral home, centered and provided a platform for Black voices. The choice of voice or heirloom--or neither or both--as part of the preservation effort helped acknowledge the silences in archives that depend mostly on physical objects to anchor a community’s history.

Roane provided an oral history of the settlement itself, and you can also see some of the preservation efforts

- Tour will link from here
- Photos of the event will link from here

### The cast of characters

This online archive sits at the intersection of several efforts: an ongoing community self-preservation effort that is centuries in the works, an academic history of black women's voice in historical archives, and a series of history harvests at Indiana University Bloomington. In all of these settings, our consideration of labor practices and its historical inequalities, was central. We acknowledge the importance of the voices that contributed to this archive.

#### The descendants:

{% for oralhistory in site.oralhistories %}
{% if oralhistory.folder == undefined %}
- [{{oralhistory.interviewee}}]({{ oralhistory.url }})
{%endif%}
{% endfor %}
{% for descendant in site.descendants %}
- [{{descendant.title}}]({{ descendant.url }})
{% endfor %}

#### IUB homecoming participants:

- Jazma Sutton
- Chavonté Wright
- Michelle Moyd
- Justin
- Kennedi
- Victoria

#### IUB history-harvest support team:

- Kalani
- Maks
- Lillian
- Matt


### Land acknowledgement

Greenville and Longtown are on the traditional land of the Miami, Shawnee, and Kiikaapoi (Kickapoo) Peoples.