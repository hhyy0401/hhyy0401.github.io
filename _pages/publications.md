---
layout: page
permalink: /publications/
title: publications
description: "*: equal contribution | P: Preprint, J: Journal, C: Conference"
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography --query @*[presentation!=poster] %}

</div>

## Conference Presentations & Posters
{:.mt-5}

<div class="publications">

{% bibliography --query @*[presentation=poster] %}

</div>
