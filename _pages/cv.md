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
* **Ph.D. candidate, Electrical and Computer Engineering**, Rutgers, The State University of New Jersey, New Brunswick, NJ
  * Advisor: Prof. Anand D. Sarwate; also working with Prof. Roy D. Yates and Prof. Narayan Mandayam
  * Research focus: machine learning, uncertainty-aware inference, sequential decision-making, optimization
* **B.E., Electrical and Electronics Engineering**, RV College of Engineering, Bangalore, India, May 2019

Professional Experience
======
* **Edge & Industrial Network Systems Research Intern**, Siemens AG, Princeton, NJ — Jul–Sep 2026
  * **IT network diagnostics tool:** Built a PowerShell tool that runs layer-by-layer checks (physical through application layer) on connectivity from an engineering laptop to Siemens Industrial Edge devices and the Industrial Edge Management cloud, pinpointing the exact layer where a connection fails.
  * **OT network diagnostics tool:** Developed a companion tool for the operational technology (OT) side to validate and troubleshoot connectivity between virtual machines and PLCs on the industrial network.
  * **IT/OT integration:** Together, the tools streamline fault isolation across the IT/OT boundary of edge deployments and reduce manual troubleshooting effort for engineers.

* **Graduate Research Assistant**, WINLAB, Rutgers University — Sep 2020–present
  * **Hybrid ML system design:** Engineered a stage-switching client–server framework for multi-class image classification that offloads high-uncertainty inputs to a server model, cutting compute while preserving accuracy.
  * **Model training and tuning:** Trained CNN (LeNet-5, AlexNet) and Vision Transformer classifiers in PyTorch on GPU (CIFAR-10/100, SVHN); ran hyperparameter sweeps to map accuracy–convergence trade-offs.
  * **Robustness:** The router handles class imbalance and distribution shift, deferring unseen-class and blurry images to the server.
  * **Loss function design:** Derived a convex, Bayes-consistent surrogate loss for joint client–server training.
  * **Deployment constraints:** Built asynchronous training for pay-per-request costs, intermittent servers, and bounded reject rates.
  * **Sequential decision-making:** Formulated freshness–stability and offloading problems as average-cost Markov decision processes and derived optimal state-aware scheduling policies.
  * **Constrained optimization:** Solved the timeliness–privacy trade-off as a fractional program using Dinkelbach's method and linear programming, validated with large-scale Monte Carlo simulations.

* **Teaching Assistant**, Department of Electrical and Computer Engineering, Rutgers University
  * Signals and Systems, Probability and Random Processes, and Principles of Electrical Engineering (details below).

Awards
======
* ECE Teaching Assistant Award, Rutgers University (2021, 2023)

Research Projects
======
* **Timeliness and Privacy in Discrete-Time Updating Systems**
  * Studied the trade-off between age of information (AoI) and maximal leakage when an adversary observes a server's output to infer the timing of a Bernoulli update process.
  * Analyzed memoryless-thinning and accumulate-and-dump server policies (ISIT 2022), then characterized optimal coupled and decoupled LCFS policies, showing that the optimal dumping strategy dithers between two adjacent deterministic dump periods (submitted to IEEE Transactions on Information Theory).

* **Timely Offloading in Mobile Edge Cloud Systems**
  * Formulated offloading to a mobile edge cloud as an infinite-horizon, average-cost Markov decision process balancing timeliness against MEC usage cost.
  * Proved that an optimal scheduling policy has an age-threshold structure that depends on how long an update has been in service (ITW 2024); extending the analysis to multiple sources (under submission).

* **Age and Stability Trade-offs in Remote Monitoring Systems**
  * Modeled a shared server balancing queue clearing against status updates as an MDP minimizing a weighted sum of average AoI and queue length; showed the optimal policy is a monotone threshold rule on the queue state (ITW 2026).

* **Learning to Help in Multi-Class Settings**
  * Extended the Learning to Help (L2H) framework for hybrid client–server ML systems from binary to multi-class classification, with a differentiable, convex, Bayes-consistent surrogate loss (ICLR 2025).

* **REALTIME: Resilient Edge-Cloud Autonomous Learning with Timely Inferences**
  * Developed frameworks for real-time operation of ML applications that remain resilient to data, user, and system changes, including privacy metrics for edge-assisted ML systems.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Under Submission
======
* N. Sathyavageeswaran et al., "Timely Offloading with Multiple Sources."

Posters
======
* N. Sathyavageeswaran, A. D. Sarwate, R. D. Yates and N. Mandayam, "Controlling Timeliness with a Costly Oracle," poster presentation, BIRS, Chennai, 2025. [[PDF]](/files/ControllingTimelinessPosterNitya.pdf)

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Technical Skills
======
* **Machine learning:** PyTorch, scikit-learn, Pandas, NumPy
* **Programming:** Python (including CuPy for GPU acceleration), C/C++, SQL, MATLAB, Git, Docker, LaTeX
* **Core concepts:** ML system design, MDPs and reinforcement learning, convex optimization, privacy
