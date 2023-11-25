---
layout: page
permalink: /publications/
title: publications
description: >
  <p>* Equal Contribution<br>
  † Corresponding Author</p>
years: [2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{% for y in page.years %}
  <div class="col-sm-1 align-self-end mt-2 p-0 pr-1">
      <h2 class="bibliography-year">{{y}}</h2>
  </div>
  <div class="row m-0 p-0" style="border-bottom: 1px solid #ddd;">
    <div class="col-sm-11 p-0">
      {% bibliography -f papers -q @*[year={{y}}]* %}
    </div>
  </div>
{% endfor %}


[//]: # ({% bibliography -f {{ site.scholar.bibliography }} %})

</div>
