---
layout: default
title: Publications
description: Research publications from the LION Lab.
permalink: /publications/
---

{% include page-styles.html %}

<style>
  .pub-entry {
    display: grid;
    grid-template-columns: 60px 1fr;
    gap: 1.5rem;
    padding: 1.75rem 0;
    border-bottom: 1px solid #f0e4d4;
  }

  .pub-entry:first-of-type {
    border-top: 1px solid #f0e4d4;
  }

  .pub-year {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.75rem;
    letter-spacing: 0.1em;
    color: #E26600;
    padding-top: 0.2rem;
    text-align: right;
  }

  .pub-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.05rem;
    font-weight: 400;
    color: #1a1209;
    margin-bottom: 0.3rem;
    line-height: 1.35;
  }

  .pub-title a {
    color: inherit;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
    transition: color 0.2s;
  }

  .pub-title a:hover { color: #E26600; }

  .pub-authors {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.85rem;
    color: #7a6a55;
    margin-bottom: 0.2rem;
  }

  .pub-authors strong {
    color: #3a2e20;
    font-weight: 600;
  }

  .pub-venue {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.82rem;
    color: #a09080;
  }

  .pub-venue em {
    font-style: normal;
    color: #E26600;
  }

  .pub-abstract {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.83rem;
    color: #5a4e40;
    line-height: 1.75;
    margin-top: 0.75rem;
    border-left: 2px solid #f0e4d4;
    padding-left: 1rem;
    display: none;
  }

  .pub-abstract.open {
    display: block;
  }

  .pub-toggle {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.72rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #E26600;
    background: none;
    border: none;
    cursor: pointer;
    padding: 0;
    margin-top: 0.5rem;
    display: inline-block;
    transition: opacity 0.2s;
  }

  .pub-toggle:hover { opacity: 0.7; }

  @media (max-width: 600px) {
    .pub-entry {
      grid-template-columns: 1fr;
      gap: 0.3rem;
    }
    .pub-year { text-align: left; }
  }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Publications</h1>
    <div class="lion-page-rule"></div>
  </div>

  <div class="pub-entry">
    <p class="pub-year">2026</p>
    <div>
      <p class="pub-title">
        <a href="https://arxiv.org/abs/2605.31586" target="_blank" rel="noopener">

          Language Models Learn Constructional Semantics, Not To Mention Syntax: Investigating LM Understanding of Paired-Focus Constructions
        </a>
      </p>
      <p class="pub-authors">Wesley Scivetti, Ethan Gotlieb Wilcox, Nathan Schneider, Kanishka Misra, <strong>Leonie Weissweiler</strong></p>
      <p class="pub-venue"><em>30th Conference on Computational Natural Language Learning (CoNLL 2026)</em></p>
      <button class="pub-toggle" onclick="this.nextElementSibling.classList.toggle('open'); this.textContent = this.nextElementSibling.classList.contains('open') ? 'Hide abstract ↑' : 'Abstract ↓'">Abstract ↓</button>
      <p class="pub-abstract">
        Grasping the semantics of rare constructions (form–meaning pairings) has been shown to be a challenging problem that has currently only been solved by the largest LLMs. It remains an open question if open-source models have robust constructional understanding, and if so, what learning dynamics underlie the acquisition of this knowledge. Focusing on a set of rare Paired-Focus constructions in English (e.g. "let alone", "much less"), we construct a novel dataset to test their meanings using both scalar adjectival semantics and general world knowledge. Testing a wide range of models differing in parameter count, architecture, and pretraining dataset size, we find that several modestly sized models are sensitive to both the forms and the meanings of Paired-Focus constructions, though models trained on human-scale data fail at all meaning evaluations. Turning to training dynamics for a set of open-checkpoint models, we find that Paired-Focus understanding emerges later in training than Paired-Focus syntactic knowledge, and that learning of Paired-Focus semantics is correlated with gains in some domains of world knowledge. Overall, our empirical results support the conclusion that modestly sized open-source models can grasp the rare Paired-Focus constructions, and demonstrate a connection between knowledge of Paired-Focus constructions and other meaning domains.
      </p>
    </div>
  </div>

  <!-- Add further entries above in the same format -->

</div>