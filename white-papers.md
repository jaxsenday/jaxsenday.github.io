---
layout: default
title: White Papers
permalink: /white-papers/
description: "Practice-based white papers by Jaxsen R. Day on accessibility, AI-supported work, and information systems."
---

<div class="section-head">
  <h1>White Papers</h1>
</div>

<p class="page-intro">This section shares extended, practice-based papers that develop ideas, methods, and frameworks outside the format of a journal article. Each paper is available as structured HTML for easier navigation, reflow, and screen reader access.</p>

<ul class="card-list">
  {% for paper in site.data.site.white_papers %}
    <li>
      <h2>{{ paper.title }}</h2>
      <p class="meta">{{ paper.authors }}</p>
      <p>{{ paper.status }} · {{ paper.year }}{% if paper.updated %} · Updated {{ paper.updated }}{% endif %}</p>
      <p>{{ paper.summary }}</p>
      <p><a href="{{ paper.url | relative_url }}">Read {{ paper.title }} in HTML</a></p>
    </li>
  {% endfor %}
</ul>
