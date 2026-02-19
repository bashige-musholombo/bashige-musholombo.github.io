---
layout: page
permalink: /research/
title: Research
description:
nav: true
nav_order: 2
---

<div class="publications">

## Publications

{% bibliography --query @*[keywords~=publication] %}

## Working Papers

{% bibliography --query @*[keywords~=working] %}

## Work in Progress

{% bibliography --query @*[keywords~=wip] %}

</div>
