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
    border-bottom: 1px solid var(--lion-border);
  }

  .event-card:first-of-type { border-top: 1px solid var(--lion-border); }

  .event-meta-row {
    display: flex;
    align-items: baseline;
    gap: 1rem;
    flex-wrap: wrap;
    margin-bottom: 0.75rem;
  }

  .event-tag {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #fff;
    background: var(--lion-dark);
    padding: 0.15rem 0.55rem;
    flex-shrink: 0;
  }


  .event-tag-lab {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--lion-dark);
    background: transparent;
    border: 1.5px solid var(--lion-dark);
    padding: 0.15rem 0.55rem;
    flex-shrink: 0;
  }

  .event-date {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.78rem;
    letter-spacing: 0.08em;
    color: var(--lion-muted);
  }

  .event-location {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.78rem;
    color: var(--lion-faint);
  }

  .event-main {
    display: grid;
    grid-template-columns: 140px 1fr;
    gap: 2rem;
    align-items: start;
  }

  .event-speaker-photo {
    width: 140px;
    height: 140px;
    object-fit: cover;
    object-position: top;
    display: block;
    flex-shrink: 0;
  }

  .event-content { min-width: 0; }

  .event-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.4rem;
    font-weight: 400;
    color: var(--lion-ink);
    line-height: 1.25;
    margin-top: 0;
    margin-bottom: 0.25rem;
  }

  .event-speaker {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.88rem;
    color: var(--lion-dark);
    margin-bottom: 1.25rem;
  }

  .event-body {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.9rem;
    color: var(--lion-body);
    line-height: 1.75;
    margin-bottom: 1rem;
  }

  .event-body a {
    color: var(--lion-dark);
    text-decoration: none;
    border-bottom: 1px solid var(--lion-dark);
    transition: opacity 0.2s;
  }

  .event-body a:hover { opacity: 0.7; }

  .event-abstract {
    border-left: 2px solid var(--lion-border);
    padding-left: 1.25rem;
    margin: 1.25rem 0;
  }

  .event-section-label {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--lion-faint);
    margin-bottom: 0.5rem;
    margin-top: 1.25rem;
  }

  .mailing-list-block {
    background: var(--lion-bg-tint);
    border: 1px solid var(--lion-border);
    padding: 1.5rem 2rem;
    margin-bottom: 3rem;
  }

  .mailing-list-block p {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.92rem;
    color: var(--lion-body);
    line-height: 1.7;
    margin: 0;
  }

  .mailing-list-block a {
    color: var(--lion-dark);
    text-decoration: none;
    border-bottom: 1px solid var(--lion-dark);
  }

  @media (max-width: 600px) {
    .event-main {
      grid-template-columns: 1fr;
    }
    .event-speaker-photo { width: 100px; height: 100px; }
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

  <!-- ── David Mortensen ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Monday, 20 July 2026 · 10:00</span>
      <span class="event-location">Paulinum, Room P901</span>
    </div>
    <div class="event-main">
      <img class="event-speaker-photo"
           src="{{ '/assets/img/speakers/david_mortensen.png' | relative_url }}"
           alt="David R. Mortensen">
      <div class="event-content">
        <h2 class="event-title">The Reconstruction will not be Supervised: Towards Neural Implementations of the Comparative Method</h2>
        <p class="event-speaker">Prof. David R. Mortensen — Carnegie Mellon University</p>
        <div class="event-abstract">
          <p class="event-section-label">Abstract</p>
          <p class="event-body" style="margin:0;">
            In the 19th century, European linguists discovered that it was possible to reconstruct the pronunciation of earlier languages with no surviving written records in a reproducible fashion by comparing their descendants (the Comparative Method). Starting in the 1960s, multiple attempts have been made to implement the Comparative Method computationally to assist linguists in reconstructing ancestors for the hundreds of language families existing today. However, these efforts have never achieved the accuracy and insight of a first-year student of historical linguistics. In particular, these models have relied on direct or indirect supervision, in contrast to linguistics students, who are able to operate without supervision. David presents a new way to understand the Comparative Method in terms of information theory, and shows how this framework can be used to reduce or eliminate the supervision necessary to reconstruct ancestral pronunciations (protoforms) and changes in pronunciation (sound laws). Finally, he presents results from an agent-based approach through which the entire Comparative Method can be automated without any direct supervision.
          </p>
        </div>
        <p class="event-section-label">Bio</p>
        <p class="event-body">
          David R. Mortensen is an Associate Research Professor in the Language Technologies Institute at Carnegie Mellon University. He received his PhD in Linguistics from the University of California at Berkeley and held a position as an Assistant Professor of Linguistics at the University of Pittsburgh before transitioning to CMU, computational linguistics, and NLP. His work sits at the intersection of natural language processing, speech processing, phonology, morphology, language change, and inductive reasoning. His unifying motto, "language use is language change," underscores a commitment to approaching language as a dynamic system, varying across space, time, social context, and ability. He received a Best Paper Award at ACL 2024 for work that brings together multiple strands of this agenda.
        </p>
      </div>
    </div>
  </div>

  <!-- ── Nina Böbel ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Tuesday, 14 July 2026 · 10:00</span>
      <span class="event-location">Paulinum, Room P901</span>
    </div>
    <div class="event-main">
      <img class="event-speaker-photo"
           src="{{ '/assets/img/speakers/nina_boebel.jpg' | relative_url }}"
           alt="Nina Böbel">
      <div class="event-content">
        <h2 class="event-title">Language as a (Linguistic) Network</h2>
        <p class="event-speaker">Dr. Nina Böbel — Heinrich Heine University Düsseldorf</p>
        <div class="event-abstract">
          <p class="event-section-label">Abstract</p>
          <p class="event-body" style="margin:0;">
            Construction Grammar (CxG) is one of the major approaches within Cognitive Linguistics. Analyzing linguistic units as so-called constructions (pairs of form and meaning with different levels of schematicity, complexity and idiomaticity) has numerous advantages: the approach allows for the analysis of a wide variety of units (individual words, multi-word units, and even entire sentence structures can all be considered constructions), is highly adaptable with other approaches, assumes a continuum between grammar and lexicon and, accordingly, accesses the area of linguistic utterances that cannot be captured by either lexicon or grammar alone. This talk introduces the key assumptions of Construction Grammar and explains how a group of different constructions form a so-called Constructicon (a lexicon of constructions) — basically a network of constructions. The advantages and challenges of working with linguistic networks are addressed, and it is shown that the representation of a linguistic network varies depending on the parameters assigned to the relations and on the research question. Case studies illustrating the network approach in the domains of Intensification, Conditionality, and Superlatives will show different usage scenarios.
          </p>
        </div>
        <p class="event-section-label">Bio</p>
        <p class="event-body">
          Nina Böbel is a Postdoctoral Researcher at Heinrich Heine University Düsseldorf. She is responsible for the Constructicon in the German FrameNet-Constructicon project. She earned her PhD in 2024 with a dissertation on the network of conditional clause constructions from Middle High German to today. Her research focuses on Constructicography, Construction Grammar, Historical Linguistics, Variational Linguistics, and Typology.
        </p>
      </div>
    </div>
  </div>

  <!-- ── Digital Humanities Open Garden 2026 ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag-lab">Lab Presentation</span>
      <span class="event-date">Thursday, 18 June 2026 · 16:00</span>
      <span class="event-location">Sächsische Akademie der Wissenschaften</span>
    </div>
    <div class="event-content">
        <h2 class="event-title">Hybrid Human-LLM Corpus Construction and LLM Evaluation for the Caused-Motion Construction</h2>
        <p class="event-speaker">Jun.-Prof. Dr. Leonie Weißweiler — <a href="https://fdhl.info/veranstaltungen/digital-humanities-open-garden/opengarden2026/" target="_blank" rel="noopener">Digital Humanities Open Garden 2026</a></p>
        <div class="event-abstract">
          <p class="event-section-label">About the event</p>
          <p class="event-body" style="margin:0;">
            The <a href="https://fdhl.info/veranstaltungen/digital-humanities-open-garden/opengarden2026/" target="_blank" rel="noopener">Digital Humanities Open Garden</a> is an open event hosted by the FDHL, bringing together DH-interested researchers, students, and practitioners from Leipzig and the wider region. The 2026 edition takes place at the garden of the Sächsische Akademie der Wissenschaften, Karl-Tauchnitz-Str. 1, followed by a BBQ from 17:00.
          </p>
        </div>
    </div>
  </div>

    <!-- ── Event 1 ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Wednesday, 27 May 2025 · 13:00</span>
      <span class="event-location">Paulinum, Room P702</span>
    </div>
    <div class="event-main">
      <img class="event-speaker-photo"
           src="{{ '/assets/img/speakers/arianna_muti.jpeg' | relative_url }}"
           alt="Arianna Muti">
      <div class="event-content">
        <h2 class="event-title">Implicit Misogyny and Classism in NLP</h2>
        <p class="event-speaker">Dr. Arianna Muti — Bocconi University, Milan</p>
        <div class="event-abstract">
          <p class="event-section-label">Abstract</p>
          <p class="event-body" style="margin:0;">
            Implicit misogyny and classism are difficult for NLP systems because they are often conveyed indirectly, through presuppositions, stereotypes, and unstated assumptions rather than explicit hateful expressions. Arianna presents work on analysing these implicit forms of harm in social media — framing misogyny detection as an argumentative reasoning task, and introducing ACID, a resource for studying how lower-SES people are perceived across cultures.
          </p>
        </div>
        <p class="event-section-label">Bio</p>
        <p class="event-body">
          <a href="https://milanlp.github.io/people/arianna-muti/" target="_blank" rel="noopener">Arianna Muti</a>
          is a Postdoctoral Research Fellow at Bocconi University, part of the MilaNLP group.
          Her research focuses on NLP with particular attention to detection and explanation of implicit misogyny and classism in social media. She is currently working on PERSONAE, developing identity-aware language technologies.
        </p>
      </div>
    </div>
  </div>

  <!-- ── Event 2 ── -->
  <div class="event-card">
    <div class="event-meta-row">
      <span class="event-tag">Invited Talk</span>
      <span class="event-date">Tuesday, 19 May 2025 · 13:00</span>
      <span class="event-location">Paulinum, Room P702</span>
    </div>
    <div class="event-main">
      <img class="event-speaker-photo"
           src="{{ '/assets/img/speakers/janet_liu.webp' | relative_url }}"
           alt="Yang Janet Liu">
      <div class="event-content">
        <h2 class="event-title">What Is Discourse, and What Do LLMs Know About It?</h2>
        <p class="event-speaker">Prof. Yang Janet Liu — University of Pittsburgh</p>
        <div class="event-abstract">
          <p class="event-section-label">Abstract</p>
          <p class="event-body" style="margin:0;">
            As LLM-generated output becomes increasingly fluent, evaluating what they know and how reliably they generalise has become critical. At the discourse level, meaning is conveyed beyond single sentences, shaped by linguistic conventions, communicative goals, and variation in human interpretation. Janet presents work examining LLMs' grasp of discourse coherence, how breaking down model reasoning into discourse units can account for human label variation, and how incorporating discourse relations can improve faithfulness evaluation in long-form summarisation.
          </p>
        </div>
        <p class="event-section-label">Bio</p>
        <p class="event-body">
          <a href="https://janetlauyeung.github.io/" target="_blank" rel="noopener">Yang Janet Liu</a>
          is an Assistant Professor in the Department of Linguistics at the University of Pittsburgh, with a secondary appointment in the Intelligent Systems Program. Her research focuses on computational approaches to discourse-level phenomena, LLM evaluation, and how pragmatic variation shapes language use and model behaviour. She earned her PhD from Georgetown University and was previously a postdoctoral researcher in the MaiNLP Lab at LMU Munich.
        </p>
      </div>
    </div>
  </div>

</div>