---
layout: default
title: Papers
permalink: /papers/
---

<div class="section-head">
  <h1>Papers</h1>
</div>

<ul class="card-list">
  {% for paper in site.data.site.papers %}
    <li>
      <h2>{{ paper.title }}</h2>
      <p class="meta">{{ paper.authors }}</p>
      <p>{{ paper.venue }} · {{ paper.year }}{% if paper.status %} · {{ paper.status }}{% endif %}</p>
      <p>{{ paper.summary }}</p>
      {% if paper.url and paper.url != "" %}
        <p><a href="{{ paper.url }}">View paper</a></p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
