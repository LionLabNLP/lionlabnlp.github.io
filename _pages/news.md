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
    border-bottom: 1px solid #f0e4d4;
  }

  .news-entry:first-of-type {
    border-top: 1px solid #f0e4d4;
  }

  .news-entry-date {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.75rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #E26600;
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
    color: #E26600;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
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

  {% for item in site.data.news %}
  <div class="news-entry">
    <p class="news-entry-date">{{ item.date }}</p>
    <div>
      <p class="news-entry-title">{{ item.title }}</p>
      <p class="news-entry-body">{{ item.body }}</p>
    </div>
  </div>
  {% endfor %}

</div>