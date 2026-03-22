---
layout: default
title: Activities
permalink: /activities/
---

<div class="section-head">
  <h1>Activities</h1>
</div>

<section class="section">
  <h2>Talks and Presentations</h2>
  <ul class="timeline">
    {% for talk in site.data.site.talks %}
      <li>
        <h3>{{ talk.title }}</h3>
        <p>{{ talk.event }} · {{ talk.location }} · {{ talk.date }}</p>
        {% if talk.notes %}<p>{{ talk.notes }}</p>{% endif %}
        {% if talk.url and talk.url != "" %}
          <p><a href="{{ talk.url }}">Event link</a></p>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</section>

{% for block in site.data.site.activities %}
  <section class="section">
    <h2>{{ block.category }}</h2>
    <ul class="card-list">
      {% for item in block.items %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </section>
{% endfor %}
