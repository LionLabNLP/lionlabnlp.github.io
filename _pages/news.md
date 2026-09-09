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
    grid-template-columns: 110px 1fr 120px;
    column-gap: 0.85rem;
    align-items: center;
    padding: 2rem 0;
    border-bottom: 1px solid #f0e4d4;
  }

  .news-entry:first-of-type {
    border-top: 1px solid #f0e4d4;
  }

  .news-entry-date {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.75rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #E26600;
    padding-top: 0.2rem;
    align-self: start;
  }

  .news-entry-text { align-self: start; }

  /* Optional picture, cropped to a uniform square and centred against the text.
     The extra margin makes up the gap the tight date column gives away. */
  .news-entry-photo {
    width: 120px;
    height: 120px;
    object-fit: cover;
    object-position: center 30%;
    display: block;
    margin-left: 1.15rem;
  }

  .news-entry-title {
    font-family: var(--lion-heading-font);
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
    .news-entry { grid-template-columns: 1fr; row-gap: 0.5rem; }
    .news-entry-photo { margin-left: 0; }
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
    <div class="news-entry-text">
      <p class="news-entry-title">{{ item.title }}</p>
      <p class="news-entry-body">{{ item.body }}</p>
    </div>
    {% if item.image %}
    <img class="news-entry-photo"
         src="{{ item.image | relative_url }}"
         alt="{{ item.image_alt | default: item.title | strip_html }}"
         loading="lazy">
    {% endif %}
  </div>
  {% endfor %}

</div>