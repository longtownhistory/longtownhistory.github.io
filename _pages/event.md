---
layout: default
title: Home
permalink: /event
headerimage: https://scontent-ort2-1.xx.fbcdn.net/v/t31.0-8/1622546_610203625726859_1053089703_o.jpg?_nc_cat=110&_nc_sid=e3f864&_nc_ohc=27UWyhLUnBQAX-Oh948&_nc_ht=scontent-ort2-1.xx&oh=e9bc6a448383e3f21da77c9c38baa767&oe=5F14AE31
headerimagecredit: 
headeroverlaycolor: "45, 20, 0" #  This puts an overlay of color onto the photo. The RGB value determines what the overlay color is.
headeroverlaypercent: 0.75 # This determines the opacity of the color overlay, on a decimal scale of 0 - 1 where 1 is completely opaque
headerexcerpt: When I went to Palestine [Ohio] in junior high, it was so prejudiced, and then, you know, we’re free here at home. This is home. This is safety. This is free.... No matter where you go, how old you are, when you go home, you’re home. That’s here. That’s Longtown.
headerexcerptcredit: Patricia Hope, Longtown resident
---

Homecoming events like the one at which the history harvest took place are evidence of how the Longtown/Greenville community sees its past as a source of identity and a guide for future conduct. The oral histories are rooted in the built environment itself, in an ancestral home, which centered and provided a platform for Black voices. The choice of voice or heirloom--or neither or both--as part of the preservation effort helped acknowledge the silences in archives that depend mostly on physical objects to anchor a community’s history.

[Take the tour](/tour): During the tour, Roane Smothers provided an oral history of the settlement itself. You can also see some of the preservation efforts the community is undertaking on site, including a historic marker for the ULI.

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
- Justin Hawkins
- Kennedi Johnson
- Victoria Jones

#### IUB history-harvest support team:

- Kalani Craig
- Maks Szostalo
- Lillian Cox
- Matt Landini


### Land acknowledgement

Greenville and Longtown are on the traditional land of the Miami, Shawnee, and Kiikaapoi (Kickapoo) Peoples.