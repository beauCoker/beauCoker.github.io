---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020, 2018]
nav: true
---

One day I hope I can describe my publications like [Morbo describes his children](https://youtu.be/c2MEZg1Qol4){:target="\_blank"}. Until then, this is what I have. 

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
