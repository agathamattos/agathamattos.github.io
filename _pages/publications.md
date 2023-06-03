---
layout: page
permalink: /publications/
title: publications
description: Please see my <a href='https://scholar.google.com/citations?user=WQky650AAAAJ'>Google Scholar</a> for an up-to-date list of publications.
years: [2022, 2021, 2020]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
