---
layout: page
permalink: /publications/
title: Publications
description: Please, visit my <a href="https://scholar.google.com/citations?user=OUct8qMAAAAJ&hl=en&oi=ao" >[Google Scholar]</a> page to see the full list.
years: [2022, 2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
