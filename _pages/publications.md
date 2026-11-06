---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<!-- Each section lists the .bib entries whose `keywords` field matches.
     Sections are separated by a line (<hr>). When a section has no papers yet,
     a short "coming soon" note is shown instead. -->

<div class="publications research">

<section class="research-section">
  <h2 class="research-title">Working Papers</h2>
  {% capture n_working %}{% bibliography_count --query @*[keywords~=working] %}{% endcapture %}
  {% if n_working == "0" %}
    <p class="research-empty">Coming soon.</p>
  {% else %}
    {% bibliography --query @*[keywords~=working] --group_by none %}
  {% endif %}
</section>

<hr>

<section class="research-section">
  <h2 class="research-title">Pre-PhD Research</h2>
  {% bibliography --query @*[keywords~=publication] --group_by none %}
</section>

<!--
<hr>

<section class="research-section">
  <h2 class="research-title">Work in Progress</h2>
  {% bibliography --query @*[keywords~=wip] --group_by none %}
</section>
-->

</div>
