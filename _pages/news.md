---
layout: default
title: News
description: Latest news from the LION Lab.
permalink: /news/
---

{% include page-styles.html %}

<style>
  .news-entry {
    display: grid;
    grid-template-columns: 120px 1fr;
    gap: 2rem;
    padding: 2rem 0;
    border-bottom: 1px solid #e8dfd4;
  }

  .news-entry:first-of-type {
    border-top: 1px solid #e8dfd4;
  }

  .news-entry-date {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.75rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #DF6907;
    padding-top: 0.2rem;
  }

  .news-entry-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.15rem;
    font-weight: 400;
    color: #1a1209;
    margin-bottom: 0.5rem;
  }

  .news-entry-body {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.9rem;
    color: #3a2e20;
    line-height: 1.7;
  }

  .news-entry-body a {
    color: #DF6907;
    text-decoration: none;
    border-bottom: 1px solid #DF6907;
    transition: opacity 0.2s;
  }

  .news-entry-body a:hover { opacity: 0.7; }

  @media (max-width: 600px) {
    .news-entry { grid-template-columns: 1fr; gap: 0.5rem; }
  }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>News</h1>
    <div class="lion-page-rule"></div>
  </div>

  <div class="news-entry">
    <p class="news-entry-date">2026</p>
    <div>
      <p class="news-entry-title">Jacob presented three papers at LREC 2026</p>
      <p class="news-entry-body">
        Jacob presented at LREC 2026, including
        <a href="https://lrec.elra.info/lrec2026-main-668" target="_blank" rel="noopener">WikIPA: Integrating WikiPron and Lingua Libre for Multilingual IPA Transcription</a>,
        <a href="https://lrec.elra.info/lrec2026-main-090" target="_blank" rel="noopener">Fill-in-the-Blanks: Automatic Generation and Evaluation of Language Models' Pseudonyms for English and Swedish Texts</a>,
        and <a href="https://pustejovsky.github.io/slide-lrec2026/book.pdf#page=205" target="_blank" rel="noopener">DiNoS: Creating a Data-Driven German Noun Phrase Lexicon from Universal Dependencies</a>
        (with Ronja Laarmann-Quante) at the <a href="https://www.slide-workshop.org/index.html" target="_blank" rel="noopener">SLiDE Workshop</a>.
      </p>
    </div>
  </div>

  <div class="news-entry">
    <p class="news-entry-date">2026</p>
    <div>
      <p class="news-entry-title">New paper accepted at CoNLL 2026</p>
      <p class="news-entry-body">
        <a href="https://openreview.net/forum?id=97IvVs7z5c" target="_blank" rel="noopener">Language Models Learn Constructional Semantics, Not To Mention Syntax</a>
        by Wesley Scivetti, Ethan Gotlieb Wilcox, Nathan Schneider, Kanishka Misra, and Leonie Weissweiler
        has been accepted at the 30th Conference on Computational Natural Language Learning.
      </p>
    </div>
  </div>

  <div class="news-entry">
    <p class="news-entry-date">April 2026</p>
    <div>
      <p class="news-entry-title">Welcome, Jacob and Toshiki!</p>
      <p class="news-entry-body">Jacob Lee Suchardt and Toshiki Nakai join the lab as PhD students. Welcome to both!</p>
    </div>
  </div>

</div>