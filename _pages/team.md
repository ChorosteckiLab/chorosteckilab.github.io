---
layout: page
title: Team
permalink: /team/
description: Meet our research team
nav: true
nav_order: 3
---

<!-- Team Page -->
{%- for member in site.team %}
  <div class="col">
    <div class="card h-100 shadow-sm">
      <img src="{{ member.img | prepend: site.baseurl }}" class="card-img-top" alt="{{ member.name }}">
      <div class="card-body">
        <h5 class="card-title">{{ member.name }}</h5>
        <p class="card-text"><b>Position:</b> {{ member.position }}</p>
        <p class="card-text">{{ member.bio }}</p>
      </div>
    </div>
  </div>
{%- endfor %}
