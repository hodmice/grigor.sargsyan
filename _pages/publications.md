---
layout: page
permalink: /publications/
title: publications
description: 
years: [2025,2024,2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2010, 2009, 2008, 2007, 2006, 2005, 2004]
nav: true
nav_order: 0
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  
  {% bibliography -f  {{ site.scholar.bibliography }}  -q @*[year={{y}}]* %} {% endfor %}


</div>



