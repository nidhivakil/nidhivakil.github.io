---
layout: publication
permalink: /publications/
title: publications
description: publications
years: [2024,2023, 2022, 2021, 2020]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p>An up-to-date list is available on <a href="https://scholar.google.com/citations?hl=en&user=NIah6CsAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar</a>.</p>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
