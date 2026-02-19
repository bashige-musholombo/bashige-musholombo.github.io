---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<div class="publications">

<h2>Publications</h2>

{% bibliography --query @*[keywords~=publication] %}

<hr>

<h2>Working Papers</h2>

{% bibliography --query @*[keywords~=working] %}

<hr>

<h2>Work in Progress</h2>

{% bibliography --query @*[keywords~=wip] %}

</div>
