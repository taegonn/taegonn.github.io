---
layout: page
permalink: /publications/
title: Publications
description: published peer-reviewed and conference papers.
nav: true
nav_order: 2
---

<style>
  .tg-publication-section {
    margin-top: 1.75rem;
  }

  .tg-publication-section:first-of-type {
    margin-top: 0.75rem;
  }

  .tg-publication-note {
    color: var(--global-text-color-light, #6b7280);
    font-size: 0.95rem;
    margin-bottom: 1rem;
  }

  .tg-publication-list {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .tg-publication-item {
    border-top: 1px solid var(--global-divider-color, #e5e7eb);
    padding: 1rem 0;
  }

  .tg-publication-item:last-child {
    border-bottom: 1px solid var(--global-divider-color, #e5e7eb);
  }

  .tg-publication-title {
    font-size: 1rem;
    font-weight: 600;
    line-height: 1.35;
    margin: 0 0 0.35rem;
  }

  .tg-publication-meta,
  .tg-publication-doi {
    color: var(--global-text-color-light, #6b7280);
    font-size: 0.92rem;
    line-height: 1.45;
    margin: 0;
  }

  .tg-publication-doi {
    margin-top: 0.2rem;
  }
</style>

<section class="tg-publication-section">
  <h2>Peer-reviewed Papers</h2>
  <p class="tg-publication-note">Published journal articles only; under-review manuscripts are not listed here.</p>
  <ol class="tg-publication-list">
    {% for paper in site.data.publications.peer_reviewed %}
      <li class="tg-publication-item">
        <p class="tg-publication-title">
          <a href="{{ paper.url }}">{{ paper.title }}</a>
        </p>
        <p class="tg-publication-meta">
          {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}.
        </p>
        {% if paper.doi %}
          <p class="tg-publication-doi">doi: <a href="{{ paper.url }}">{{ paper.doi }}</a></p>
        {% endif %}
      </li>
    {% endfor %}
  </ol>
</section>

<section class="tg-publication-section">
  <h2>Conference Papers</h2>
  <ol class="tg-publication-list">
    {% for paper in site.data.publications.conference %}
      <li class="tg-publication-item">
        <p class="tg-publication-title">
          <a href="{{ paper.url }}">{{ paper.title }}</a>
        </p>
        <p class="tg-publication-meta">
          {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}{% if paper.abstract_number %}. Abstract {{ paper.abstract_number }}{% endif %}.
        </p>
        {% if paper.doi %}
          <p class="tg-publication-doi">doi: <a href="{{ paper.url }}">{{ paper.doi }}</a></p>
        {% endif %}
      </li>
    {% endfor %}
  </ol>
</section>
