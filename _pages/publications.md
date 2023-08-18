---
layout: default
permalink: /publications/
title: Publications
description: preprints and published articles in reverse chronological order
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<h1 class="post-title"> Preprints </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=true]* %}
          </div>

<br>
<h1 class="post-title"> Journal Articles & Conference Proceedings </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=false]* %}
</div>

