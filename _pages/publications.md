---
layout: page
permalink: /publications/
title: Publications
description: published peer-reviewed and conference papers.
nav: true
nav_order: 2
---

{% include tg-academic-style.html %}

<div class="tg-page">
  <section class="tg-cv-lead">
    <div class="tg-kicker">Published work</div>
    <p>Published journal articles and conference papers. Under-review manuscripts are intentionally omitted.</p>
    <div class="tg-stat-grid" aria-label="Publication summary">
      <div>
        <span class="tg-stat-value">{{ site.data.publications.peer_reviewed | size }}</span>
        <span class="tg-stat-label">peer-reviewed papers</span>
      </div>
      <div>
        <span class="tg-stat-value">{{ site.data.publications.conference | size }}</span>
        <span class="tg-stat-label">conference papers</span>
      </div>
      <div>
        <span class="tg-stat-value">2025-2026</span>
        <span class="tg-stat-label">publication span</span>
      </div>
    </div>
  </section>

  <section class="tg-section">
    <div class="tg-section-head">
      <h2>Peer-reviewed Papers</h2>
      <p class="tg-section-note">Published journal articles only.</p>
    </div>
    <ol class="tg-publication-list">
      {% for paper in site.data.publications.peer_reviewed %}
        <li class="tg-publication-item">
          <div>
            <p class="tg-publication-title">
              <a href="{{ paper.url }}">{{ paper.title }}</a>
            </p>
            <p class="tg-publication-meta">
              {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}.
            </p>
            {% if paper.doi %}
              <p class="tg-publication-doi">doi: <a href="{{ paper.url }}">{{ paper.doi }}</a></p>
            {% endif %}
          </div>
        </li>
      {% endfor %}
    </ol>
  </section>

  <section class="tg-section">
    <div class="tg-section-head">
      <h2>Conference Papers</h2>
      <p class="tg-section-note">Published abstracts and proceedings.</p>
    </div>
    <ol class="tg-publication-list">
      {% for paper in site.data.publications.conference %}
        <li class="tg-publication-item">
          <div>
            <p class="tg-publication-title">
              <a href="{{ paper.url }}">{{ paper.title }}</a>
            </p>
            <p class="tg-publication-meta">
              {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}{% if paper.abstract_number %}. Abstract {{ paper.abstract_number }}{% endif %}.
            </p>
            {% if paper.doi %}
              <p class="tg-publication-doi">doi: <a href="{{ paper.url }}">{{ paper.doi }}</a></p>
            {% endif %}
          </div>
        </li>
      {% endfor %}
    </ol>
  </section>
</div>
