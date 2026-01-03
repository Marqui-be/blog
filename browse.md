---
layout: default
title: Browse
---

<div class="hero hero-small">
  <div class="hero-kicker">Library</div>
  <h1>Browse notes</h1>
  <p class="hero-lead">Everything published on logs.marqui.org, grouped by section.</p>
</div>

<div class="section">
  <div class="section-head">
    <h2>Meta</h2>
    <p>How we think, write, and build the engine.</p>
  </div>

  <div class="listcard">
  {% for page in site.pages %}
    {% if page.path contains "notes/meta/" and page.title %}
      <a class="row" href="{{ page.url }}">
        <span class="row-title">{{ page.title }}</span>
        <span class="row-meta">Meta</span>
      </a>
    {% endif %}
  {% endfor %}
  </div>
</div>

<div class="section">
  <div class="section-head">
    <h2>Systems</h2>
    <p>Models, workflows, and tools that remove human load.</p>
  </div>

  <div class="listcard">
  {% for page in site.pages %}
    {% if page.path contains "notes/systems/" and page.title %}
      <a class="row" href="{{ page.url }}">
        <span class="row-title">{{ page.title }}</span>
        <span class="row-meta">Systems</span>
      </a>
    {% endif %}
  {% endfor %}
  </div>
</div>

<div class="section">
  <div class="section-head">
    <h2>2026</h2>
    <p>The public experiment. Logs from a real company run with AI systems.</p>
  </div>

  <div class="listcard">
  {% for page in site.pages %}
    {% if page.path contains "notes/2026/" and page.title %}
      <a class="row" href="{{ page.url }}">
        <span class="row-title">{{ page.title }}</span>
        <span class="row-meta">2026</span>
      </a>
    {% endif %}
  {% endfor %}
  </div>
</div>
