---
layout: default
title: CV
permalink: /cv/
---

<div class="section-head">
  <h1>Curriculum Vitae</h1>
</div>

<section class="panel">
  <p>A downloadable CV will be posted here once the current version is ready for publication.</p>
</section>

<section class="section grid two-up">
  <section class="panel">
    <h2>Research Interests</h2>
    <ul class="stack-list">
      {% for item in site.data.site.research_interests %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </section>

  <section class="panel">
    <h2>Professional Snapshot</h2>
    <p>{{ site.data.site.profile.title }}</p>
    <p>{{ site.data.site.profile.institution }}</p>
    <p>{{ site.data.site.profile.location }}</p>
  </section>
</section>
