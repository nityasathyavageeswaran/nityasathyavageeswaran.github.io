---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Under Submission

* **Timely Offloading with Multiple Sources**, extending the mobile edge cloud offloading analysis of the ITW 2024 paper to multiple sources.

## Posters

<div style="display:flex; flex-wrap:wrap; gap:1.25em; align-items:flex-start; margin-top:0.5em;">
  <a href="{{ base_path }}/files/ControllingTimelinessPosterNitya.pdf" style="flex:0 0 260px; max-width:100%;">
    <img src="{{ base_path }}/images/poster-controlling-timeliness.jpg" alt="Poster: Controlling Timeliness with a Costly Oracle" style="width:100%; border:1px solid #ddd; border-radius:4px;">
  </a>
  <div style="flex:1 1 260px;">
    <p style="margin-top:0;"><strong>Controlling Timeliness with a Costly Oracle</strong><br>
    N. Sathyavageeswaran, A. D. Sarwate, R. D. Yates and N. Mandayam<br>Poster presentation, BIRS, Chennai, 2025</p>
    <p>A device can process status updates locally or offload them to a mobile edge cloud (MEC) at a cost. The scheduling problem is modeled as an MDP; the optimal policy is an age-threshold policy that depends on how long an update has been in service, and a simpler service-time threshold policy performs close to optimal. Companion poster to <a href="{{ base_path }}/publication/timely-offloading-mobile-edge-cloud"><em>Timely Offloading in Mobile Edge Cloud Systems</em></a> (ITW 2024).</p>
    <p><a href="{{ base_path }}/files/ControllingTimelinessPosterNitya.pdf"><u>View poster (PDF)</u></a></p>
  </div>
</div>
