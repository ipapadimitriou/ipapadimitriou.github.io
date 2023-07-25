---
layout: page
title: teaching
permalink: /teaching/
description: 
nav: true
nav_order: 4
display_categories: [graduate, undergraduate]
horizontal: false
---

<!-- pages/teaching.md -->

## <a style="pointer-events: none; display: inline-block;" href="#">courses</a>

<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.teaching | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.teaching | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>

&nbsp;

## <a style="pointer-events: none; display: inline-block;" href="#">students</a>

> ### PhD
> [Ok Song An](https://inspirehep.net/authors/1422132) (2015 -- 2017)


> ### MSci
> [Gerassimos Kouniatalis](#) (2023 -- 2024) 
> [Vassilis Voulgaris](#) (2023 -- 2024) 
> [Georgios Korpas](https://inspirehep.net/authors/1614033) (2013 -- 2014)


> ### Undergraduate
> [Antonios Stefas](#) (2022 -- 2023) 


