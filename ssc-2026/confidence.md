<!-- .slide: class="title-slide" -->
# Communicating Confidence in Agent-Based Models
## Gary Polhill, Matt Hare, Nick Roxburgh, Doug Salt, Marie Castellazzi &amp; Becky Smith

The James Hutton Institute

<div class="logo-strip">
  <div class="logo-box"><img src="../brand/hutton/hutton-logo.png" alt="The James Hutton Institute Logo" style="height:44px;"/></div>
</div>

---

# Why?

  + Edmonds (2022) proposed various levels of rigour according to potential use of a model
    + Use by you &mdash; not too onerous...
    + ... via discussion and publication &mdash; increasing requirements
    + ... to decision support (e.g. in policy) &mdash; so onerous there wasn't space in the article write them!

  + Policy modelling is done in the UK by civil servants ('analysts') whose work is governed by the Aqua Book
    + Typically in spreadsheets; but complex analytical pipelines using computer code are also governed by the 'Duck' Book

  + How could ABM for policy meet these stipulations?
    + We don't want to rule ourselves out of contributing insights from complex systems thinking by wrapping ourselves in impossible layers of rigour

---

# Overview of Proposed Approach

  + Identify various 'dimensions' that might be used to assess the quality of a model
    + Some of these could be co-constructed and agreed with the model's end-users

  + For each such dimension, identify four levels of degree to which a model meets that dimension's requirements
    + Level 0 &mdash; most inclusive; almost anything would meet it
    + Level 3 &mdash; most rigorous

  + Use the _lowest_ level across all the agreed dimension to report the model's quality

---

<!-- .slide: class="right-image-slide"  -->

# Some Dimensions

<div class="split">
<div class="split-text">

  + Scientific and Theoretical Foundations
    + e.g. 'Basic Principles' in ODD (Grimm et al. 2020)

  + Stuctural Verification
    + How does the descriptive and causal structure of the model reflect the empirical world? ('Verisimilitude' in Jason Thompson's talk &mdash; wanted stakeholders to understand the model because it used pretty much the same language)

  + Confirmability
    + Traditional model fit metrics

  + Generalizability
    + How many case studies has the model been successfully applied to?

  + Replicability
    + How well have results been replicated?

  + Data Accessibility
    + How easy is it to use the same data sources as the model?


</div><div class="split-text">

  + Community
    + Who has used the model (besides the developer)?

  + Quality Assurance
    + To what extent has the quality assurance followed recommendations in the AQuA Book?

  + Documentation
    + What level of documentation is there about the model

  + Coding Practice &amp; Readability
    + What evidence is there of good practice in writing the code?

  + Verifiability
    + How much has the code been tested to ensure it behaves as designed?

  + Portability
    + How sensitive is the model to its runtime environment

</div></div>

---

# Example

Consider the FEARLUS model (Polhill et al. 2001), a 'typification' according to Boero &amp; Squazzoni (2005) what dimensions might _not_ be relevant?

  + **Confirmability** &mdash; FEARLUS was not designed in 2001 to be fitted to an empirical case study
  + **Generalizability** &mdash; For similar reasons, there won't be several case studies to which FEARLUS has been applied
  + **Data Accessibility** &mdash; ... and there won't be empirical data either
  + **Quality Assurance** &mdash; it was built before the AQuA book was conceived!

---

<!-- .slide: class="right-image-slide"  -->

# Example cont'd

So, how does FEARLUS measure up against the relevant dimensions?

<div class="split"><div class="split-text">

  + **Scientific &amp; Theoretical Foundations** &mdash; satisficing, imitation
    + Level 1: _References are made somewhere to scientific or theoretical foundations for some parts of the model_

  + **Structural Verification** &mdash; class names and attributes are meaningful
    + Level 1: _Nomenclature ... suggests intended link to the empirical world_

  + **Replicability** &mdash; See Doug Salt's talk on a later version
    + Level 3: _Exact ... replication of reported results_

  + **Community** &mdash; A handful of users in the project team
    + Level 1: _Used by developer and team in a project_

</div><div class="split-text">

  + **Documentation** &mdash; User guide and ODD
    + Level 2: _Documentation exists on  what the code does and how to use it_

  + **Coding Practice &amp; Readability** &mdash; Can I evaluate this objectively!?
    + Level 2: _Consistent nomenclature ... good commenting ... version controlled_

  + **Verifiability** &mdash; I don't remember unit testing... but it's been run hundreds of thousands of times
    + Level 1: _Model not expected to crash with any parameter settin or input_

  + **Portability** &mdash; Tricky: FEARLUS is built in Swarm. Has a statically-compiled executable
    + Level 1: _Model will run on multiple computers with the same OS_

</div></div>

---

<!-- .slide: class="section-title-purple" -->

# Conclusion:
## FEARLUS is a 'Level 1' model

---

# Discussion Points

  + How _practical_ are standards, protocols, etc.?
    + Can we keep ourselves in the conversation?

  + _Must_ models for decision support be empirical?
    + See Gilbert et al. (2018) &mdash; maybe the insights are gained during co-construction 

  + If not this way...
    + How _can_ we communicate rigour, and empower end-users of results and insights to make up their own mind about how much to trust a model?
    + _Without_ imposing infeasible, impractical and/or unrealistic conditions on ourselves?

---

<!-- .slide: class="final-slide" -->

These slides: https://garypolhill.github.io/talks/ssc-2026/confidence.html

![QR code for talk URL](img/confidence-qr.png)