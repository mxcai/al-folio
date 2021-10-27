---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020, 2018, 2017]
nav: true
---
[GooGle Scholar](https://scholar.google.com/citations?user=8RH6-hkAAAAJ&hl=zh-CN)

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
