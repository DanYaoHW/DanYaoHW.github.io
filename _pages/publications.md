---
layout: page
title: titles.publications
description: descriptions.publications
permalink: /publications/
years: [2023,2022,2021,2020,2019,2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
