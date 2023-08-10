---
layout: page
title: teaching
permalink: /teaching/
description: 
nav: true
nav_order: 3
display_categories:
horizontal: true
---

<!-- pages/teaching.md -->
<div class="teachings">
{%- if site.enable_teaching_categories and page.display_categories %}
  <!-- Display categorized teachings -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_teachings = site.teachings | where: "category", category -%}
  {%- assign sorted_teachings = categorized_teachings | sort: "importance" %}
  <!-- Generate cards for each teaching -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for teaching in sorted_teachings -%}
      {% include teachings_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for teaching in sorted_teachings -%}
      {% include teachings.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display teachings without categories -->
  {%- assign sorted_teachings = site.teachings | sort: "importance" -%}
  <!-- Generate cards for each teaching -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for teaching in sorted_teachings -%}
      {% include teachings_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for teaching in sorted_teachings -%}
      {% include teachings.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
