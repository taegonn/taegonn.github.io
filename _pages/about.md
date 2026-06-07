---
layout: about
permalink: /
selected_papers: false
social: false
announcements:
  enabled: false
latest_posts:
  enabled: false
---

<style>
  header.post-header,
  .post-title {
    display: none !important;
  }
</style>

{% include tg-academic-style.html %}

<div class="tg-page tg-home">
  <section class="tg-hero">
    <div>
      <div class="tg-kicker">Medical AI, sleep physiology, and clinical neuroscience</div>
      <h1 class="tg-hero-name">Tae-Gon Noh</h1>
      <p class="tg-hero-role">M.S. candidate in Neuroscience, Seoul National University</p>
      <p class="tg-hero-summary">
        I study quantitative biomarkers and disease progression in prodromal neurodegenerative disease, using multimodal sleep, electrophysiology, neuroimaging, and clinical data.
      </p>
      <nav class="tg-links" aria-label="Academic profiles">
        <a href="https://scholar.google.com/citations?user=gZOAJD4AAAAJ&hl=en">Google Scholar</a>
        <a href="https://orcid.org/0009-0001-1388-0903">ORCID</a>
        <a href="https://www.linkedin.com/in/tae-gon-noh-778857318/">LinkedIn</a>
        <a href="https://github.com/taegonn">GitHub</a>
      </nav>
      <div class="tg-stat-grid" aria-label="Research summary">
        <div>
          <span class="tg-stat-value">{{ site.data.publications.peer_reviewed | size }}</span>
          <span class="tg-stat-label">peer-reviewed papers</span>
        </div>
        <div>
          <span class="tg-stat-value">{{ site.data.publications.conference | size }}</span>
          <span class="tg-stat-label">conference papers</span>
        </div>
        <div>
          <span class="tg-stat-value">3</span>
          <span class="tg-stat-label">research axes</span>
        </div>
      </div>
    </div>
    <div class="tg-hero-media">
      <img class="tg-portrait" src="{{ '/assets/img/tg-profile.jpg' | relative_url }}" alt="Tae-Gon Noh">
    </div>
  </section>

  <section class="tg-section">
    <div class="tg-section-head">
      <h2>Research Focus</h2>
      <p class="tg-section-note">Multimodal modeling for sleep and neurodegeneration.</p>
    </div>
    <div class="tg-focus-grid">
      <article class="tg-focus-item">
        <h3>Medical AI</h3>
        <p>Disease progression modeling for Parkinson's disease, isolated REM sleep behavior disorder, and related neurodegenerative diseases.</p>
      </article>
      <article class="tg-focus-item">
        <h3>Sleep and Biosignals</h3>
        <p>Quantitative biomarkers from PSG, EEG, EMG, sleep physiology, and clinical neurophysiology data.</p>
      </article>
      <article class="tg-focus-item">
        <h3>Clinical Prediction</h3>
        <p>Survival modeling, heterogeneity analysis, and longitudinal modeling for neurodegenerative disease.</p>
      </article>
    </div>
  </section>

  <section class="tg-section">
    <div class="tg-section-head">
      <h2>Highlights & Selected Works</h2>
      <p class="tg-section-note">Recent and representative outputs.</p>
    </div>
    <div class="tg-feed-wrap">
      <div class="tg-feed-toolbar">
        <strong>Selected work feed</strong>
        <span>{{ site.data.highlights | size }} items</span>
      </div>
      <div class="tg-feed" tabindex="0">
        {% for item in site.data.highlights %}
          <article class="tg-work-card">
            <img src="{{ item.image | prepend: '/assets/img/' | relative_url }}" alt="{{ item.alt }}">
            <div>
              <p class="tg-work-title">
                {% if item.url %}
                  <a href="{{ item.url }}">{{ item.title }}</a>
                {% else %}
                  {{ item.title }}
                {% endif %}
              </p>
              <p class="tg-work-meta">{{ item.meta }}</p>
            </div>
          </article>
        {% endfor %}
      </div>
    </div>
  </section>
</div>
