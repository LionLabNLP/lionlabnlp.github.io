---
layout: default
title: Team
description: Meet the LION Lab team.
permalink: /team/
---

<style>
  .team-page {
    max-width: 1100px;
    margin: 0 auto;
    padding: 5rem 2.5rem 7rem;
  }

  /* ── Header ── */
  .team-header {
    margin-bottom: 5rem;
  }

  .team-header h1 {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: clamp(2.8rem, 6vw, 4.5rem);
    font-weight: 400;
    color: #1a1209;
    letter-spacing: -0.01em;
    line-height: 1;
    margin: 0 0 1.25rem;
  }

  .team-rule {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .team-rule-bar {
    width: 3rem;
    height: 3px;
    background: #DF6907;
    flex-shrink: 0;
  }

  .team-rule-label {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.75rem;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #DF6907;
  }

  /* ── PI Section ── */
  .pi-section {
    display: grid;
    grid-template-columns: 280px 1fr;
    gap: 4rem;
    align-items: start;
    padding-bottom: 4rem;
    margin-bottom: 4rem;
    border-bottom: 1px solid #e8dfd4;
  }

  .pi-photo-wrap {
    position: relative;
  }

  .pi-photo-wrap img {
    width: 100%;
    aspect-ratio: 1;
    object-fit: cover;
    display: block;
  }

  .pi-photo-wrap::before {
    content: '';
    position: absolute;
    top: -8px;
    left: -8px;
    width: 32px;
    height: 32px;
    border-top: 3px solid #DF6907;
    border-left: 3px solid #DF6907;
  }

  .pi-photo-wrap::after {
    content: '';
    position: absolute;
    bottom: -8px;
    right: -8px;
    width: 32px;
    height: 32px;
    border-bottom: 3px solid #DF6907;
    border-right: 3px solid #DF6907;
  }

  .pi-info {
    padding-top: 0.5rem;
  }

  .pi-role {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.72rem;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #DF6907;
    margin-bottom: 0.75rem;
  }

  .pi-name {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 2rem;
    font-weight: 400;
    color: #1a1209;
    line-height: 1.15;
    margin-bottom: 0.6rem;
  }

  .pi-name a {
    color: inherit;
    text-decoration: none;
    border-bottom: 1.5px solid #DF6907;
    transition: color 0.2s;
  }

  .pi-name a:hover {
    color: #DF6907;
  }

  .pi-email {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.82rem;
    color: #7a6a55;
    margin-bottom: 1.75rem;
    letter-spacing: 0.01em;
  }

  .pi-email a {
    color: inherit;
    text-decoration: none;
    border-bottom: 1px solid #c8b89a;
    transition: color 0.2s, border-color 0.2s;
  }

  .pi-email a:hover {
    color: #DF6907;
    border-color: #DF6907;
  }

  /* ── Shared list style ── */
  .member-details {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
  }

  .member-details li {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.95rem;
    color: #3a2e20;
    line-height: 1.5;
    padding-left: 1.1rem;
    position: relative;
  }

  .member-details li::before {
    content: '—';
    position: absolute;
    left: 0;
    color: #DF6907;
    font-size: 0.8rem;
    top: 0.1em;
  }

  /* ── PhD Section ── */
  .phd-heading {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.72rem;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #DF6907;
    margin-bottom: 2.5rem;
  }

  .phd-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0;
  }

  .phd-card {
    padding: 0 3rem 0 0;
    border-right: 1px solid #e8dfd4;
  }

  .phd-card:last-child {
    padding: 0 0 0 3rem;
    border-right: none;
  }

  .phd-photo {
    width: 150px;
    height: 150px;
    object-fit: cover;
    margin-bottom: 1.5rem;
    display: block;
  }

  .phd-name {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.35rem;
    font-weight: 400;
    color: #1a1209;
    line-height: 1.2;
    margin-bottom: 0.25rem;
  }

  .phd-role {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.7rem;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: #DF6907;
    margin-bottom: 0.4rem;
  }

  .phd-since {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.78rem;
    color: #a09080;
    margin-bottom: 0.5rem;
  }

  .phd-email {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.8rem;
    color: #7a6a55;
    margin-bottom: 1.5rem;
  }

  .phd-email a {
    color: inherit;
    text-decoration: none;
    border-bottom: 1px solid #c8b89a;
    transition: color 0.2s, border-color 0.2s;
  }

  .phd-email a:hover {
    color: #DF6907;
    border-color: #DF6907;
  }

  .phd-card .member-details li {
    font-size: 0.875rem;
  }

  .phd-card .member-details li::before {
    color: #c8b89a;
  }

  /* ── Responsive ── */
  @media (max-width: 700px) {
    .pi-section {
      grid-template-columns: 1fr;
      gap: 2rem;
    }

    .pi-photo-wrap {
      max-width: 220px;
    }

    .phd-grid {
      grid-template-columns: 1fr;
    }

    .phd-card,
    .phd-card:last-child {
      padding: 2rem 0;
      border-right: none;
      border-bottom: 1px solid #e8dfd4;
    }

    .phd-card:last-child {
      border-bottom: none;
    }
  }
