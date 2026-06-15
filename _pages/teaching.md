---
layout: default
title: Teaching
description: Courses and thesis opportunities at the LION Lab.
permalink: /teaching/
---

{% include page-styles.html %}

<style>
  .course-entry {
    padding: 1.75rem 0;
    border-bottom: 1px solid #f0e4d4;
  }

  .course-entry:first-of-type { border-top: 1px solid #f0e4d4; }
  .course-entry:last-of-type { border-bottom: none; }

  .course-name {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.1rem;
    font-weight: 400;
    color: #1a1209;
    margin-bottom: 0.3rem;
  }

  .course-meta {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.75rem;
    color: #a09080;
    letter-spacing: 0.04em;
    margin-bottom: 0.75rem;
  }

  .course-desc {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.88rem;
    color: #3a2e20;
    line-height: 1.75;
  }

  .thesis-entry {
    padding: 2rem 0;
    border-bottom: 1px solid #f0e4d4;
  }

  .thesis-entry:first-of-type { border-top: 1px solid #f0e4d4; }

  .thesis-header {
    display: flex;
    align-items: baseline;
    gap: 0.75rem;
    margin-bottom: 0.75rem;
    flex-wrap: wrap;
  }

  .thesis-level {
    font-family: var(--lion-caps-font, 'Amasis MT Pro', Georgia, serif);
    font-size: 0.68rem;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #fff;
    background: #E26600;
    padding: 0.15rem 0.55rem;
    flex-shrink: 0;
  }

  .thesis-title {
    font-family: 'Playfair Display', Georgia, serif;
    font-size: 1.1rem;
    font-weight: 400;
    color: #1a1209;
  }

  .thesis-body {
    font-family: 'Lora', Georgia, serif;
    font-size: 0.88rem;
    color: #3a2e20;
    line-height: 1.75;
  }

  .thesis-body a {
    color: #E26600;
    text-decoration: none;
    border-bottom: 1px solid #E26600;
    transition: opacity 0.2s;
  }

  .thesis-body a:hover { opacity: 0.7; }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Teaching</h1>
    <div class="lion-page-rule"></div>
  </div>

  <p class="lion-section-label">Courses</p>

  <div class="course-entry">
    <p class="course-name">Natural Language Processing</p>
    <p class="course-meta">Lecture · B.Sc. Digital Humanities, B.Sc. Computer Science · Summer Semester</p>    
    <p class="course-desc">
      This course introduces students to the field of Natural Language Processing. We start with
      classic NLP tasks, then cover prerequisites to language models such as preprocessing and
      tokenisation. We move on to transformers and large language models, and finally cover topics
      from computational linguistics and their application to LLMs.
    </p>
  </div>

  <div class="course-entry">
    <p class="course-name">Foundations of Machine Learning</p>
    <p class="course-meta">Lecture · B.Sc. Digital Humanities, B.Sc. Computer Science · Winter Semester</p>
    <p class="course-desc">
      For a given task and measure of success, a computer program learns when its performance
      improves with experience. This course introduces machine learning as a guided search through
      a space of potential hypotheses. Students gain a broad overview of learning paradigms —
      including linear regression, decision trees, support vector machines, Bayesian learning,
      and neural networks — and understand the mathematical foundations that determine
      discrimination power and learning complexity.
    </p>
  </div>

  <div class="course-entry">
    <p class="course-name">Current Topics in Natural Language Processing</p>
    <p class="course-meta">Seminar · M.Sc. Digital Humanities, M.Sc. Computer Science, M.Sc. Data Science · Irregular</p>
    <p class="course-desc">
      This seminar covers a different topic from current NLP research each time it is offered.
      Students each present a paper, and at the end of the semester write up a project proposal
      for a new research project building on the current state of the topic.
      The most recent edition focused on <em>Massively Multilingual Language Models</em>.
    </p>
  </div>

  <p class="lion-section-label" style="margin-top: 3rem;">Open Thesis Positions</p>

  <div class="lion-prose" style="margin-bottom: 2rem;">
    <p>
      We offer B.Sc. and M.Sc. thesis topics to students at Leipzig University in Computer Science,
      Digital Humanities, or Data Science. Potential topics are detailed below and updated regularly,
      but we also welcome topic suggestions that fit our general research areas. We generally require
      that students have successfully completed at least our Natural Language Processing and 
      Machine Learning courses, or equivalents if their bachelor's degree is not from Leipzig University.
    </p>
    <p>
      To apply, email us with <strong>[THESIS]</strong> in the subject line, including: the topic
      you'd like to work on (with a short explanation if it's not from the list below), why you find
      it interesting, prior NLP coursework and practical experience, full transcripts, and your CV.
    </p>
  </div>

  <div class="thesis-entry">
    <div class="thesis-header">
      <span class="thesis-level">B.Sc. / M.Sc.</span>
      <p class="thesis-title">Expanding and Improving Universal Dependencies for German</p>
    </div>
    <p class="thesis-body">
      Universal Dependencies (UD) is a framework for consistent annotation of grammar across
      human languages. The largest UD treebank of any language is UD-HDT, created via automatic
      conversion from the Hamburg Dependency Treebank and not actively maintained since 2017.
      A thesis could integrate additional pre-conversion data and fix known errors and inconsistencies.
      A M.Sc. thesis would additionally train UD parsers before and after the fixes and evaluate
      them on German treebanks to demonstrate the impact of the changes.
    </p>
  </div>

  <div class="thesis-entry">
    <div class="thesis-header">
      <span class="thesis-level">B.Sc. / M.Sc.</span>
      <p class="thesis-title">Adopt a UD Treebank</p>
    </div>
    <p class="thesis-body">
      Most UD treebanks have not been actively maintained since creation, accumulating validation
      errors that limit their usefulness. If you read (natively or with reasonable comprehension)
      any of the languages in the
      <a href="https://quest.ms.mff.cuni.cz/udvalidator/cgi-bin/unidep/validation-report.pl" target="_blank" rel="noopener">UD validation report</a>,
      a thesis could adopt that treebank, fix errors and warnings, and expand feature coverage
      or cross-treebank consistency. A M.Sc. thesis would validate improvements by training and
      comparing parsers before and after.
    </p>
  </div>

  <div class="thesis-entry">
    <div class="thesis-header">
      <span class="thesis-level">B.Sc. / M.Sc.</span>
      <p class="thesis-title">Unsupervised Discovery of Unaccusative and Unergative Verbs</p>
    </div>
    <p class="thesis-body">
      Within the broader category of intransitive verbs, unaccusative (e.g., <i>You fall</i>) and unergative (e.g., <i>You resign</i>) verbs have special syntactic
      behaviour relating to the semantic role of the subject, with is agentive for unaccusative verbs and patient-like for unergative verbs. These syntactic behaviours are 
      not trivial to detect because in standard sentences, the distinction is only visible through the semantics of the subject. <a href="https://arxiv.org/pdf/2111.00808" target="_blank" rel="noopener">Previous work</a> has made a first attempt at unsupervised discovery of both categories, and the thesis would attempt to approve on this
      with more modern methods, or possibly extend it to further languages where unaccusative and unergative verbs might have different properties.
    </p>
  </div>

  <div class="thesis-entry">
    <div class="thesis-header">
      <span class="thesis-level">B.Sc. / M.Sc.</span>
      <p class="thesis-title">Complex Noun Compound Benchmark</p>
    </div>
    <p class="thesis-body">
      Noun compounds provide an interesting test case for LLMs' understanding of complex noun semantics, as well as generalisation to novel compounds. <a href="https://aclanthology.org/2023.findings-acl.169.pdf">Previous work</a> has investigated this for compounds of two nouns. Compounds of more than two nouns are semantically far more complex and 
      remain unexplored as a test case for LLMs. We might for example ask, is a <i>child camel jockey slave</i> a type of (child|camel|jockey|slave)? Data for this could e.g. come
      from the recently release <a href="https://github.com/ilndwhr/CoBra/tree/main">Compound Branching Resource</a>, or could be automatically collected from corpora and then hand-annotated. The thesis would lead to the creation of a (possibly multilingual) benchmark of LLMs' understanding of complex noun compounds and their internal structure.
    </p>
  </div>

</div>