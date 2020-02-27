---
layout: page
permalink: /publications/:path/
title: publications
description: My academic contributions: papers, posters, talks, acheivements.
years: [2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
