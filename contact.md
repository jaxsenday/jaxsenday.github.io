---
layout: default
title: Contact
permalink: /contact/
---

<div class="section-head">
  <h1>Contact</h1>
</div>

<section class="panel">
  <p><strong>Email:</strong> <a href="mailto:{{ site.data.site.contact.email }}">{{ site.data.site.contact.email }}</a></p>
  {% if site.data.site.contact.office and site.data.site.contact.office != "" %}
    <p><strong>Office:</strong> {{ site.data.site.contact.office }}</p>
  {% endif %}
  {% if site.data.site.contact.office_hours and site.data.site.contact.office_hours != "" %}
    <p><strong>Office hours:</strong> {{ site.data.site.contact.office_hours }}</p>
  {% endif %}
  {{ site.data.site.contact.note | markdownify }}
</section>
