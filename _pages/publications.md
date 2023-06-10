---
layout: page
permalink: /publications/
title: publications
years_conf: [2021, 2020]
years_journal: [2022]
years_workshop: [2020]
nav: true
nav_order: 1
---

### Journal Articles
<div class="publications">

{%- for y in page.years_journal %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography2 }} -q @*[year={{y}}]* %}
{% endfor %}

</div>

### Conference Proceedings
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years_conf %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>

### Workshop Publications
<div class="publications">

{%- for y in page.years_workshop %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography3 }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
