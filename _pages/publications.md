---
layout: page
permalink: /publications/
title: publications
description: Please reach the full list of publications at this <a href=https://scholar.google.ca/citations?hl=en&user=1HJ-KYMAAAAJ&view_op=list_works&sortby=pubdate target=_blank><u>Google Scholar Profile</u></a>
years: [2022, 2021, 2020, 2019]
nav: true
nav_order: 5
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
