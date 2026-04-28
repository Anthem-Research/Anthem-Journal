---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-grid">
    <div>
      <p class="kicker">Independent art and research practice</p>
      <h1>Anthem Journal</h1>
    </div>
    <div class="intro-panel">
      <p>Anthem studies sovereignty, science, ecology, technology, philosophy, and new forms of living. The journal publishes essays, concepts, project documents, and research notes on how people might build, inhabit, and govern life differently.</p>
      <a class="button" href="/journal/">Read the journal</a>
    </div>
  </div>
</section>

<section class="section">
  <div class="section-header">
    <div>
      <p class="kicker">Recent writing</p>
      <h2>Journal</h2>
    </div>
    <p>Essays and studies from the public surface of Anthem.</p>
  </div>
  <div class="grid">
    {% for post in site.posts limit:3 %}
      {% include post-card.html post=post %}
    {% endfor %}
  </div>
</section>

<section class="section">
  <div class="section-header">
    <div>
      <p class="kicker">Ongoing work</p>
      <h2>Projects</h2>
    </div>
    <p>Live research systems, protocols, software concepts, and applied frameworks.</p>
  </div>
  <div class="grid">
    {% assign featured_projects = site.projects | sort: 'order' %}
    {% for project in featured_projects limit:3 %}
      {% include project-card.html project=project %}
    {% endfor %}
  </div>
</section>

<section class="section">
  <div class="section-header">
    <div>
      <p class="kicker">Private archive</p>
      <h2>Access</h2>
    </div>
    <p>The deeper archive can remain separate from the public journal: private notes, project documents, protocols, and working material.</p>
  </div>
  <a class="button" href="/access/">Access information</a>
</section>
