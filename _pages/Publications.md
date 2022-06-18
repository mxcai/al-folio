---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2018, 2017]
nav: true
---
[GooGle Scholar](https://scholar.google.com/citations?user=bK5JkV4AAAAJ&hl=zh-CN)

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
