---
layout: page
title: Team
permalink: /team/
description: Meet our research team
nav: true
nav_order: 3
---

<!-- Team Page -->
<div class="team">
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
      {%- for member in site.team %}
        {%- include team.html member=member %}
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
    </div>
  </div>
</div>
