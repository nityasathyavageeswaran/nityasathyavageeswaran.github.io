---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D. candidate, Electrical and Computer Engineering, Rutgers University, 2019–present
  * Advisor: Prof. Anand D. Sarwate; also working with Prof. Roy D. Yates and Prof. Narayan Mandayam
* B.E., Electrical and Electronics Engineering, RV College of Engineering, 2019

Research Interests
======
Stochastic network optimization, applied probability, and queueing theory: age of information, privacy (maximal leakage), Markov decision processes, and scheduling for mobile edge cloud systems.

Research Projects
======
* **Timeliness and Privacy in Discrete-Time Updating Systems**
  * Studied the trade-off between age of information (AoI) and maximal leakage when an adversary observes a server's output to infer the timing of a Bernoulli update process.
  * Analyzed memoryless-thinning and accumulate-and-dump server policies (ISIT 2022), then characterized optimal coupled and decoupled LCFS policies, showing that the optimal dumping strategy dithers between two adjacent deterministic dump periods (arXiv 2025).

* **Timely Offloading in Mobile Edge Cloud Systems**
  * Formulated offloading to a mobile edge cloud as an infinite-horizon, average-cost Markov decision process balancing timeliness against MEC usage cost.
  * Proved that an optimal scheduling policy has an age-threshold structure that depends on how long an update has been in service (ITW 2024).

* **Learning to Help in Multi-Class Settings**
  * Extended the Learning to Help (L2H) framework for hybrid client–server ML systems from binary to multi-class classification, with a differentiable, convex, Bayes-consistent surrogate loss (ICLR 2025).

* **REALTIME: Resilient Edge-Cloud Autonomous Learning with Timely Inferences**
  * Developed frameworks for real-time operation of ML applications that remain resilient to data, user, and system changes, including privacy metrics for edge-assisted ML systems.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Posters
======
* N. Sathyavageeswaran, A. D. Sarwate, R. D. Yates and N. Mandayam, "Controlling Timeliness with a Costly Oracle." [[PDF]](/files/ControllingTimelinessPosterNitya.pdf)

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Skills
======
* Python (Pandas, PyTorch, NumPy, scikit-learn), MATLAB, C/C++
* LaTeX, Microsoft Office
