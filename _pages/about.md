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
/* al-folio 테마가 자동으로 출력하는 기본 제목 숨기기 */
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
  background-color: #f8f9fa; /* 아주 연한 회색 배경 */
  border: 1px solid #e9ecef;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.news-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.08);
}

.news-image {
  flex: 0 0 220px; /* 이미지 영역 고정 너비 */
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

.news-desc {
  font-size: 0.95rem;
  line-height: 1.5;
  color: #495057;
}

/* 모바일 화면에서는 카드 이미지가 위로 가도록 변경 */
@media (max-width: 768px) {
  .news-card { flex-direction: column; }
  .news-image { flex: auto; width: 100%; }
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
      <a href="https://github.com/taegonn" style="color: #333; text-decoration: none;">🐙 GitHub</a>
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

<!-- 첫 번째 뉴스/논문 카드 -->
<div class="news-card">
  <div class="news-image">
    <!-- assets/img 폴더에 abstract 이미지를 넣고 파일명을 아래에 맞춰주세요 -->
    <img src="{{ '/assets/img/abstract-1.jpg' | relative_url }}" alt="Graphical Abstract">
  </div>
  <div class="news-content">
    <div class="news-title">논문 제목 또는 하이라이트 타이틀 입력</div>
    <div class="news-meta">Published in <em>Journal Name</em> (2024)</div>
    <div class="news-desc">
      이곳에 해당 연구의 Graphical Abstract에 대한 설명이나 핵심 발견(Key findings)을 간략하게 적습니다. 2~3문장으로 요약하여 방문자가 직관적으로 연구 내용을 파악할 수 있게 유도하세요.
    </div>
  </div>
</div>

<!-- 두 번째 뉴스/논문 카드 -->
<div class="news-card">
  <div class="news-image">
    <img src="{{ '/assets/img/abstract-2.jpg' | relative_url }}" alt="Graphical Abstract">
  </div>
  <div class="news-content">
    <div class="news-title">두 번째 프로젝트 또는 학회 발표 내용</div>
    <div class="news-meta">Presented at <em>Conference Name</em> (2023)</div>
    <div class="news-desc">
      학회에서 발표한 포스터의 일부분이나 프로젝트의 파이프라인 이미지를 넣고, 어떤 문제를 어떤 모델로 해결했는지 어필할 수 있습니다.
    </div>
  </div>
</div>
