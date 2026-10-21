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
    font-family: var(--lion-heading-font);
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
    font-family: var(--lion-heading-font);
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

  /* Collapsible entries (closed by default) */
  .course-entry > summary,
  .thesis-entry > summary {
    cursor: pointer;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1.5rem;
  }
  .course-entry > summary::-webkit-details-marker,
  .thesis-entry > summary::-webkit-details-marker { display: none; }
  .course-entry > summary::after,
  .thesis-entry > summary::after {
    content: '';
    flex-shrink: 0;
    width: 0.5rem;
    height: 0.5rem;
    border-right: 2px solid var(--lion-dark);
    border-bottom: 2px solid var(--lion-dark);
    transform: translateY(-0.15rem) rotate(45deg);
    transition: transform 0.2s;
  }
  .course-entry[open] > summary::after,
  .thesis-entry[open] > summary::after { transform: translateY(0.1rem) rotate(225deg); }
  .course-entry > summary:hover .course-name,
  .thesis-entry > summary:hover .thesis-title { color: var(--lion-dark); }
  .course-entry .course-meta { margin-bottom: 0; }
  .thesis-entry .thesis-header { margin-bottom: 0; flex-wrap: nowrap; }
  .thesis-entry .thesis-title { min-width: 0; }
  .course-entry[open] .course-desc,
  .thesis-entry[open] .thesis-body { margin-top: 0.9rem; }
</style>

