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

I am currently a scientist in the Institute of Computation  at [Altos Labs](https://www.altoslabs.com/). Before moving to the Bay Area, I had a short stint at [MathWorks](https://www.mathworks.com/) as a senior application engineer in the computational biology group.

I am mostly interested in the intersection of **biology**, **computation**, **modeling** (statistical and first-principle), and **artificial intelligence**. Before pivoting to industry, I obtained a PhD at the University of California San Diego under the supervision of [Prof. David Saintillan](http://stokeslet.ucsd.edu/index.html) in computational biophysics to understand how our genome organizes inside the nucleus of a cell.

Prior to UCSD, I obtained an M.S.(Engg.) degree from Jawaharlal Nehru Centre for Advanced Scientific Research (Bangalore, India) under the supervision of [Prof. Meheboob Alam](https://www.jncasr.ac.in/faculty/meheboob/) and a B.Tech. degree in Chemical Engineering from National Institute of Technology Karnataka Surathkal.

---

## Research Interests

- Computational biology and biophysics
- Statistical and first-principle modeling
- Graph based machine learning for drug discovery
- Chromatin organization and gene regulation
- Multiscale modeling

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
