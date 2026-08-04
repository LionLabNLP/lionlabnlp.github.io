---
layout: default
title: Job Posting Template
description: Template for job postings — not published.
permalink: /jobs/template/
published: false
noindex: true
sitemap: false
---

{% comment %}
  ── How to use this template ──

  1. Copy this file to _pages/jobs/<short-name>.md
  2. Edit the front matter:
       title / description  — shown in the browser tab and search results
       permalink            — the public URL, e.g. /jobs/postdoc-2027/
       published            — DELETE this line (`published: false` hides the page entirely)
       noindex / sitemap    — keep both while the posting is unannounced; delete
                              them once it goes live so search engines pick it up
  3. Fill in the sections below. Drop any that don't apply.
  4. To announce it, link the page from _pages/join-us.md (and _data/news.yml).

  A page with `noindex`/`sitemap: false` still builds and is reachable by URL —
  it's just not linked from the site or indexed. That's the "ready but not live"
  state. `published: false` is stronger: the page isn't built at all.
{% endcomment %}

{% include page-styles.html %}
{% include job-styles.html %}

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Position Title</h1>
    <div class="lion-page-rule"></div>
  </div>

  <div class="lion-prose" style="margin-bottom: 2rem;">
    <p>
      One-paragraph summary: how many positions, what field, which institute,
      and whose group.
    </p>
  </div>

  <div class="job-facts">
    <div class="job-fact">
      <span class="job-fact-label">Preferred start</span>
      <span class="job-fact-value">Date (later possible)</span>
    </div>
    <div class="job-fact">
      <span class="job-fact-label">Deadline</span>
      <span class="job-fact-value">Date (after that, open until filled)</span>
    </div>
    <div class="job-fact">
      <span class="job-fact-label">Positions</span>
      <span class="job-fact-value">Full-time (TV-L E13) for N years</span>
    </div>
  </div>

  <div class="job-section">
    <h2 class="lion-h2">Topics</h2>
    <div class="lion-prose">
      <p>What the successful candidate would work on.</p>
    </div>
  </div>

  <div class="job-section">
    <h2 class="lion-h2">Funding</h2>
    <div class="lion-prose">
      <p>Pay scale, duration, and any teaching obligations.</p>
    </div>
  </div>

  <div class="job-section">
    <h2 class="lion-h2">Candidates</h2>
    <div class="lion-prose">
      <p>Required and desirable background.</p>
    </div>
  </div>

  <div class="job-section">
    <h2 class="lion-h2">Location</h2>
    <div class="lion-prose">
      <p>Leipzig University, the institute, and the city.</p>
    </div>
  </div>

  <hr class="lion-divider">

  <div class="job-section job-apply">
    <h2 class="lion-h2">Application</h2>
    <div class="lion-prose">
      <p>
        What to send, where to send it, and which subject line to use.
      </p>
    </div>
  </div>

</div>
