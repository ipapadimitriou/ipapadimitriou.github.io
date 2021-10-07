---
title: ""
permalink: /index.html
layout: single
classes: wide
toc: false
sidebar:
    - nav: sitemap
    - nav: contact
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


<table style="width:100%">
<img src="./attachments/images/photo.jpeg" alt="" width="200" style="float:left"/>
</table>

<p>I am an Associate Professor in Mathematical Physics at the <a href="http://www.bimsa.cn/wzsy">Beijing Institute of Mathematical Sciences and Applications (BIMSA)</a> in Beijing, China. My research combines aspects of string theory, quantum field theory, and the remarkable mathematical relation between them known as holographic duality in order to probe the quantum nature of black holes and the exotic properties of strongly interacting quantum matter.</p>
