---
layout: default
title: Contact
description: Contact the LION Lab at Leipzig University.
permalink: /contact/
---

{% include page-styles.html %}

<style>
  .contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
  }

  .contact-block h2 {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.3rem;
    font-weight: 400;
    color: #1a1209;
    margin-bottom: 1.25rem;
  }

  .contact-detail {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.9rem;
    color: #3a2e20;
    line-height: 2;
  }

  .contact-detail a {
    color: #3a2e20;
    text-decoration: none;
    border-bottom: 1px solid #f0d4b0;
    transition: color 0.2s, border-color 0.2s;
  }

  .contact-detail a:hover {
    color: #E26600;
    border-color: #E26600;
  }

  .contact-label {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #a09080;
    margin-bottom: 0.25rem;
    margin-top: 1rem;
  }

  @media (max-width: 700px) {
    .contact-grid {
      grid-template-columns: 1fr;
      gap: 3rem;
    }
  }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Contact</h1>
    <div class="lion-page-rule"></div>
  </div>

  <div class="contact-grid">

    <div class="contact-block">
      <h2>Jun.-Prof. Dr. Leonie Weißweiler</h2>
      <p class="contact-detail">
        Fakultät für Mathematik und Informatik<br>
        Institut für Informatik<br>
        Augustusplatz 10<br>
        04109 Leipzig<br>
        Room P816
      </p>
      <p class="contact-label">Phone</p>
      <p class="contact-detail">+49 341 97 32382</p>
      <p class="contact-label">Email</p>
      <p class="contact-detail"><a href="mailto:leonie.weissweiler@uni-leipzig.de">leonie.weissweiler@uni-leipzig.de</a></p>
      <p class="contact-label">Website</p>
      <p class="contact-detail"><a href="https://leonieweissweiler.github.io/" target="_blank" rel="noopener">leonieweissweiler.github.io</a></p>
    </div>

    <div class="contact-block">
      <h2>Sekretariat</h2>
      <p class="contact-detail">
        Petra Gamrath<br>
        Room P825
      </p>
      <p class="contact-label">Phone</p>
      <p class="contact-detail">+49 341 9732230</p>
      <p class="contact-label">Email</p>
      <p class="contact-detail"><a href="mailto:petra.gamrath@uni-leipzig.de">petra.gamrath@uni-leipzig.de</a></p>
    </div>

  </div>

</div>