<div class="lion-page">

  <div class="lion-page-header">
    <h1>Teaching</h1>
    <div class="lion-page-rule"></div>
  </div>

  <p class="lion-section-label">Courses</p>

  <details class="course-entry">
    <summary>
      <div>
        <div class="course-name">Natural Language Processing</div>
        <div class="course-meta">Lecture · B.Sc. Digital Humanities, B.Sc. Computer Science · Summer Semester</div>
      </div>
    </summary>
    <p class="course-desc">
      This course introduces students to the field of Natural Language Processing. We start with
      classic NLP tasks, then cover prerequisites to language models such as preprocessing and
      tokenisation. We move on to transformers and large language models, and finally cover topics
      from computational linguistics and their application to LLMs.
    </p>
  </details>

  <details class="course-entry">
    <summary>
      <div>
        <div class="course-name">Foundations of Machine Learning</div>
        <div class="course-meta">Lecture · B.Sc. Digital Humanities, B.Sc. Computer Science · Winter Semester</div>
      </div>
    </summary>
    <p class="course-desc">
      For a given task and measure of success, a computer program learns when its performance
      improves with experience. This course introduces machine learning as a guided search through
      a space of potential hypotheses. Students gain a broad overview of learning paradigms —
      including linear regression, decision trees, support vector machines, Bayesian learning,
      and neural networks — and understand the mathematical foundations that determine
      discrimination power and learning complexity.
    </p>
  </details>

  <details class="course-entry">
    <summary>
      <div>
        <div class="course-name">Current Topics in Natural Language Processing</div>
        <div class="course-meta">Seminar · M.Sc. Digital Humanities, M.Sc. Computer Science, M.Sc. Data Science · Irregular</div>
      </div>
    </summary>
    <p class="course-desc">
      This seminar covers a different topic from current NLP research each time it is offered.
      Students each present a paper, and at the end of the semester write up a project proposal
      for a new research project building on the current state of the topic.
      The most recent edition focused on <em>Massively Multilingual Language Models</em>.
    </p>
  </details>

  <p class="lion-section-label" style="margin-top: 3rem;">Open Thesis Positions</p>

  <div class="lion-prose" style="margin-bottom: 2rem;">
    <p>
      We offer B.Sc. and M.Sc. thesis topics to students at Leipzig University in Computer Science,
      Digital Humanities, or Data Science. Potential topics are detailed below and updated regularly,
      but we also welcome topic suggestions that fit our general research areas.
    </p>
    <p>
      We require that students have successfully completed at least our Natural Language Processing and 
      Machine Learning courses, or equivalents if their bachelor's degree is not from Leipzig University.
    </p>
    <p>
      To apply, email us with <strong>[THESIS]</strong> in the subject line, including: the topic
      you'd like to work on (with a short explanation if it's not from the list below), why you find
      it interesting, prior NLP coursework and practical experience, full transcripts, and your CV.
    </p>
  </div>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc.</span>
        <div class="thesis-title">Masked Language Models for Natural Language Pseudonym Generation</div>
      </div>
    </summary>
    <p class="thesis-body">
      Data privacy is a critical issue in NLP which limits data sharing and development of NLP
      tools to protect natural persons. While anonymisation, i.e., the removal of all Personally
      Identifiable Information (PII) from the data (&ldquo;Anne&rdquo; &rarr; &ldquo;X&rdquo;), or
      replacement with placeholders (&ldquo;Anne&rdquo; &rarr; &ldquo;firstname&rdquo;) are common
      and effective ways to ensure compliance with privacy laws, they render the source data
      illegible and thus unusable for tool development and downstream applications. MLMs present
      themselves as a particularly suitable, lightweight, and privacy-friendly tool for the task of
      predicting pseudonyms from natural language context
      (<a href="https://aclanthology.org/2026.lrec-1.90/" target="_blank" rel="noopener">cloze-style</a>).
      A thesis on this topic could work on, e.g.: (i) developing and improving evaluation metrics
      for natural-language pseudonyms, (ii) refining the prediction pipeline via, e.g., NER and
      coreference resolution, or (iii) exploring continued pre-training of MLMs using content-word
      focused training data to improve, e.g., POS accuracy. This thesis offers co-supervision with
      <a href="https://sites.google.com/view/mariaszawerna/home" target="_blank" rel="noopener">Maria Irena Szawerna</a>,
      University of Gothenburg.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc. / M.Sc.</span>
        <div class="thesis-title">Exploring Implicit Grammatical Gender in LLMs</div>
      </div>
    </summary>
    <p class="thesis-body">
      Grammatical gender, while challenging for language learners, is mastered easily by native
      speakers during language acquisition. Despite its widespread reputation of being arbitrary,
      lexical gender in German can be predicted fairly reliably via semantic, morphological, and
      phonological cues using
      <a href="https://www.cambridge.org/core/journals/language/article/abs/typology-meets-statistical-modeling-the-german-gender-system/8731EB0CEE0FC59EA9A33BEA6311EEDD" target="_blank" rel="noopener">boosting tree models</a>,
      adding evidence to the regularity of gender assignment. A thesis in this area would explore
      whether LLMs also show signs of a generalised gender assignment system in German by testing
      their behaviour on
      <a href="https://edoc.hu-berlin.de/items/63022332-0d27-4847-9f00-b10ce28cf5ab" target="_blank" rel="noopener">nonce words</a>.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc.</span>
        <div class="thesis-title">Last Translation Benchmark</div>
      </div>
    </summary>
    <p class="thesis-body">
      The <a href="https://last-translation-benchmark.vilda.net/" target="_blank" rel="noopener">Last Translation Benchmark</a>
      is an international initiative to collect translation examples that are currently unsolvable
      by LLMs, together with handwritten rules to evaluate on them automatically. A thesis could
      consist of contributing to this benchmark in a systematic way, for example by targeting a
      specific set of constructions, or a language that is so far underrepresented, or a
      semi-automatic approach to discovering potential new examples.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">M.Sc.</span>
        <div class="thesis-title">Multilingual Benchmark for Speech Language Models</div>
      </div>
    </summary>
    <p class="thesis-body">
      Although speech-text language models such as Qwen2-Audio and SeamlessM4T have shown
      remarkable abilities to process both speech and text across multiple languages, it remains
      unclear to what extent these models rely on morphosyntactic and prosodic cues when
      interpreting spoken language. Inspired by
      <a href="https://aclanthology.org/2024.wmt-1.119/" target="_blank" rel="noopener">existing</a>
      <a href="https://aclanthology.org/2024.findings-eacl.46.pdf" target="_blank" rel="noopener">benchmarks</a>
      for evaluating prosodic understanding, this thesis aims to develop a multilingual benchmark
      for systematically evaluating how speech language models process prosodic and
      morphosyntactic information across languages.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">M.Sc.</span>
        <div class="thesis-title">Grammatical Structures in the Implicit Vocabulary of LLMs</div>
      </div>
    </summary>
    <p class="thesis-body">
      <a href="https://aclanthology.org/2024.emnlp-main.543/" target="_blank" rel="noopener">Recent</a>
      <a href="https://proceedings.iclr.cc/paper_files/paper/2025/hash/aef75887979ae1287b5deb54a1e3cbda-Abstract-Conference.html" target="_blank" rel="noopener">work</a>
      has discovered that in their lower layers, LLMs form an implicit vocabulary, merging or
      &lsquo;detokenising&rsquo; subword tokens back into representations of complete words. While
      results suggest that LLMs do this not only for multi-token words, but also for multi-word
      expressions or more complex small phrases, the linguistic nature of these representations
      has not been studied. Extending previous methods to the study of the implicit vocabulary
      beyond words would form a contribution to the question of implicit learning of grammatical
      structures in LLMs.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc. / M.Sc.</span>
        <div class="thesis-title">Expanding and Improving Universal Dependencies for German</div>
      </div>
    </summary>
    <p class="thesis-body">
      Universal Dependencies (UD) is a framework for consistent annotation of grammar across
      human languages. The largest UD treebank of any language is UD-HDT, created via automatic
      conversion from the Hamburg Dependency Treebank and not actively maintained since 2017.
      A thesis could integrate additional pre-conversion data and fix known errors and inconsistencies.
      A M.Sc. thesis would additionally train UD parsers before and after the fixes and evaluate
      them on German treebanks to demonstrate the impact of the changes.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc. / M.Sc.</span>
        <div class="thesis-title">Adopt a Universal Dependencies Treebank</div>
      </div>
    </summary>
    <p class="thesis-body">
      Universal Dependencies (UD) is a framework for consistent annotation of grammar across
      human languages. Most UD treebanks have not been actively maintained since creation, accumulating validation
      errors that limit their usefulness. If you read (natively or with reasonable comprehension)
      any of the languages in the
      <a href="https://quest.ms.mff.cuni.cz/udvalidator/cgi-bin/unidep/validation-report.pl" target="_blank" rel="noopener">UD validation report</a>,
      a thesis could adopt that treebank, fix errors and warnings, and expand feature coverage
      or cross-treebank consistency. A M.Sc. thesis would validate improvements by training and
      comparing parsers before and after.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc. / M.Sc.</span>
        <div class="thesis-title">Unsupervised Discovery of Unaccusative and Unergative Verbs</div>
      </div>
    </summary>
    <p class="thesis-body">
      Within the broader category of intransitive verbs, unaccusative (e.g., <i>You fall</i>) and unergative (e.g., <i>You resign</i>) verbs have special syntactic
      behaviour relating to the semantic role of the subject, with is agentive for unaccusative verbs and patient-like for unergative verbs. These syntactic behaviours are 
      not trivial to detect because in standard sentences, the distinction is only visible through the semantics of the subject. <a href="https://arxiv.org/pdf/2111.00808" target="_blank" rel="noopener">Previous work</a> has made a first attempt at unsupervised discovery of both categories, and the thesis would attempt to approve on this
      with more modern methods, or possibly extend it to further languages where unaccusative and unergative verbs might have different properties.
    </p>
  </details>

  <details class="thesis-entry">
    <summary>
      <div class="thesis-header">
        <span class="thesis-level">B.Sc. / M.Sc.</span>
        <div class="thesis-title">Complex Noun Compound Benchmark</div>
      </div>
    </summary>
    <p class="thesis-body">
      Noun compounds provide an interesting test case for LLMs' understanding of complex noun semantics, as well as generalisation to novel compounds. <a href="https://aclanthology.org/2023.findings-acl.169.pdf">Previous work</a> has investigated this for compounds of two nouns. Compounds of more than two nouns are semantically far more complex and 
      remain unexplored as a test case for LLMs. We might for example ask, is a <i>child camel jockey slave</i> a type of (child|camel|jockey|slave)? Data for this could e.g. come
      from the recently release <a href="https://github.com/ilndwhr/CoBra/tree/main">Compound Branching Resource</a>, or could be automatically collected from corpora and then hand-annotated. The thesis would lead to the creation of a (possibly multilingual) benchmark of LLMs' understanding of complex noun compounds and their internal structure.
    </p>
  </details>

</div>
