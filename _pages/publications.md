---
layout: default
permalink: /publications/
title: Publications
description: preprints and published articles in reverse chronological order
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<h1 class="post-title"> Preprints </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=true]* %}
          </div>

<br>
<h1 class="post-title"> Journal and Conference Articles </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=false]* %}
</div>

