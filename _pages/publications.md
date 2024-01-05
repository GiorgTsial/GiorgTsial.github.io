---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2023, 2022, 2021, 2020]
---
<!-- _pages/publications.md -->
<!-- <div class="publications"> -->

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
