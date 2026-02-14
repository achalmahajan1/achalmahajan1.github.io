---
layout: single
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
classes: wide
---

<style>
  .cv-timeline {
    position: relative;
    padding-left: 28px;
    margin-top: 12px;
    margin-bottom: 8px;
  }
  .cv-timeline-line {
    position: absolute;
    left: 5px;
    top: 6px;
    bottom: 0;
    width: 2px;
    background: var(--border, #e9ecef);
  }
  .cv-item {
    position: relative;
    margin-bottom: 20px;
  }
  .cv-item:last-child {
    margin-bottom: 10px;
  }
  .cv-dot {
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
  .cv-item:hover .cv-dot {
    transform: scale(1.3);
  }
  .cv-date {
    font-family: 'Barlow', sans-serif;
    font-weight: 400;
    font-size: 0.82em;
    color: var(--accent, #784e51);
  }
  .cv-role {
    font-family: 'Nunito Sans', sans-serif;
    font-weight: 600;
    color: var(--text, #333);
    font-size: 0.95em;
  }
  .cv-place {
    font-family: 'Barlow', sans-serif;
    font-weight: 300;
    color: var(--text-muted, #666);
    font-size: 0.9em;
    font-style: italic;
  }
  .cv-section-icon {
    color: var(--accent, #784e51) !important;
    margin-right: 8px;
  }
</style>

[PDF: Long Version](https://drive.google.com/file/d/1s6ccny89q8tg4Hj5qP1Q1OtdMJnd4mTE/view?usp=sharing){: .btn .btn--inverse .btn--small}
[PDF: Short Version](https://drive.google.com/file/d/1PAn-iX0LTCsofbQeFbrlLfbrIOFKlpog/view?usp=sharing){: .btn .btn--inverse .btn--small}

<h2><i class="fas fa-graduation-cap cv-section-icon"></i>Education</h2>

<div class="cv-timeline fade-in-section">
  <div class="cv-timeline-line"></div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">2021</div>
    <div class="cv-role">Ph.D. (Engineering Physics)</div>
    <div class="cv-place">University of California, San Diego</div>
  </div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">2016</div>
    <div class="cv-role">M.S. (Engineering Mechanics)</div>
    <div class="cv-place">Jawaharlal Nehru Centre for Advanced Scientific Research, Bangalore</div>
  </div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">2013</div>
    <div class="cv-role">B.Tech. (Chemical Engineering)</div>
    <div class="cv-place">National Institute of Technology Karnataka Surathkal</div>
  </div>
</div>

<h2><i class="fas fa-briefcase cv-section-icon"></i>Work Experience</h2>

<div class="cv-timeline fade-in-section">
  <div class="cv-timeline-line"></div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">Oct 2022 – Present</div>
    <div class="cv-role">Scientist II</div>
    <div class="cv-place">Altos Labs</div>
  </div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">Jan 2022 – Sept 2022</div>
    <div class="cv-role">Senior Application Engineer</div>
    <div class="cv-place">MathWorks</div>
  </div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">2016 – 2021</div>
    <div class="cv-role">Graduate Student Researcher</div>
    <div class="cv-place">University of California, San Diego</div>
  </div>

  <div class="cv-item">
    <div class="cv-dot"></div>
    <div class="cv-date">2013 – 2016</div>
    <div class="cv-role">Graduate Research Assistant</div>
    <div class="cv-place">Jawaharlal Nehru Centre for Advanced Scientific Research, Bangalore</div>
  </div>
</div>


<h2><i class="fas fa-chalkboard-teacher cv-section-icon"></i>Academic Service</h2>

<style>
  /* ---- Academic Service Cards ---- */
  .service-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 16px;
    margin-top: 14px;
  }
  .service-card {
    padding: 18px 20px;
    border-left: 3px solid var(--accent, #784e51);
    border-radius: 4px;
    background: var(--card-bg, #fdfdfd);
    transition: background 0.2s ease, box-shadow 0.2s ease;
  }
  .service-card:hover {
    background: var(--card-hover, #f7f4f4);
    box-shadow: 0 2px 8px var(--card-shadow, rgba(120, 78, 81, 0.08));
  }
  .service-card-header {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 12px;
  }
  .service-card-icon {
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--accent, #784e51), #a0696c);
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.85em;
    flex-shrink: 0;
  }
  .service-card-title {
    font-family: 'Nunito Sans', sans-serif;
    font-weight: 600;
    color: var(--heading, #893636);
    font-size: 1.02em;
  }
  .service-venues {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }
  .service-venue {
    display: inline-flex;
    align-items: center;
    gap: 5px;
    padding: 5px 12px;
    border-radius: 20px;
    background: var(--bg-secondary, #f8f9fa);
    border: 1px solid var(--border, #e9ecef);
    font-family: 'Nunito Sans', sans-serif;
    font-size: 0.82em;
    font-weight: 500;
    color: var(--text, #333);
    transition: border-color 0.2s ease, background 0.2s ease;
  }
  .service-venue:hover {
    border-color: var(--accent, #784e51);
    background: var(--card-hover, #f7f4f4);
  }
  .service-venue-year {
    font-family: 'Barlow', sans-serif;
    font-weight: 400;
    font-size: 0.9em;
    color: var(--text-muted, #888);
  }

  /* dark mode adjustments */
  [data-theme="dark"] .service-card-icon {
    background: linear-gradient(135deg, #c17e82, #a0696c);
  }

  @media (max-width: 600px) {
    .service-venue {
      font-size: 0.78em;
      padding: 4px 10px;
    }
  }
</style>

<div class="service-grid fade-in-section">

  <div class="service-card">
    <div class="service-card-header">
      <div class="service-card-icon"><i class="fas fa-search"></i></div>
      <div class="service-card-title">Reviewer</div>
    </div>
    <div class="service-venues">
      <span class="service-venue">Physical Review Fluids <span class="service-venue-year">2023</span></span>
      <span class="service-venue">New Journal of Physics <span class="service-venue-year">2023</span></span>
      <span class="service-venue">ACM-BCB <span class="service-venue-year">2023</span></span>
      <span class="service-venue">IEEE-BIBM <span class="service-venue-year">2023, 2024</span></span>
      <span class="service-venue">Scientific Reports <span class="service-venue-year">2023</span></span>
      <span class="service-venue">NeurIPS-AI4D3 <span class="service-venue-year">2023</span></span>
      <span class="service-venue">AAAI-W3PHIAI <span class="service-venue-year">2024</span></span>
      <span class="service-venue">ISMB <span class="service-venue-year">2024</span></span>
    </div>
  </div>

  <div class="service-card">
    <div class="service-card-header">
      <div class="service-card-icon"><i class="fas fa-users-cog"></i></div>
      <div class="service-card-title">Program Chair</div>
    </div>
    <div class="service-venues">
      <span class="service-venue">IEEE-BIBM <span class="service-venue-year">2023, 2024</span></span>
      <span class="service-venue">AAAI-W3PHIAI <span class="service-venue-year">2024</span></span>
      <span class="service-venue">ISMB <span class="service-venue-year">2024</span></span>
    </div>
  </div>

</div>
