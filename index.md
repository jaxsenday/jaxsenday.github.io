---
layout: default
---

<section class="hero">
  <div class="hero-card">
    <div class="eyebrow">{{ site.data.site.profile.title }}</div>
    <h1>{{ site.data.site.profile.name }}</h1>
    <p class="subtitle">{{ site.data.site.profile.institution }}</p>
    {{ site.data.site.profile.biography | markdownify }}

    <nav class="hero-actions" aria-label="Primary actions">
      <a class="button-link button-link--solid" href="{{ '/papers/' | relative_url }}">View publications</a>
      <a class="button-link" href="{{ '/contact/' | relative_url }}">Contact</a>
    </nav>

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

    <section class="panel accent-panel">
      <p class="eyebrow">Current agenda</p>
      <p class="feature-text">Disability, accessibility, and information access across academic and technological systems.</p>
      <p class="meta">Recent work examines academic reading materials, library workflows, visual information, and AI-enabled tools.</p>
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

<section class="section section-band">
  <section class="metric-grid" aria-label="Site overview">
    <article class="metric-card">
      <p class="metric-value">{{ site.data.site.papers | size }}</p>
      <p class="metric-label">Selected publications and presentations</p>
    </article>
    <article class="metric-card">
      <p class="metric-value">{{ site.data.site.talks | size }}</p>
      <p class="metric-label">Recent talks, interviews, and featured appearances</p>
    </article>
    <article class="metric-card">
      <p class="metric-value">{{ site.data.site.activities | size }}</p>
      <p class="metric-label">Major activity areas spanning teaching, service, and research</p>
    </article>
  </section>
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

<section class="section">
  <div class="section-head">
    <h2>White Papers</h2>
    <a href="{{ '/white-papers/' | relative_url }}">View all white papers</a>
  </div>
  <ul class="card-list">
    {% for paper in site.data.site.white_papers limit:2 %}
      <li>
        <h3>{{ paper.title }}</h3>
        <p class="meta">{{ paper.authors }}</p>
        <p>{{ paper.status }} · {{ paper.year }}{% if paper.updated %} · Updated {{ paper.updated }}{% endif %}</p>
        <p>{{ paper.summary }}</p>
        <p><a href="{{ paper.url | relative_url }}">Read the white paper in HTML</a></p>
      </li>
    {% endfor %}
  </ul>
</section>

<section class="section spotlight-grid">
  <section class="panel spotlight-panel">
    <p class="eyebrow">Research themes</p>
    <h2>Designing access into the workflow, not adding it after the fact</h2>
    <p>My work looks at how accessibility is shaped by infrastructure: document formats, library systems, classroom practices, interface design, and the adoption of AI tools in higher education.</p>
    <p>The throughline is practical. I am interested in the points where disabled people lose time, context, or autonomy, and in the design choices that can restore them.</p>
  </section>

  <section class="panel quote-panel">
    <p class="eyebrow">Approach</p>
    <blockquote>
      Accessibility becomes more durable when it is treated as part of everyday information systems rather than as a special-case exception.
    </blockquote>
  </section>
</section>

<section class="section grid two-up">
  <section class="panel">
    <div class="section-head">
      <h2>Recent Talks and Features</h2>
      <a href="{{ '/activities/' | relative_url }}">View all talks and features</a>
    </div>
    <ul class="stack-list">
      {% for talk in site.data.site.talks limit:4 %}
        <li>
          {% if talk.url and talk.url != "" %}
            <a href="{{ talk.url }}"><strong>{{ talk.title }}</strong></a><br>
          {% else %}
            <strong>{{ talk.title }}</strong><br>
          {% endif %}
          {{ talk.event }} · {{ talk.date }}
        </li>
      {% endfor %}
    </ul>
  </section>

  <section class="panel">
    <div class="section-head">
      <h2>Academic Work</h2>
      <a href="{{ '/cv/' | relative_url }}">Review CV and experience</a>
    </div>
    <ul class="stack-list">
      <li><strong>Research</strong><br>Accessibility, disability, visual information, and information access in academic contexts.</li>
      <li><strong>Teaching</strong><br>Experience across informatics, ethics in AI, accessible user experience, and capstone instruction.</li>
      <li><strong>Service</strong><br>Academic committees, invited guest speaking, and accessibility-centered collaboration.</li>
    </ul>
  </section>
</section>
