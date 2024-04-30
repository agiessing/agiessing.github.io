---
layout: default
permalink: /publications/
title: Research
description: preprints and published articles in reverse chronological order
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<h1 class="post-title"> Preprints </h1>
<p class="post-description"> &#x2A; Student Author </p>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=true]* %}
          </div>

<br>
<h1 class="post-title"> Journal & Conference Articles </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=false]* %}
</div>
