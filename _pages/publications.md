---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<!-- Inline styling -->
<style>
.research-title {
  color: var(--global-theme-color);  /* uses al-folio theme blue */
  font-weight: 500;
  margin-top: 3rem;
  margin-bottom: 1rem;
  padding-bottom: 0.3rem;
  border-bottom: 2px solid var(--global-theme-color);
}
</style>

<div class="publications">

<h2 class="research-title">Publication</h2>

{% bibliography --query @*[keywords~=publication] %}

<h2 class="research-title">Working Papers</h2>

{% bibliography --query @*[keywords~=working] %}

<h2 class="research-title">Work in Progress</h2>

{% bibliography --query @*[keywords~=wip] %}

</div>
