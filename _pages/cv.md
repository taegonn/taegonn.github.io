---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description: Compact curriculum vitae for graduate application review.
---

{% include tg-academic-style.html %}

<div class="tg-page">
  <section class="tg-cv-lead">
    <div class="tg-kicker">Curriculum vitae</div>
    <p>
      M.S. candidate at Seoul National University studying medical AI, sleep physiology, and multimodal biomarkers for neurodegenerative disease progression.
    </p>
    <div class="tg-cv-actions">
      <a href="mailto:ghgh3110@snu.ac.kr">ghgh3110@snu.ac.kr</a>
      <a href="https://scholar.google.com/citations?user=gZOAJD4AAAAJ&hl=en">Google Scholar</a>
      <a href="https://orcid.org/0009-0001-1388-0903">ORCID</a>
      <a href="{{ '/assets/rendercv/rendercv_output/Tae-Gon_Noh_CV.pdf' | relative_url }}">Download PDF</a>
    </div>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Education</h2>
      <p class="tg-section-note">Academic training.</p>
    </div>
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
    <div class="tg-section-head">
      <h2>Research Experience</h2>
      <p class="tg-section-note">Laboratory appointments.</p>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">2024 - present</div>
      <div>
        <p class="tg-cv-title">Graduate Researcher, Seoul National University</p>
        <p class="tg-cv-meta">Advisor: Prof. Ki-Young Jung</p>
      </div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">2023 - 2024</div>
      <div>
        <p class="tg-cv-title">Research Intern, Seoul National University Hospital</p>
        <p class="tg-cv-meta">Advisor: Prof. Ki-Young Jung</p>
      </div>
    </div>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Research Focus</h2>
      <p class="tg-section-note">Core research directions.</p>
    </div>
    <div class="tg-focus-grid">
      <article class="tg-focus-item">
        <h3>Medical AI</h3>
        <p>Foundation model-based medical AI for disease progression modeling in Parkinson's disease and isolated REM sleep behavior disorder.</p>
      </article>
      <article class="tg-focus-item">
        <h3>Quantitative Biomarkers</h3>
        <p>Sleep and electrophysiology biomarkers from PSG, EEG, EOG, EMG, ECG, brain MRI, and clinical data.</p>
      </article>
      <article class="tg-focus-item">
        <h3>Clinical Prediction</h3>
        <p>Survival modeling, heterogeneity modeling, longitudinal analysis, and clinical prediction in prodromal neurodegenerative disease.</p>
      </article>
    </div>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Peer-reviewed Papers</h2>
      <p class="tg-section-note">{{ site.data.publications.peer_reviewed | size }} published journal articles.</p>
    </div>
    <ol class="tg-cv-publications">
      {% for paper in site.data.publications.peer_reviewed %}
        <li>
          <div>
            <p class="tg-cv-title"><a href="{{ paper.url }}">{{ paper.title }}</a></p>
            <p class="tg-cv-publication-meta">
              {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}.
            </p>
          </div>
        </li>
      {% endfor %}
    </ol>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Conference Papers</h2>
      <p class="tg-section-note">{{ site.data.publications.conference | size }} published abstracts and proceedings.</p>
    </div>
    <ol class="tg-cv-publications">
      {% for paper in site.data.publications.conference %}
        <li>
          <div>
            <p class="tg-cv-title"><a href="{{ paper.url }}">{{ paper.title }}</a></p>
            <p class="tg-cv-publication-meta">
              {{ paper.authors }}. <em>{{ paper.venue }}</em>. {{ paper.year }}{% if paper.volume %};{{ paper.volume }}{% endif %}{% if paper.issue %}({{ paper.issue }}){% endif %}{% if paper.pages %}:{{ paper.pages }}{% endif %}{% if paper.abstract_number %}. Abstract {{ paper.abstract_number }}{% endif %}.
            </p>
          </div>
        </li>
      {% endfor %}
    </ol>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Honors & Awards</h2>
      <p class="tg-section-note">Selected awards and presentation honors.</p>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Dec 2025</div>
      <div>Paper Award, Seoul National University.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Jul 2025</div>
      <div>Award for Oral Presentation, Korean Sleep Research Society.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Dec 2024</div>
      <div>Paper Award, Seoul National University.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Jul 2024</div>
      <div>Grand Award for Poster Presentation, Korean Society of Sleep Medicine.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Nov 2023</div>
      <div>Award for Poster Presentation, Korean Sleep Research Society.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Jul 2023</div>
      <div>Award for Poster Presentation, Korean Society of Sleep Medicine.</div>
    </div>
    <div class="tg-cv-item">
      <div class="tg-cv-date">Aug 2020</div>
      <div>2nd Award for CANSAT Korea, Korea Advanced Institute of Science and Technology.</div>
    </div>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Professional Memberships</h2>
      <p class="tg-section-note">Society memberships.</p>
    </div>
    <ul class="tg-cv-list">
      <li>American Academy of Sleep Medicine, student member, Dec 2023-present.</li>
      <li>Korean Sleep Research Society, student member, Mar 2023-present.</li>
      <li>Korean Society of Sleep Medicine, student member, Mar 2023-present.</li>
      <li>Korean EEG Study Group, student member, Feb 2023-present.</li>
    </ul>
  </section>

  <section class="tg-cv-section">
    <div class="tg-section-head">
      <h2>Skills</h2>
      <p class="tg-section-note">Methods and technical tools.</p>
    </div>
    <div class="tg-cv-skills">
      <div><strong>Programming</strong><br>Python, MATLAB, C/C++, Linux</div>
      <div><strong>Machine Learning</strong><br>PyTorch, scikit-learn, representation learning, foundation model-based medical AI</div>
      <div><strong>Signal Processing and Sleep Analysis</strong><br>PSG, EEG, EOG, EMG, ECG, connectivity analysis, time-frequency analysis</div>
      <div><strong>Neuroimaging</strong><br>Brain MRI preprocessing and analysis, NIfTI processing, atlas-based regional analysis</div>
      <div><strong>Genetics and Statistical Genomics</strong><br>Polygenic risk score analysis, GWAS summary statistics analysis, Mendelian randomization</div>
      <div><strong>Biostatistics and Clinical Data Analysis</strong><br>Regression modeling, survival analysis, longitudinal analysis, clinical prediction modeling</div>
    </div>
  </section>
</div>
