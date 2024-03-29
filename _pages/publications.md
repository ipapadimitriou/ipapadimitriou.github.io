---
layout: page
permalink: /publications/
title: publications
description: (author names in alphabetical order)
nav: true
nav_order: 2
---

<!--
    Script for Latex, copied from https://www.sarpublisher.com/how-to-enable-latex-in-blogger/
    Remember change the http in src to https, or your browser may refuse to load it.
    Offical docs of MathJax can be found under https://docs.mathjax.org/en/v2.7-latest/configuration.html#configuring-mathjax
    Under default setting, all formulas are too large. I added `scale: 80` under "HTML-CSS" to fix this.
-->
<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js">
    MathJax.Hub.Config({
        extensions: ["tex2jax.js","TeX/AMSmath.js","TeX/AMSsymbols.js"],
        jax: ["input/TeX", "output/HTML-CSS"],
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
        },
        "HTML-CSS": {availableFonts: ["TeX"], scale: 80}
    });
</script>


<!-- _pages/publications.md -->
<div class="publications">

An up-to-date list is available on <a href='https://inspirehep.net/literature?q=a%20I.Papadimitriou.1'>iNSPIRE</a>

<h1 style="text-align: left;">preprints</h1>

{% bibliography -f {{ site.scholar.bibliography }} -q @*[category~=preprint]* %}

<h1 style="text-align: left;">refereed journals</h1>

{% bibliography -f {{ site.scholar.bibliography }} -q @*[category~=article]* %}

<h1 style="text-align: left;">refereed conference proceedings</h1>

 {% bibliography -f {{ site.scholar.bibliography }} -q @*[category~=proceedings]* %}

<h1 style="text-align: left;">theses</h1>

{% bibliography -f {{ site.scholar.bibliography }} -q @*[category~=thesis]* %}

</div>
