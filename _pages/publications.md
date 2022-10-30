---
layout: page
permalink: /publications/
title: publications
description: <b>*</b> denotes equal contribution and joint lead authorship
years: [2022, 2021, 2020, 2019, 2018, 2017, 2015]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
