---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Publication summary -->
<div class="card mb-4">
  <div class="card-body">
    <h4 class="card-title text-center mb-4">Summary of Publications</h4>
    <div class="row text-center">
      <div class="col-6 col-md-3 mb-3 mb-md-0">
        <h2 class="mb-0">2</h2>
        <div class="text-muted">First-author publications</div>
      </div>
      <div class="col-6 col-md-3 mb-3 mb-md-0">
        <h2 class="mb-0">1</h2>
        <div class="text-muted">Second-author publications</div>
      </div>
      <div class="col-6 col-md-3">
        <h2 class="mb-0">5</h2>
        <div class="text-muted">Significant contribution</div>
      </div>
      <div class="col-6 col-md-3">
        <h2 class="mb-0">4</h2>
        <div class="text-muted">SKAO "Advancing Astrophysics II" book chapters</div>
      </div>
    </div>
  </div>
</div>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h3>First-author publications</h3>
{% bibliography --group_by none --query @*[category=first-author]* %}

<h3>Second-author publications</h3>
{% bibliography --group_by none --query @*[category=second-author]* %}

<h3>Significant contribution</h3>
{% bibliography --group_by none --query @*[category=significant-contribution]* %}

<h3>SKAO "Advancing Astrophysics II" book chapters</h3>
{% bibliography --group_by none --query @*[category=skao-book]* %}

</div>
