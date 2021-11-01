---
layout: page
permalink: /publications/
title: Publications
description: Please, visit my 
<!-- <A HREF="https://scholar.google.com/citations?user=pDLXZy0AAAAJ&hl=en"> Google Scholar</A> page to see the full list. -->
years: [2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>


<!-- <a href="https://scholar.google.com/citations?user=pDLXZy0AAAAJ&hl=en" target="_top">Google Scholar</a>  -->