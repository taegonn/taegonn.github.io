---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description: Compact curriculum vitae for graduate application review.
---

<style>
  .tg-cv-section {
    border-top: 1px solid var(--global-divider-color, #e5e7eb);
    margin-top: 1.8rem;
    padding-top: 1.25rem;
  }

  .tg-cv-section:first-of-type {
    border-top: 0;
    margin-top: 0;
    padding-top: 0;
  }

  .tg-cv-item {
    display: grid;
    gap: 0.4rem 1rem;
    grid-template-columns: 10rem minmax(0, 1fr);
    margin-bottom: 1rem;
  }

  .tg-cv-date {
    color: var(--global-text-color-light, #6b7280);
    font-size: 0.9rem;
  }

  .tg-cv-title {
    font-weight: 650;
    margin: 0;
  }

  .tg-cv-meta,
  .tg-cv-note,
  .tg-cv-publication-meta {
    color: var(--global-text-color-light, #6b7280);
    font-size: 0.92rem;
    line-height: 1.45;
    margin: 0.15rem 0 0;
  }

  .tg-cv-list {
    margin: 0.45rem 0 0;
    padding-left: 1.15rem;
  }

  .tg-cv-list li {
    margin-bottom: 0.35rem;
  }

  .tg-cv-publications {
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .tg-cv-publications li {
    border-top: 1px solid var(--global-divider-color, #e5e7eb);
    padding: 0.8rem 0;
  }

  .tg-cv-publications li:first-child {
    border-top: 0;
    padding-top: 0;
  }

  .tg-cv-skills {
    display: grid;
    gap: 0.7rem 1rem;
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  @media (max-width: 720px) {
    .tg-cv-item,
    .tg-cv-skills {
      grid-template-columns: 1fr;
    }
  }
</style>

<section class="tg-cv-section">
  <p>
    M.S. candidate at Seoul National University studying medical AI, sleep physiology, and multimodal biomarkers for neurodegenerative disease progression.
  </p>
  <p class="tg-cv-note">
    Email: <a href="mailto:ghgh3110@snu.ac.kr">ghgh3110@snu.ac.kr</a> /
    <a href="https://scholar.google.com/citations?user=gZOAJD4AAAAJ&hl=en">Google Scholar</a> /
    <a href="https://orcid.org/0009-0001-1388-0903">ORCID</a>
  </p>
</section>

<section class="tg-cv-section">
  <h2>Education</h2>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2024 - expected 2026</div>
    <div>
      <p class="tg-cv-title">M.S. candidate in Neuroscience, Seoul National University</p>
      <p class="tg-cv-meta">Seoul, South Korea / GPA: 3.56/4.0 / Advisor: Prof. Ki-Young Jung</p>
    </div>
  </div>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2018 - 2024</div>
    <div>
      <p class="tg-cv-title">B.S. in Biology, minor in Computer Engineering, Pusan National University</p>
      <p class="tg-cv-meta">Busan, South Korea / GPA: 3.57/4.5 / Mandatory military service, Republic of Korea Army, 2020-2022</p>
    </div>
  </div>
</section>

<section class="tg-cv-section">
  <h2>Research Experience</h2>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2024 - present</div>
    <div>
      <p class="tg-cv-title">Graduate Researcher, Seoul National University</p>
      <p class="tg-cv-meta">Advisor: Prof. Ki-Young Jung</p>
      <ul class="tg-cv-list">
        <li>Foundation model-based disease progression modeling using brain MRI and PSG.</li>
        <li>Multimodal biomarkers for Parkinson's disease and isolated REM sleep behavior disorder.</li>
      </ul>
    </div>
  </div>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2023 - 2024</div>
    <div>
      <p class="tg-cv-title">Research Intern, Seoul National University Hospital</p>
      <p class="tg-cv-meta">Advisor: Prof. Ki-Young Jung</p>
      <ul class="tg-cv-list">
        <li>Data-driven quantification of sleep and electrophysiological markers in isolated REM sleep behavior disorder.</li>
      </ul>
    </div>
  </div>
</section>

<section class="tg-cv-section">
  <h2>Research Focus</h2>
  <ul class="tg-cv-list">
    <li>Foundation model-based medical AI for disease progression modeling in Parkinson's disease and isolated REM sleep behavior disorder.</li>
    <li>Quantitative sleep and electrophysiology biomarkers from PSG, EEG, EMG, EOG, ECG, brain MRI, and clinical data.</li>
    <li>Survival modeling, heterogeneity modeling, longitudinal analysis, and clinical prediction in prodromal neurodegenerative disease.</li>
  </ul>
</section>

<section class="tg-cv-section">
  <h2>Peer-reviewed Papers</h2>
  <ol class="tg-cv-publications">
    {% for paper in site.data.publications.peer_reviewed %}
      <li>
        <p class="tg-cv-title"><a href="{{ paper.url }}">{{ paper.title }}</a></p>
        <p class="tg-cv-publication-meta">
          {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}.
        </p>
      </li>
    {% endfor %}
  </ol>
</section>

<section class="tg-cv-section">
  <h2>Conference Papers</h2>
  <ol class="tg-cv-publications">
    {% for paper in site.data.publications.conference %}
      <li>
        <p class="tg-cv-title"><a href="{{ paper.url }}">{{ paper.title }}</a></p>
        <p class="tg-cv-publication-meta">
          {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}{% if paper.abstract_number %}. Abstract {{ paper.abstract_number }}{% endif %}.
        </p>
      </li>
    {% endfor %}
  </ol>
</section>

<section class="tg-cv-section">
  <h2>Honors & Awards</h2>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2025</div>
    <div>Paper Award, Seoul National University; Award for Oral Presentation, Korean Sleep Research Society.</div>
  </div>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2024</div>
    <div>Paper Award, Seoul National University; Grand Award for Poster Presentation, Korean Society of Sleep Medicine.</div>
  </div>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2023</div>
    <div>Award for Poster Presentation, Korean Sleep Research Society; Award for Poster Presentation, Korean Society of Sleep Medicine.</div>
  </div>
  <div class="tg-cv-item">
    <div class="tg-cv-date">2020</div>
    <div>2nd Award for CANSAT Korea, Korea Advanced Institute of Science and Technology.</div>
  </div>
</section>

<section class="tg-cv-section">
  <h2>Professional Memberships</h2>
  <ul class="tg-cv-list">
    <li>American Academy of Sleep Medicine, student member, Dec 2023-present.</li>
    <li>Korean Sleep Research Society, student member, Mar 2023-present.</li>
    <li>Korean Society of Sleep Medicine, student member, Mar 2023-present.</li>
    <li>Korean EEG Study Group, student member, Feb 2023-present.</li>
  </ul>
</section>

<section class="tg-cv-section">
  <h2>Skills</h2>
  <div class="tg-cv-skills">
    <div><strong>Programming</strong><br>Python, MATLAB, C/C++, Linux</div>
    <div><strong>Machine Learning</strong><br>PyTorch, scikit-learn, representation learning, foundation model-based medical AI</div>
    <div><strong>Signal Processing and Sleep Analysis</strong><br>PSG, EEG, EOG, EMG, ECG, connectivity analysis, time-frequency analysis</div>
    <div><strong>Neuroimaging</strong><br>Brain MRI preprocessing and analysis, NIfTI processing, atlas-based regional analysis</div>
    <div><strong>Genetics and Statistical Genomics</strong><br>Polygenic risk score analysis, GWAS summary statistics analysis, Mendelian randomization</div>
    <div><strong>Biostatistics and Clinical Data Analysis</strong><br>Regression modeling, survival analysis, longitudinal analysis, clinical prediction modeling</div>
  </div>
</section>
