---
title: "About"
excerpt: "About me"
author_profile: true
permalink: /
classes: wide
redirect_from: 
  - /index/
  - /index.html
---

<!-- ============ HERO SECTION ============ -->
<div class="hero-banner fade-in-section">
  <div class="hero-content">
    <h1 class="hero-title">Exploring Life at the <span class="hero-accent">Intersection</span> of Biology &amp; Computation</h1>
    <p class="hero-subtitle">Scientist at Altos Labs · Computational Biology · Chromatin Biophysics · AI for Drug Discovery</p>
    <div class="hero-actions">
      <a href="/publications/" class="hero-btn hero-btn-primary">Publications</a>
      <a href="/cv/" class="hero-btn hero-btn-outline">Curriculum Vitae</a>
    </div>
  </div>
  <div class="hero-visual">
    <div class="hero-orb hero-orb-1"></div>
    <div class="hero-orb hero-orb-2"></div>
    <div class="hero-orb hero-orb-3"></div>
  </div>
</div>

<!-- ============ ABOUT ============ -->

I am currently a scientist in the Institute of Computation  at [Altos Labs](https://www.altoslabs.com/). Before moving to the Bay Area, I had a short stint at [MathWorks](https://www.mathworks.com/) as a senior application engineer in the computational biology group.

I am mostly interested in the intersection of **biology**, **computation**, **modeling** (statistical and first-principle), and **artificial intelligence**. Before pivoting to industry, I obtained a PhD at the University of California San Diego under the supervision of [Prof. David Saintillan](http://stokeslet.ucsd.edu/index.html) in computational biophysics to understand how our genome organizes inside the nucleus of a cell.

Prior to UCSD, I obtained an M.S.(Engg.) degree from Jawaharlal Nehru Centre for Advanced Scientific Research (Bangalore, India) under the supervision of [Prof. Meheboob Alam](https://www.jncasr.ac.in/faculty/meheboob/) and a B.Tech. degree in Chemical Engineering from National Institute of Technology Karnataka Surathkal.

---

<!-- ============ RESEARCH CARDS ============ -->
## Research Interests

<div class="research-cards fade-in-section">
  <div class="research-card">
    <div class="research-card-icon">🧬</div>
    <h3 class="research-card-title">Computational Biology &amp; Biophysics</h3>
    <p class="research-card-desc">Modeling cellular processes from molecular to tissue scales, with focus on chromatin dynamics and gene regulation.</p>
  </div>
  <div class="research-card">
    <div class="research-card-icon">📊</div>
    <h3 class="research-card-title">Statistical &amp; First-Principle Modeling</h3>
    <p class="research-card-desc">Bridging data-driven and physics-based approaches to understand complex biological phenomena.</p>
  </div>
  <div class="research-card">
    <div class="research-card-icon">🤖</div>
    <h3 class="research-card-title">AI for Drug Discovery</h3>
    <p class="research-card-desc">Graph-based machine learning and deep learning methods for molecular property prediction and therapeutic design.</p>
  </div>
  <div class="research-card">
    <div class="research-card-icon">🔬</div>
    <h3 class="research-card-title">Multiscale Modeling</h3>
    <p class="research-card-desc">Connecting nano-scale chromatin mechanics to micro-scale nuclear organization and epigenetic regulation.</p>
  </div>
</div>

---

## Recent News

<div class="news-timeline fade-in-section">
  <div class="news-line"></div>

  {% assign displayed_count = 0 %}
  {% for news in site.data.news %}
    {% if news.text != nil and news.text != "" and displayed_count < 5 %}
  <div class="news-item">
    <div class="news-dot"></div>
    <div class="news-date">{{ news.date }}</div>
    <div class="news-text">
      {{ news.text | markdownify | remove: '<p>' | remove: '</p>' }}
    </div>
  </div>
      {% assign displayed_count = displayed_count | plus: 1 %}
    {% endif %}
  {% endfor %}
</div>

<div style="text-align: right; margin-top: 10px;">
  <a href="/allnews/" class="news-see-all">... see all News →</a>
</div>

<!-- ======== PAGE-SPECIFIC STYLES ======== -->
<style>
/* ---- Hero Banner ---- */
.hero-banner {
  position: relative;
  padding: 40px 32px 36px;
  margin: -10px -10px 28px -10px;
  border-radius: 12px;
  background: linear-gradient(135deg, var(--bg-secondary) 0%, var(--card-bg) 50%, var(--bg-secondary) 100%);
  border: 1px solid var(--border);
  overflow: hidden;
}

.hero-content {
  position: relative;
  z-index: 2;
}

.hero-title {
  font-family: 'Nunito Sans', 'Avenir Next', sans-serif !important;
  font-size: 1.65em;
  font-weight: 700;
  line-height: 1.35;
  color: var(--text) !important;
  margin: 0 0 12px 0;
  padding: 0;
  border: none !important;
}

.hero-accent {
  color: var(--heading);
  position: relative;
}

.hero-accent::after {
  content: '';
  position: absolute;
  bottom: 2px;
  left: 0;
  width: 100%;
  height: 6px;
  background: var(--accent);
  opacity: 0.2;
  border-radius: 3px;
}

.hero-subtitle {
  font-family: 'Barlow', sans-serif;
  font-weight: 300;
  font-size: 1em;
  color: var(--text-muted);
  margin: 0 0 20px 0;
  letter-spacing: 0.3px;
}

.hero-actions {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

.hero-btn {
  display: inline-block;
  padding: 8px 22px;
  border-radius: 6px;
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 600;
  font-size: 0.88em;
  text-decoration: none !important;
  border: none !important;
  transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
  cursor: pointer;
}

.hero-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 14px var(--card-shadow);
}

.hero-btn-primary {
  background: var(--accent);
  color: #fff !important;
}

.hero-btn-primary:hover {
  background: #5e3c3e;
  color: #fff !important;
}

[data-theme="dark"] .hero-btn-primary:hover {
  background: #a06568;
}

.hero-btn-outline {
  background: transparent;
  color: var(--accent) !important;
  border: 1.5px solid var(--accent) !important;
}

.hero-btn-outline:hover {
  background: var(--accent);
  color: #fff !important;
}

/* Decorative floating orbs */
.hero-visual {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  width: 40%;
  pointer-events: none;
  z-index: 1;
}

.hero-orb {
  position: absolute;
  border-radius: 50%;
  opacity: 0.12;
}

.hero-orb-1 {
  width: 180px;
  height: 180px;
  background: radial-gradient(circle, var(--accent) 0%, transparent 70%);
  top: -30px;
  right: -20px;
  animation: orbFloat 8s ease-in-out infinite;
}

.hero-orb-2 {
  width: 120px;
  height: 120px;
  background: radial-gradient(circle, var(--heading) 0%, transparent 70%);
  bottom: -10px;
  right: 80px;
  animation: orbFloat 6s ease-in-out infinite reverse;
}

.hero-orb-3 {
  width: 80px;
  height: 80px;
  background: radial-gradient(circle, var(--accent) 0%, transparent 70%);
  top: 40%;
  right: 30%;
  animation: orbFloat 10s ease-in-out infinite;
}

@keyframes orbFloat {
  0%, 100% { transform: translate(0, 0); }
  33% { transform: translate(8px, -12px); }
  66% { transform: translate(-6px, 8px); }
}

@media (max-width: 767px) {
  .hero-banner {
    padding: 28px 20px 24px;
    margin: -5px -5px 20px -5px;
  }
  .hero-title {
    font-size: 1.3em;
  }
  .hero-visual {
    display: none;
  }
}

/* ---- Research Cards ---- */
.research-cards {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px;
  margin-top: 16px;
  margin-bottom: 8px;
}

@media (max-width: 600px) {
  .research-cards {
    grid-template-columns: 1fr;
  }
}

.research-card {
  padding: 20px 18px 16px;
  border-radius: 8px;
  background: var(--card-bg);
  border: 1px solid var(--border);
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
  cursor: default;
}

.research-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 20px var(--card-shadow);
  border-color: var(--accent);
}

.research-card-icon {
  font-size: 1.8em;
  margin-bottom: 8px;
  line-height: 1;
}

.research-card-title {
  font-family: 'Nunito Sans', sans-serif !important;
  font-size: 0.98em !important;
  font-weight: 600 !important;
  color: var(--heading) !important;
  margin: 0 0 6px 0 !important;
  padding: 0 !important;
}

.research-card-desc {
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 300;
  font-size: 0.87em;
  color: var(--text-muted);
  line-height: 1.55;
  margin: 0;
}

/* ---- News Timeline ---- */
.news-timeline {
  position: relative;
  padding-left: 28px;
  margin-top: 10px;
}

.news-line {
  position: absolute;
  left: 5px;
  top: 6px;
  bottom: 0;
  width: 2px;
  background: var(--border, #e9ecef);
}

.news-item {
  position: relative;
  margin-bottom: 22px;
}

.news-dot {
  position: absolute;
  left: -27px;
  top: 5px;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: var(--accent, #784e51);
  border: 2px solid var(--bg, #fff);
  box-shadow: 0 0 0 2px var(--border, #e9ecef);
  transition: transform 0.2s ease;
}

.news-item:hover .news-dot {
  transform: scale(1.3);
}

.news-date {
  font-family: 'Barlow', sans-serif;
  font-weight: 400;
  font-size: 0.82em;
  color: var(--accent, #784e51);
  margin-bottom: 2px;
}

.news-text {
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 300;
  color: var(--text-light, #555);
  font-size: 0.93em;
  line-height: 1.55;
}

.news-text a {
  color: var(--heading, #893636) !important;
}

.news-see-all {
  color: var(--accent, #784e51) !important;
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 500;
  font-size: 0.9em;
  text-decoration: none !important;
  border-bottom: 1px dashed var(--accent, #784e51) !important;
  transition: opacity 0.2s ease;
}

.news-see-all:hover {
  opacity: 0.75;
}
</style>
