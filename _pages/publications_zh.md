---
layout: page
permalink: /zh/publications/
title: 论文
lang: zh
description:
years: [2026, 2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018]
nav: true
nav_order: 1
---

<div class="publications">

<p style="font-family: Times; font-size: 1rem; margin-bottom: 1.5rem; font-weight: bold;">
  如需查看更新的论文信息，请访问我的
  <a href="https://scholar.google.com/citations?user=SQl1XCUAAAAJ&hl=en&oi=ao" target="_blank" style="text-decoration: underline;">
    Google Scholar
  </a>。
</p>

<h2><span class="font-weight-bold">Papers</span></h2>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
