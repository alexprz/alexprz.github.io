---
layout: page
permalink: /publications/
title: Publications
description: Manuscripts I got involved into, from latest to oldest.
years: [2022, 2020]
# years: [1956, 1950, 1935, 1905]
nav: true
---

<!-- #### **Under review**
<div class="publications">
  <h2 class="year">Pending</h2>
  {% bibliography -f under_review %}
</div> -->

<div style="height:50px"></div>

#### **Published**
<div class="publications">
  {% for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {% bibliography -f published -q @*[year={{y}}]* %}
  {% else %}
    None yet.
  {% endfor %}
</div>
