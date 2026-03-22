---
layout: default
---

<section class="hero">
  <div class="hero-card">
    <div class="eyebrow">{{ site.data.site.profile.title }}</div>
    <h1>{{ site.data.site.profile.name }}</h1>
    <p class="subtitle">{{ site.data.site.profile.institution }}</p>
    {{ site.data.site.profile.biography | markdownify }}

    <ul class="pill-list" aria-label="Research interests">
      {% for item in site.data.site.research_interests %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </div>

  <aside class="hero-aside">
    <section class="panel">
      <img class="profile-photo" src="{{ site.data.site.profile.photo | relative_url }}" alt="Portrait of {{ site.data.site.profile.name }}">
      <p class="meta">{{ site.data.site.profile.location }}</p>
    </section>

    <section class="panel">
      <h2>Links</h2>
      <ul class="link-list">
        {% for link in site.data.site.links %}
          {% if link.url and link.url != "" %}
            <li><a href="{{ link.url }}">{{ link.label }}</a></li>
          {% endif %}
        {% endfor %}
      </ul>
    </section>
  </aside>
</section>

<section class="section">
  <div class="section-head">
    <h2>Publications and Presentations</h2>
    <a href="{{ '/papers/' | relative_url }}">View all publications and presentations</a>
  </div>
  <ul class="card-list">
    {% for paper in site.data.site.papers limit:3 %}
      <li>
        <h3>{{ paper.title }}</h3>
        <p class="meta">{{ paper.authors }}</p>
        <p>{{ paper.venue }} · {{ paper.year }}{% if paper.status %} · {{ paper.status }}{% endif %}</p>
        <p>{{ paper.summary }}</p>
        {% if paper.url and paper.url != "" %}
          <p><a href="{{ paper.url }}">Paper link</a></p>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
</section>

<section class="section grid two-up">
  <section class="panel">
    <div class="section-head">
      <h2>Recent Talks</h2>
      <a href="{{ '/activities/' | relative_url }}">View all academic activities</a>
    </div>
    <ul class="stack-list">
      {% for talk in site.data.site.talks limit:4 %}
        <li>
          <strong>{{ talk.title }}</strong><br>
          {{ talk.event }} · {{ talk.date }}
        </li>
      {% endfor %}
    </ul>
  </section>

  <section class="panel">
    <div class="section-head">
      <h2>Current Focus</h2>
      <a href="{{ '/activities/' | relative_url }}">Review academic activities</a>
    </div>
    <p>My current work focuses on disability, accessibility, and information access across academic and technological settings.</p>
  </section>
</section>
