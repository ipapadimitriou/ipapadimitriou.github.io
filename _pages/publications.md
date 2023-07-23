---
layout: page
permalink: /publications/
title: publications
description: (author names in alphabetical order)
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

An up-to-date list is available on <a href='https://inspirehep.net/literature?q=a%20I.Papadimitriou.1'>iNSPIRE</a>

<h1 style="text-align: left;">preprints</h1>

{% bibliography -f {{ site.scholar.bibliography }} -q @*[type~=preprint]* %}

<h1 style="text-align: left;">refereed journals</h1>

{% bibliography -f {{ site.scholar.bibliography }} -q @*[type~=article]* %}

<h1 style="text-align: left;">refereed conference proceedings</h1>

 {% bibliography -f papers -q @*[type~=proceedings]* %}

<h1 style="text-align: left;">theses</h1>

{% bibliography -f papers -q @*[type~=thesis]* %}

</div>


