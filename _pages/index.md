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

<div class="hero-intro fade-in-section">
  <h1 style="font-family: 'Nunito Sans', sans-serif; font-weight: 700; color: var(--heading); font-size: 1.75em; margin-bottom: 0.15em; letter-spacing: -0.3px;">
    Hi, I'm Achal <span style="display:inline-block; animation: wave 2.5s infinite; transform-origin: 70% 70%;">👋</span>
  </h1>
  <p style="font-family: 'Nunito Sans', sans-serif; font-weight: 300; color: var(--accent); font-size: 1.12em; margin-bottom: 0.3em; line-height: 1.5;">
    <span id="typed-output"></span><span id="typed-cursor" style="color: var(--accent);">|</span>
  </p>
</div>

<div class="fade-in-section" style="margin-top: 0.5em;">

I am currently a scientist in the Institute of Computation at [Altos Labs](https://www.altoslabs.com/). Before moving to the Bay Area, I had a short stint at [MathWorks](https://www.mathworks.com/) as a senior application engineer in the computational biology group.

I am mostly interested in the intersection of **biology**, **computation**, **modeling** (statistical and first-principle), and **artificial intelligence**. Before pivoting to industry, I obtained a PhD at the University of California San Diego under the supervision of [Prof. David Saintillan](http://stokeslet.ucsd.edu/index.html) in computational biophysics to understand how our genome organizes inside the nucleus of a cell.

Prior to UCSD, I obtained an M.S.(Engg.) degree from Jawaharlal Nehru Centre for Advanced Scientific Research (Bangalore, India) under the supervision of [Prof. Meheboob Alam](https://www.jncasr.ac.in/faculty/meheboob/) and a B.Tech. degree in Chemical Engineering from National Institute of Technology Karnataka Surathkal.

</div>

---

## Research Interests

<div class="research-grid fade-in-section">
  <div class="research-card">
    <div class="research-icon">🧬</div>
    <div class="research-title">Computational Biology</div>
    <div class="research-desc">Biophysics &amp; genomics</div>
  </div>
  <div class="research-card">
    <div class="research-icon">📊</div>
    <div class="research-title">Statistical Modeling</div>
    <div class="research-desc">First-principle &amp; statistical</div>
  </div>
  <div class="research-card">
    <div class="research-icon">🤖</div>
    <div class="research-title">Machine Learning</div>
    <div class="research-desc">Graph ML for drug discovery</div>
  </div>
  <div class="research-card">
    <div class="research-icon">🔬</div>
    <div class="research-title">Chromatin &amp; Epigenetics</div>
    <div class="research-desc">Gene regulation &amp; organization</div>
  </div>
  <div class="research-card">
    <div class="research-icon">🧪</div>
    <div class="research-title">Multiscale Modeling</div>
    <div class="research-desc">From nano to macro scales</div>
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
/* Wave hand animation */
@keyframes wave {
  0%   { transform: rotate(0deg); }
  10%  { transform: rotate(14deg); }
  20%  { transform: rotate(-8deg); }
  30%  { transform: rotate(14deg); }
  40%  { transform: rotate(-4deg); }
  50%  { transform: rotate(10deg); }
  60%  { transform: rotate(0deg); }
  100% { transform: rotate(0deg); }
}

/* Typed cursor blink */
#typed-cursor {
  animation: blink 0.75s step-end infinite;
}
@keyframes blink {
  0%, 100% { opacity: 1; }
  50%      { opacity: 0; }
}

/* ---- Research Interest Cards ---- */
.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
  margin-top: 18px;
  margin-bottom: 28px;
}

.research-card {
  background: linear-gradient(135deg, var(--card-bg, #fdfdfd) 0%, var(--bg-secondary, #f8f9fa) 100%);
  border-radius: 10px;
  padding: 20px 18px;
  border-left: 3px solid var(--accent, #784e51);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: default;
}

.research-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 25px var(--card-shadow, rgba(120,78,81,0.12));
}

.research-icon {
  font-size: 1.5em;
  margin-bottom: 6px;
}

.research-title {
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 600;
  color: var(--heading, #893636);
  font-size: 0.95em;
}

.research-desc {
  font-family: 'Barlow', sans-serif;
  font-weight: 300;
  color: var(--text-muted, #777);
  font-size: 0.82em;
  margin-top: 4px;
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

/* ---- Mobile tweaks ---- */
@media (max-width: 600px) {
  .research-grid {
    grid-template-columns: 1fr 1fr;
    gap: 10px;
  }
  .research-card {
    padding: 14px 12px;
  }
}
</style>

<!-- ======== TYPING ANIMATION SCRIPT ======== -->
<script>
document.addEventListener('DOMContentLoaded', function() {
  var phrases = [
    'Scientist at Altos Labs.',
    'Computational biologist.',
    'Machine learning enthusiast.',
    'Exploring chromatin & epigenetics.',
    'Bridging biology and computation.'
  ];
  var el = document.getElementById('typed-output');
  if (!el) return;

  var phraseIdx = 0, charIdx = 0, deleting = false;

  function tick() {
    var current = phrases[phraseIdx];
    if (deleting) {
      el.textContent = current.substring(0, charIdx - 1);
      charIdx--;
    } else {
      el.textContent = current.substring(0, charIdx + 1);
      charIdx++;
    }

    var delay = deleting ? 35 : 65;

    if (!deleting && charIdx === current.length) {
      delay = 2200; // pause at full phrase
      deleting = true;
    } else if (deleting && charIdx === 0) {
      deleting = false;
      phraseIdx = (phraseIdx + 1) % phrases.length;
      delay = 450;
    }

    setTimeout(tick, delay);
  }

  tick();
});
</script>
