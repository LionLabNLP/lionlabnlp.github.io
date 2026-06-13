---
layout: default
title: Home
description: LION Lab — Linguistically-Oriented NLP research group at the University of Leipzig.
permalink: /
---

{% include page-styles.html %}

<style>
  /* ── About-specific ── */
  .about-hero {
    display: flex;
    align-items: center;
    gap: 2.5rem;
    margin-bottom: 3rem;
  }

  .about-hero-logo {
    width: 160px;
    flex-shrink: 0;
  }

  .about-hero-logo img {
    width: 100%;
    height: auto;
    display: block;
  }

  .about-hero-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: clamp(2.2rem, 5vw, 3.8rem);
    font-weight: 400;
    color: #1a1209;
    letter-spacing: -0.01em;
    line-height: 1;
    margin: 0 0 1rem;
  }

  .about-intro {
    display: grid;
    grid-template-columns: 1fr 200px;
    gap: 5rem;
    align-items: start;
    margin-bottom: 4rem;
  }

  /* Social links — stacked column */
  .about-social {
    display: flex;
    flex-direction: column;
    gap: 0.65rem;
  }

  .about-social a {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.82rem;
    letter-spacing: 0.06em;
    color: #3a2e20;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 0.6rem;
    transition: color 0.2s;
  }

  .about-social a:hover {
    color: #DF6907;
  }

  .about-social img {
    width: 18px;
    height: 18px;
    object-fit: contain;
    flex-shrink: 0;
    opacity: 0.75;
  }

  .about-social a:hover img {
    opacity: 1;
  }

  /* News preview */
  .news-item {
    padding: 1.5rem 0;
    border-bottom: 1px solid #e8dfd4;
  }

  .news-item:first-of-type {
    border-top: 1px solid #e8dfd4;
  }

  .news-item-date {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.72rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #DF6907;
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
    color: #DF6907;
    text-decoration: none;
    border-bottom: 1px solid #DF6907;
    transition: opacity 0.2s;
  }

  .news-item-body a:hover { opacity: 0.7; }

  .see-all-link {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.82rem;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    color: #DF6907;
    text-decoration: none;
    border-bottom: 1px solid #DF6907;
    margin-top: 1.5rem;
    display: inline-block;
    transition: opacity 0.2s;
  }

  .see-all-link:hover { opacity: 0.7; }

  /* Funding */
  .funding-block {
    margin-top: 1.5rem;
    display: flex;
    align-items: center;
    gap: 2rem;
    flex-wrap: wrap;
  }

  .funding-block p {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.92rem;
    color: #3a2e20;
    line-height: 1.7;
    margin: 0;
  }

  .funding-block a {
    color: #3a2e20;
    text-decoration: none;
    border-bottom: 1px solid #c8b89a;
    transition: color 0.2s;
  }

  .funding-block a:hover { color: #DF6907; }

  .funding-logo {
    height: 48px;
    width: auto;
    display: block;
    flex-shrink: 0;
  }

  @media (max-width: 800px) {
    .about-hero {
      flex-direction: column;
      align-items: flex-start;
      gap: 1.5rem;
    }
    .about-hero-logo { width: 100px; }
    .about-intro {
      grid-template-columns: 1fr;
      gap: 2rem;
    }
  }
</style>

<div class="lion-page">

  <!-- Hero: logo + title -->
  <div class="about-hero">
    <div class="about-hero-logo">
      <img src="{{ '/assets/img/logos/lion_lab.svg' | relative_url }}" alt="LION Lab">
    </div>
    <div>
      <h1 class="about-hero-title">LION Lab</h1>
      <div class="lion-page-rule"></div>
    </div>
  </div>

  <div class="about-intro">
    <div class="lion-prose">
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
        X / Twitter
      </a>
      <a href="https://bsky.app/profile/lionlab.bsky.social" target="_blank" rel="noopener">
        <img src="{{ '/assets/img/logos/bluesky.svg' | relative_url }}" alt="">
        Bluesky
      </a>
      <a href="https://www.linkedin.com/company/lion-lab-leipzig" target="_blank" rel="noopener">
        <img src="{{ '/assets/img/logos/linkedin.png' | relative_url }}" alt="">
        LinkedIn
      </a>
    </div>
  </div>

  <hr class="lion-divider">

  <!-- News preview: auto-pulls first 5 items from _data/news.yml -->
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
      <img class="funding-logo" src="{{ '/assets/img/logos/scads_rgb.png' | relative_url }}" alt="ScaDS.AI Dresden/Leipzig">
    </a>
    <p>We are grateful for support from
      <a href="https://scads.ai/" target="_blank" rel="noopener">ScaDS.AI Dresden/Leipzig</a>
      (Center for Scalable Data Analytics and Artificial Intelligence).
      <!-- TODO: add further funders here in the same format -->
    </p>
  </div>

</div>