---
layout: default
title: Events
description: Talks, seminars, and events hosted by the LION Lab.
permalink: /events/
---

{% include page-styles.html %}

<style>
  .event-card {
    padding: 2.5rem 0;
    border-bottom: 1px solid #e8dfd4;
  }

  .event-card:first-of-type {
    border-top: 1px solid #e8dfd4;
  }

  .event-meta-row {
    display: flex;
    align-items: baseline;
    gap: 1rem;
    flex-wrap: wrap;
    margin-bottom: 0.75rem;
  }

  .event-tag {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #fff;
    background: #DF6907;
    padding: 0.15rem 0.55rem;
  }

  .event-date {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.78rem;
    letter-spacing: 0.08em;
    color: #7a6a55;
  }

  .event-location {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.78rem;
    color: #a09080;
  }

  .event-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.4rem;
    font-weight: 400;
    color: #1a1209;
    line-height: 1.25;
    margin-bottom: 0.25rem;
  }

  .event-speaker {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.88rem;
    color: #DF6907;
    margin-bottom: 1.25rem;
  }

  .event-body {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.9rem;
    color: #3a2e20;
    line-height: 1.75;
    margin-bottom: 1rem;
  }

  .event-body a {
    color: #DF6907;
    text-decoration: none;
    border-bottom: 1px solid #DF6907;
    transition: opacity 0.2s;
  }

  .event-body a:hover { opacity: 0.7; }

  .event-abstract {
    border-left: 2px solid #e8dfd4;
    padding-left: 1.25rem;
    margin: 1.25rem 0;
  }

  .event-abstract-label {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #a09080;
    margin-bottom: 0.5rem;
  }

  .event-bio-label {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #a09080;
    margin-bottom: 0.5rem;
    margin-top: 1.25rem;
  }

  .mailing-list-block {
    background: #fdf8f0;
    border: 1px solid #e8dfd4;
    padding: 2rem 2.5rem;
    margin-bottom: 3rem;
  }

  .mailing-list-block p {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.92rem;
    color: #3a2e20;
    line-height: 1.7;
    margin: 0;
  }

  .mailing-list-block a {
    color: #DF6907;
    text-decoration: none;
    border-bottom: 1px solid #DF6907;
  }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Events</h1>
    <div class="lion-page-rule"></div>
  </div>

  <div class="mailing-list-block">
    <p>Sign up for our mailing list to be informed about future events:
      <a href="https://lists.uni-leipzig.de/mailman/listinfo/nlp-talks" target="_blank" rel="noopener">join the mailing list →</a>
    </p>
  </div>

  <!-- ── Event 1 ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Wednesday, 27 May 2025 · 13:00</span>
      <span class="event-location">Paulinum, Room P702 · Leipzig</span>
    </div>
    <h2 class="event-title">Implicit Misogyny and Classism in NLP</h2>
    <p class="event-speaker">Dr. Arianna Muti — Bocconi University, Milan</p>

    <p class="event-body">
      We're excited to welcome Arianna Muti for an invited talk on misogyny and classism in NLP.
      Lunch with the speaker at 11:30 in the mensa.
      Can't make it in person?
      <a href="https://docs.google.com/spreadsheets/d/1_H7D9hwJizNyzT1nWvZ3-NC_nhNr7LHtsuInynfEPS4/edit?usp=sharing" target="_blank" rel="noopener">Zoom link and 1-on-1 sign-ups here.</a>
    </p>

    <div class="event-abstract">
      <p class="event-abstract-label">Abstract</p>
      <p class="event-body" style="margin:0;">
        Implicit misogyny and classism are difficult for NLP systems because they are often conveyed indirectly, through presuppositions, stereotypes, and unstated assumptions rather than explicit hateful expressions. Arianna presents work on analysing these implicit forms of harm in social media — framing misogyny detection as an argumentative reasoning task, and introducing ACID, a resource for studying how lower-SES people are perceived across cultures.
      </p>
    </div>

    <p class="event-bio-label">Bio</p>
    <p class="event-body">
      <a href="https://milanlp.github.io/people/arianna-muti/" target="_blank" rel="noopener">Arianna Muti</a>
      is a Postdoctoral Research Fellow at Bocconi University, part of the MilaNLP group.
      Her research focuses on NLP with particular attention to detection and explanation of implicit misogyny and classism in social media. She is currently working on PERSONAE, developing identity-aware language technologies.
    </p>
  </div>

  <!-- ── Event 2 ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Tuesday, 19 May 2025 · 13:00</span>
      <span class="event-location">Paulinum, Room P702 · Leipzig</span>
    </div>
    <h2 class="event-title">What Is Discourse, and What Do LLMs Know About It?</h2>
    <p class="event-speaker">Prof. Yang Janet Liu — University of Pittsburgh</p>

    <p class="event-body">
      We're pleased to welcome Yang Janet Liu for a talk on discourse and LLM evaluation.
      Lunch with the speaker at 11:30 in the mensa; dinner at 18:00 (email Leonie by 15 May to join).
      <a href="https://docs.google.com/spreadsheets/d/1A0vJITBmVxFspPqbpbsmAEvZI9upun-55NqGcjeWKWU/edit?usp=sharing" target="_blank" rel="noopener">Zoom link and 1-on-1 sign-ups here.</a>
    </p>

    <div class="event-abstract">
      <p class="event-abstract-label">Abstract</p>
      <p class="event-body" style="margin:0;">
        As LLM-generated output becomes increasingly fluent, evaluating what they know and how reliably they generalise has become critical. At the discourse level, meaning is conveyed beyond single sentences, shaped by linguistic conventions, communicative goals, and variation in human interpretation. Janet presents work examining LLMs' grasp of discourse coherence, how breaking down model reasoning into discourse units can account for human label variation, and how incorporating discourse relations can improve faithfulness evaluation in long-form summarisation.
      </p>
    </div>

    <p class="event-bio-label">Bio</p>
    <p class="event-body">
      <a href="https://janetlauyeung.github.io/" target="_blank" rel="noopener">Yang Janet Liu</a>
      is an Assistant Professor in the Department of Linguistics at the University of Pittsburgh, with a secondary appointment in the Intelligent Systems Program. Her research focuses on computational approaches to discourse-level phenomena, LLM evaluation, and how pragmatic variation shapes language use and model behaviour. She earned her PhD from Georgetown University and was previously a postdoctoral researcher in the MaiNLP Lab at LMU Munich.
    </p>
  </div>

</div>