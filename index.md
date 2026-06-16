---
layout: default
title: Home
description: LION Lab — Linguistically-Oriented NLP research group at the University of Leipzig.
permalink: /
---

{% include page-styles.html %}

<style>
  /* ── Hero: big logo left, group photo right ── */
  .about-hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
    margin-bottom: 3rem;
  }

  .about-hero-left {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 2rem;
  }

  .about-hero-logo img {
    width: 100%;
    max-width: 690px;
    height: auto;
    aspect-ratio: 5250 / 2000;
    display: block;
  }

  /* Social links — single horizontal row */
  .about-social {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 1.25rem 2rem;
    align-items: center;
  }

  .about-social a {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.82rem;
    letter-spacing: 0.06em;
    color: #3a2e20;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 0.5rem;
    transition: color 0.2s;
  }

  .about-social a:hover { color: #E26600; }

  .about-social img {
    width: 20px;
    height: 20px;
    object-fit: contain;
    flex-shrink: 0;
    opacity: 0.7;
  }

  .about-social a:hover img { opacity: 1; }

  /* Group photo with corner bracket decoration (matches team page PI photo) */
  .about-group-wrap {
    position: relative;
  }

  .about-group-photo {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  .about-group-wrap::before {
    content: '';
    position: absolute;
    top: -8px;
    left: -8px;
    width: 32px;
    height: 32px;
    border-top: 3px solid #E26600;
    border-left: 3px solid #E26600;
    z-index: 1;
  }

  .about-group-wrap::after {
    content: '';
    position: absolute;
    bottom: -8px;
    right: -8px;
    width: 32px;
    height: 32px;
    border-bottom: 3px solid #E26600;
    border-right: 3px solid #E26600;
    z-index: 1;
  }

  /* Body text below hero */
  .about-body {
    margin-bottom: 4rem;
  }

  /* News preview */
  .news-item {
    padding: 1.5rem 0;
    border-bottom: 1px solid #f0e4d4;
  }

  .news-item:first-of-type { border-top: 1px solid #f0e4d4; }

  .news-item-date {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.72rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #E26600;
    margin-bottom: 0.3rem;
  }

  .news-item-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.05rem;
    font-weight: 400;
    color: #1a1209;
    margin-bottom: 0.3rem;
  }

  .news-item-body {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.88rem;
    color: #3a2e20;
    line-height: 1.65;
  }

  .news-item-body a {
    color: #E26600;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
    transition: opacity 0.2s;
  }

  .news-item-body a:hover { opacity: 0.7; }

  .see-all-link {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.82rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: #E26600;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
    margin-top: 1.5rem;
    display: inline-block;
    transition: opacity 0.2s;
  }

  .see-all-link:hover { opacity: 0.7; }

  /* Funding */
  .funding-block {
    margin-top: 1.5rem;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 2.5rem;
    flex-wrap: wrap;
  }

  .funding-block p {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.92rem;
    color: #3a2e20;
    line-height: 1.7;
    margin: 0;
    flex: 1;
    min-width: 200px;
  }

  .funding-block a {
    color: #E26600;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
    transition: opacity 0.2s;
  }

  .funding-block a:hover { opacity: 0.7; }

  .funding-logo {
    height: 200px;
    width: auto;
    display: block;
    flex-shrink: 0;
  }

  @media (max-width: 800px) {
    .about-hero {
      grid-template-columns: 1fr;
    }
    .about-hero-logo img { max-width: 384px; }
    .funding-logo { height: 100px; }
  }
</style>

<div class="lion-page">

  <!-- Hero -->
  <div class="about-hero">
    <div class="about-hero-left">
      <div class="about-hero-logo">
        <img src="{{ '/assets/img/logos/lionlablogo-full-transparent.svg' | relative_url }}" alt="LION Lab">
      </div>
      <div class="about-social">
        <a href="https://github.com/LionLabNLP/" target="_blank" rel="noopener">
          <img src="{{ '/assets/img/logos/github.svg' | relative_url }}" alt="">
          GitHub
        </a>
        <a href="https://huggingface.co/LIONLab-NLP" target="_blank" rel="noopener">
          <img src="{{ '/assets/img/logos/huggingface.svg' | relative_url }}" alt="">
          Hugging Face
        </a>
        <a href="https://x.com/LIONLabNLP" target="_blank" rel="noopener">
          <img src="{{ '/assets/img/logos/twitter.svg' | relative_url }}" alt="">
          X
        </a>
        <a href="https://bsky.app/profile/lionlab.bsky.social" target="_blank" rel="noopener">
          <img src="{{ '/assets/img/logos/bluesky.svg' | relative_url }}" alt="">
          Bluesky
        </a>
        <a href="https://www.linkedin.com/company/lionlabnlp" target="_blank" rel="noopener">
          <img src="{{ '/assets/img/logos/linkedin.png' | relative_url }}" alt="">
          LinkedIn
        </a>
      </div>
    </div>
    <div class="about-group-wrap">
      <img class="about-group-photo"
           src="{{ '/assets/img/members/group_cropped.JPG' | relative_url }}"
           alt="LION Lab group photo">
    </div>
  </div>

  <!-- Intro text -->
  <div class="about-body lion-prose">
    <p>
      We are a research group at the
      <a href="https://www.informatik.uni-leipzig.de/" target="_blank" rel="noopener">Department of Computer Science</a>
      at <a href="https://www.uni-leipzig.de/" target="_blank" rel="noopener">Leipzig University</a>, Germany,
      led by <a href="https://leonieweissweiler.github.io/" target="_blank" rel="noopener">Jun.-Prof. Dr. Leonie Weissweiler</a>.
    </p>
    <p>
      We work on linguistically-oriented natural language processing — asking what language
      models actually learn about the structure of language, and using insights from linguistic
      theory to build better, more interpretable NLP systems.
    </p>
    <!-- TODO: expand with research statement -->
  </div>

  <hr class="lion-divider">

  <!-- News preview -->
  <p class="lion-section-label">Latest News</p>

  {% for item in site.data.news limit:5 %}
  <div class="news-item">
    <p class="news-item-date">{{ item.date }}</p>
    <p class="news-item-title">{{ item.title }}</p>
    <p class="news-item-body">{{ item.body }}</p>
  </div>
  {% endfor %}

  <a href="/news" class="see-all-link">All news →</a>

  <hr class="lion-divider">

  <!-- Funding -->
  <p class="lion-section-label">Funding</p>
  <div class="funding-block">
    <a href="https://scads.ai/" target="_blank" rel="noopener">
      <img class="funding-logo"
           src="{{ '/assets/img/logos/scads_rgb.png' | relative_url }}"
           alt="ScaDS.AI Dresden/Leipzig">
    </a>
    <p>We are grateful for support from
      <a href="https://scads.ai/" target="_blank" rel="noopener">ScaDS.AI Dresden/Leipzig</a>
      (Center for Scalable Data Analytics and Artificial Intelligence).
      <!-- TODO: add further funders here -->
    </p>
  </div>

</div>