---
layout: page
permalink: /publications/
title: Publications
description: Peer-reviewed publications. (* = equal contribution)
years: [2024, 2023, 2022, 2021, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h2 class="year">Ph.D. Thesis</h2>
{% bibliography -f papers -q @*[booktitle=Ph.D. Thesis]* %}

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
