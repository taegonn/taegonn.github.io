---
layout: about
permalink: /
selected_papers: false
social: true
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

.name-title {
  text-align: center;
  font-size: 2.8rem;
  font-weight: 800;
  margin-bottom: 2.5rem;
  color: #212529;
}

.intro-container {
  display: flex;
  align-items: center;
  gap: 3rem;
  margin-bottom: 3.5rem;
}

@media (max-width: 768px) {
  .intro-container {
    flex-direction: column;
    text-align: center;
    gap: 1.5rem;
  }
}

.intro-image img {
  width: 180px;
  height: 180px;
  object-fit: cover;
  border-radius: 50%;
  box-shadow: 0 4px 14px rgba(0,0,0,0.12);
}

.intro-text {
  font-size: 1.05rem;
  line-height: 1.6;
  color: #333;
  text-align: left;
}

/* 깃허브 링크 다크모드 대응을 위한 클래스 */
.github-link {
  color: #333;
  text-decoration: none;
}

.research-keyword {
  color: #212529;
  border-bottom: 2.5px solid #a8c1d9;
}

.post h2 { margin-top: 3.5rem !important; margin-bottom: 1.5rem !important; }

/* 🌟 Highlights & News 카드 디자인 */
.news-card {
  display: flex;
  gap: 1.5rem;
  margin-bottom: 2rem;
  padding: 1.2rem;
  border-radius: 12px;
  background-color: #f8f9fa;
  border: 1px solid #e9ecef;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.news-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.08);
}

.news-image {
  flex: 0 0 220px;
  display: flex;
  align-items: center;
}

.news-image img {
  width: 100%;
  height: auto;
  border-radius: 8px;
  border: 1px solid #dee2e6;
}

.news-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.news-title {
  font-weight: 700;
  font-size: 1.15rem;
  color: #2c3e50;
  margin-bottom: 0.3rem;
}

.news-meta {
  font-size: 0.9rem;
  color: #6c757d;
  margin-bottom: 0.8rem;
}

@media (max-width: 768px) {
  .news-card { flex-direction: column; }
  .news-image { flex: auto; width: 100%; }
}

/* ==========================================
   🌙 테마별 다크모드 (Dark Mode) 완벽 대응 오버라이드
   ========================================== */
html[data-theme='dark'] .name-title {
  color: #f8f9fa !important;
}

html[data-theme='dark'] .intro-text {
  color: #e0e0e0 !important;
}

html[data-theme='dark'] .github-link {
  color: #e0e0e0 !important;
}

html[data-theme='dark'] .research-keyword {
  color: #f8f9fa !important;
  border-bottom: 2.5px solid #4a7a96;
}

html[data-theme='dark'] .news-card {
  background-color: #1c1c1e !important;
  border: 1px solid #2c2c2e !important;
}

html[data-theme='dark'] .news-title {
  color: #f8f9fa !important;
}

html[data-theme='dark'] .news-meta {
  color: #a0aab2 !important;
}

html[data-theme='dark'] .news-image img {
  border: 1px solid #3a3a3c !important;
}
</style>


<div class="name-title">Tae-Gon Noh</div>

<div class="intro-container">
  <div class="intro-image">
    <img src="{{ '/assets/img/tg-profile.jpg' | relative_url }}" alt="Tae-Gon Noh">
  </div>
  <div class="intro-text">
    <span style="font-weight: 600; font-size: 1.15rem;">M.S. candidate in Neuroscience</span>, Seoul National University<br><br>
    My research uses <strong>machine learning, sleep physiology, medical imaging,</strong> and <strong>clinical neuroscience</strong> to model disease progression in neurodegenerative diseases.
    
    <div style="margin-top: 1.2rem; font-weight: 500; font-size: 0.95rem;">
      <a href="https://scholar.google.com/citations?user=gZOAJD4AAAAJ&hl=en" style="margin-right: 15px; color: #4285F4; text-decoration: none;">🎓 Google Scholar</a>
      <a href="https://orcid.org/0009-0001-1388-0903" style="margin-right: 15px; color: #A6CE39; text-decoration: none;">iD ORCID</a>
      <a href="https://www.linkedin.com/in/tae-gon-noh-778857318/" style="margin-right: 15px; color: #0077B5; text-decoration: none;">💼 LinkedIn</a>
      <a href="https://github.com/taegonn" class="github-link">🐙 GitHub</a>
    </div>
  </div>
