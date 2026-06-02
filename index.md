---
layout: default
title: Home
description: LION Lab — Linguistically-Oriented NLP research group at the University of Leipzig.
permalink: /
---

{% include page-styles.html %}

<style>
  /* ── About-specific ── */
  .about-intro {
    display: grid;
    grid-template-columns: 1fr 340px;
    gap: 5rem;
    align-items: start;
    margin-bottom: 4rem;
  }

  .about-logo-block {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.5rem;
  }

  .about-logo-placeholder {
    width: 220px;
    height: 220px;
    background: #DF6907;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 6rem;
    /* TODO: replace with <img src="/assets/images/logo.svg"> when logo is ready */
  }

  .about-social {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    justify-content: center;
  }

  .about-social a {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.72rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #7a6a55;
    text-decoration: none;
    border-bottom: 1px solid #c8b89a;
    padding-bottom: 1px;
    transition: color 0.2s, border-color 0.2s;
    display: flex;
    align-items: center;
    gap: 0.35rem;
  }

  .about-social a:hover {
    color: #DF6907;
    border-color: #DF6907;
  }

  /* News preview on homepage */
  .news-item {
    padding: 1.5rem 0;
    border-bottom: 1px solid #e8dfd4;
  }

  .news-item:first-child {
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
  }

  .funding-block a {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.95rem;
    color: #3a2e20;
    text-decoration: none;
    border-bottom: 1px solid #c8b89a;
    transition: color 0.2s;
  }

  .funding-block a:hover { color: #DF6907; }

  @media (max-width: 800px) {
    .about-intro {
      grid-template-columns: 1fr;
    }
    .about-logo-block {
      flex-direction: row;
      justify-content: flex-start;
    }
    .about-logo-placeholder {
      width: 100px;
      height: 100px;
      font-size: 3rem;
    }
  }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>LION Lab</h1>
    <div class="lion-page-rule"></div>
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
      <p>
        <!-- TODO: expand with research statement -->
      </p>
    </div>

    <div class="about-logo-block">
      <!-- TODO: replace with real logo -->
      <div class="about-logo-placeholder" aria-hidden="true">🦁</div>
      <div class="about-social">
        <a href="https://github.com/LionLabNLP/" target="_blank" rel="noopener">
          <!-- GitHub icon -->
          <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0024 12c0-6.63-5.37-12-12-12z"/></svg>
          GitHub
        </a>
        <a href="https://huggingface.co/LIONLab-NLP" target="_blank" rel="noopener">🤗 HuggingFace</a>
        <a href="https://x.com/LIONLabNLP" target="_blank" rel="noopener">
          <svg width="13" height="13" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-4.714-6.231-5.401 6.231H2.744l7.737-8.835L1.254 2.25H8.08l4.253 5.622zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
          X / Twitter
        </a>
        <a href="https://bsky.app/profile/lionlab.bsky.social" target="_blank" rel="noopener">Bluesky</a>
        <a href="https://www.linkedin.com/company/lion-lab-leipzig" target="_blank" rel="noopener">LinkedIn</a>
      </div>
    </div>
  </div>

  <hr class="lion-divider">

  <!-- News preview -->
  <p class="lion-section-label">Latest News</p>

  <div class="news-item">
    <p class="news-item-date">2026</p>
    <p class="news-item-title">Jacob presented three papers at LREC 2026</p>
    <p class="news-item-body">Including WikIPA, Fill-in-the-Blanks, and DiNoS (at the SLiDE Workshop).</p>
  </div>

  <div class="news-item">
    <p class="news-item-date">2026</p>
    <p class="news-item-title">New paper accepted at CoNLL 2026</p>
    <p class="news-item-body">Language Models Learn Constructional Semantics, Not To Mention Syntax — Wesley Scivetti et al.</p>
  </div>

  <div class="news-item">
    <p class="news-item-date">April 2026</p>
    <p class="news-item-title">Welcome, Jacob and Toshiki!</p>
    <p class="news-item-body">Jacob Lee Suchardt and Toshiki Nakai join the lab as PhD students.</p>
  </div>

  <a href="/news" class="see-all-link">All news →</a>

  <hr class="lion-divider">

  <!-- Funding -->
  <p class="lion-section-label">Funding</p>
  <div class="funding-block lion-prose">
    <p>We are grateful for support from
      <a href="https://scads.ai/" target="_blank" rel="noopener">ScaDS.AI Dresden/Leipzig</a>
      (Center for Scalable Data Analytics and Artificial Intelligence).
    </p>
    <!-- TODO: add further funders here -->
  </div>

</div>