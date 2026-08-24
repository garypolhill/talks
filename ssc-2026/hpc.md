<!-- .slide: class="title-slide" -->
# Why ABM needs HPC
## Gary Polhill<sup>1</sup> &amp; Alison Heppenstall<sup>2</sup>

<sup>1</sup> The James Hutton Institute
<sup>2</sup> University of Glasgow

<div class="logo-strip">
  <div class="logo-box"><img src="../brand/hutton/hutton-logo.png" alt="The James Hutton Institute Logo" style="height:44px;"/></div>
  <div class="logo-box"><img src="../brand/glasgow/glasgow-logo.png" alt="University of Glasgow Logo" style="height:44px;"/></div>
</div>

---

# What is High-Performance Computing?

  + High-Performance Computing provides its users with access to far greater computing resource than is available on a personal computing device

    + Personal computers are capable of about 1bn floating-point operations per second (gigascale)
    + Local or institutional HPC infrastructure allows you access to about 1000 times that (terascale)
    + National HPC infrastructure is generally 1000 times more... (petascale)
    + The USA, Europe, Japan, China, and the UK already have, or will soon have exascale computing infrastructure

  + Some personal computers with expensive graphics cards can also scale up computation rates _if they are carefully programmed_

  + Exascale computing typically relies on efficient GPU programming to achieve these speeds
    
    + Most HPC infrastructure is generally CPU-based, but newer systems include significant GPU provision, and some are exclusively so

---

<!-- .slide: class="right-image-slide" -->

# The ExAMPLER project

<div class="split">
<div class="split-text">

  + Funded by the Engineering and Physical Sciences Research Council under the ExCALIBUR Programme, the ExAMPLER project explored what needed to be done to get agent-based models using exascale compute

  + Our main finding is that we need to increase our HPC (and GPU) use

    + Typical-case ABM is still personal computer based (Polhill et al., under revision)

    + (Strictly, typical-case ABM doesn't report the computing environment...)

</div> <div class="split-image">

![ExAMPLER logo](img/exampler-logo.png)

</div>
</div>

---

# ExAMPLER project findings

We also found that there are many hurdles faced by the social simulation community when accessing HPC resources

![Graphic showing the hurdles faced by ABMers](img/hurdles.png)

--- 

<!-- .slide: class="right-image-slide" -->

# Use cases of HPC with ABMs

<div class="split">
<div class="split-text">

  + Work using HPC and GPUs includes

    + Polhill et al. (2013) _Environmental Modelling &amp; Software_ &mdash; roughly 22000 runs of the FEARLUS-SPOMM agent-based model to explore principles for incentivizing biodiversity

    + Axtell (2016) _AAMAS_ &mdash; simulates 120 million agents (citizens and businesses) in the US economy on a GPU

    + Joubert et al. (2022) _Computers, Environment &amp; Urban Systems_ &mdash; model street robbery in Cape Town at a high resolution using a hybrid CPU/GPU simuation environment; it still takes several days for each simulation to complete!

</div><div class="split-image">

![Decision tree summarizing results from Polhill et al. (2013)](img/fearlus-spomm.jpg)

</div>
</div>

---

# Potential of HPC with ABMs

  + Regional, national and international-scale simulations
    + Town / small city scale more common currently
    + _Northern Powerhouse_ in the UK would involve several cities &mdash; Leeds, Sheffield, Manchester, Liverpool
    + More generally: if we build infrastructure _here_ what is the effect on people _there_ (100+km away)

  + Calibration &mdash; an 'embarrassingly parallel' problem perfect for HPC
    + If I can explore 100 parameter samples on my laptop, I can do 100,000,000 samples on national HPC infrastructure!
    + Better calibrated models are easier to trust

  + Similarly for uncertainty analysis

  + Better exploration of formalized social theories
    + Searching all the alternative representations rather than just one implementation with many arbitrary choices...

---

<!-- .slide: class="right-image-slide" -->

# Access to HPC for ABMs


<div class="split">
<div class="split-text">


  + See Polhill (2022)

  + Sound theoretical reasons why agent-based models are difficult to use in environments where RAM and CPU time need to be predicted

    + Birth and death of agents
    + Creation and destruction of social links
    + Context sensitive decision-making algorithms (e.g. CONSUMAT)

  + Technical reasons too &mdash; _must_ we access HPC by command-line?

</div> <div class="split-image">

![Screenshot of antiscoial simulation paper](img/antisoc-sim.png)

</div>
</div>