</div>


## Research Focus

<ul>
  <li style="margin-bottom: 0.5rem;"><strong class="research-keyword">Medical AI:</strong> Disease progression modeling for Parkinson's disease, isolated REM sleep behavior disorder, and related neurodegenerative diseases.</li>
  <li style="margin-bottom: 0.5rem;"><strong class="research-keyword">Sleep and biosignals:</strong> Quantitative biomarkers from PSG, EEG, EMG, sleep physiology, and clinical neurophysiology data.</li>
  <li style="margin-bottom: 0.5rem;"><strong class="research-keyword">Clinical prediction:</strong> Survival modeling, heterogeneity analysis, and longitudinal modeling for neurodegenerative disease.</li>
</ul>


## Highlights & Selected Works
<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/Basal_EMG_amplitude.jpg' | relative_url }}" alt="Basal EMG amplitude">
  </div>
  <div class="news-content">
    <div class="news-title">Basal electromyographic amplitude in rapid eye movement (REM) and non-rapid eye movement (NREM) sleep as a predictor of disease progression in isolated REM sleep behavior disorder</div>
    <div class="news-meta">TG Noh, JI Byun, EK St. Louis, KY Jung.<br>Published in <em>SLEEPJ</em> (2026)</div>
  </div>
</div>

<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/Continuous_RWA.jpg' | relative_url }}" alt="Continuous RWA">
  </div>
  <div class="news-content">
    <div class="news-title">Continuous REM sleep without atonia quantification improves prediction of phenoconversion to α-synucleinopathies in isolated REM sleep behavior disorder</div>
    <div class="news-meta">TG Noh, S Lee, Y Lee, N Kim, DS Shin, JH Shin, JI Byun, HJ Kim, KY Jung.<br>Published in <em>Sleep Medicine</em> (2025)</div>
  </div>
</div>

<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/Enhanced_delta_gamma_PAC.jpg' | relative_url }}" alt="Enhanced delta gamma PAC">
  </div>
  <div class="news-content">
    <div class="news-title">Enhanced delta-gamma phase-amplitude coupling during phasic rapid eye movement sleep in isolated rapid eye movement sleep behavior disorder</div>
    <div class="news-meta">TG Noh, KM Choi, JS Jun, JW Shin, JI Byun, JS Sunwoo, KY Jung.<br>Published in <em>Sleep</em> (2025)</div>
  </div>
</div>

<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/ERP_prediction.jpg' | relative_url }}" alt="ERP prediction">
  </div>
  <div class="news-content">
    <div class="news-title">Prediction of phenoconversion into alpha-synucleinopathy in patients with isolated REM sleep behavior disorder using event-related potentials during visuospatial attention tasks</div>
    <div class="news-meta">KM Choi, KS Cha, TG Noh, S Lee, YW Shin, JI Byun, JS Jun, JH Shin, ...<br>Published in <em>Sleep</em> (2025)</div>
  </div>
</div>

<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/FC_network.jpg' | relative_url }}" alt="FC network">
  </div>
  <div class="news-content">
    <div class="news-title">Altered functional brain networks in isolated REM sleep behavior disorder during phasic REM sleep</div>
    <div class="news-meta">KM Choi, TG Noh, JS Sunwoo, JI Byun, KY Jung.<br>Published in <em>Sleep Medicine</em> (2025)</div>
  </div>
</div>
