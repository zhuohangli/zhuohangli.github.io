---
layout: default
permalink: /publications/
title: Publications
description:
years: [2024, 2023, 2022, 2021, 2020]
nav: true
nav_title: <i class="fa fa-book"></i> # <i class="far fa-file-alt"></i>
nav_order: 1
---
### Publications
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
