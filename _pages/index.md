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

{% assign displayed_count = 0 %}
{% for news in site.data.news %}
  {% if news.text != nil and news.text != "" and displayed_count < 5 %}
<div style="margin-bottom: 14px; padding-bottom: 14px; border-bottom: 1px solid #e9ecef;">
  <span style="color: #784e51; font-size: 0.85em; font-family: 'Barlow', sans-serif; font-weight: 400;">{{ news.date }}</span>
  <div style="margin-top: 3px; font-family: 'Nunito Sans', sans-serif; font-weight: 300; color: #555; font-size: 0.95em; line-height: 1.5;">
    {{ news.text | markdownify | remove: '<p>' | remove: '</p>' }}
  </div>
</div>
    {% assign displayed_count = displayed_count | plus: 1 %}
  {% endif %}
{% endfor %}
