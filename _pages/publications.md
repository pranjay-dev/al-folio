---
layout: page
permalink: /publications/
title: Publications
description: Publications in reverse chronological order </br> * denotes equal contribution # by categories </br>
years: [2022, 2021, 2020]
nav: true
sort: 3
---

<div class="publications">
<!-- * denotes equal contribution -->
<!-- <h1> preprints </h1> -->

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