</style>

<div class="team-page">

  <div class="team-header">
    <h1>Team</h1>
    <div class="team-rule">
      <div class="team-rule-bar"></div>
      <span class="team-rule-label">Linguistically-Oriented NLP</span>
    </div>
  </div>

  <!-- PI -->
  <div class="pi-section">
    <div class="pi-photo-wrap">
      <img src="{{ '/assets/img/leonie.png' | relative_url }}" alt="Leonie Weissweiler">
    </div>
    <div class="pi-info">
      <p class="pi-role">Principal Investigator</p>
      <h2 class="pi-name">
        <a href="https://leonieweissweiler.github.io/" target="_blank" rel="noopener">Jun.-Prof. Dr.<br>Leonie Weissweiler</a>
      </h2>
      <p class="pi-email"><a href="mailto:leonie.weissweiler@uni-leipzig.de">leonie.weissweiler@uni-leipzig.de</a></p>
      <ul class="member-details">
        <li>Juniorprofessor (~Assistant Professor) at the University of Leipzig</li>
        <li>PhD in Computational Linguistics from LMU Munich</li>
        <li>Research at the intersection of linguistic theory and NLP</li>
        <li>Computational linguistics &amp; language models</li>
      </ul>
    </div>
  </div>

  <!-- PhD Students -->
  <p class="phd-heading">PhD Students</p>
  <div class="phd-grid">

    <div class="phd-card">
      <img class="phd-photo" src="{{ '/assets/img/jacob.png' | relative_url }}" alt="Jacob Lee Suchardt">
      <h3 class="phd-name"><a href="https://scholar.google.com/citations?user=S4YThOIAAAAJ&hl=en&oi=ao" target="_blank" rel="noopener">Jacob Lee Suchardt M.Sc.</a></h3>
      <p class="phd-role">PhD Student</p>
      <p class="phd-since">Since April 2026</p>
      <p class="phd-email"><a href="mailto:jacob.suchardt@uni-leipzig.de">jacob.suchardt@uni-leipzig.de</a></p>
      <ul class="member-details">
        <li>Bio placeholder</li>
        <li>Research topic placeholder</li>
        <li>Methods / focus placeholder</li>
      </ul>
    </div>

    <div class="phd-card">
      <img class="phd-photo" src="{{ '/assets/img/toshiki.jpg' | relative_url }}" alt="Toshiki Nakai">
      <h3 class="phd-name"><a href="https://scholar.google.com/citations?hl=en&user=gKPYpYQAAAAJ" target="_blank" rel="noopener">Toshiki Nakai M.Sc.</a></h3>
      <p class="phd-role">PhD Student</p>
      <p class="phd-since">Since April 2026</p>
      <p class="phd-email"><a href="mailto:toshiki.nakai@uni-leipzig.de">toshiki.nakai@uni-leipzig.de</a></p>
      <ul class="member-details">
        <li>Bio placeholder</li>
        <li>Research topic placeholder</li>
        <li>Methods / focus placeholder</li>
      </ul>
    </div>

  </div>

</div>