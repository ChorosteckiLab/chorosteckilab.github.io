---
layout: page
title: Resources and tools
permalink: /resources/
description: Web-based software resources of value to the biological community 
nav: true
nav_order: 4
display_categories: [Palatnik, Gabaldon]
horizontal: false
---

<!-- pages/resources.md -->
<div class="projects">
{%- if site.enable_resource_categories and page.display_categories %}
  <!-- Display categorized resources -->
  {%- for category in page.display_categories %}
  
  <!-- Ommit category title -->
  <h2 class="category">{{ category }}</h2>

  {%- assign categorized_resources = site.resources | where: "category", category -%}
  {%- assign sorted_resources = categorized_resources | sort: "importance" %}
  <!-- Generate cards for each resource -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for resource in sorted_resources -%}
      {% include resources_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for resource in sorted_resources -%}
      {% include resources.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display resources without categories -->
  {%- assign sorted_resources = site.resources | sort: "importance" -%}
  <!-- Generate cards for each resource -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for resource in sorted_resources -%}
      {% include resources_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for resource in sorted_resources -%}
      {% include resources.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>
