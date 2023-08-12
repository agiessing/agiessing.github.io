---
layout: none # page
permalink: /publications/
title: Publications
description: preprints and published articles in reverse chronological order
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<h2 class="post-title"> Preprints </h2>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=true]* %}
          </div>

<br>
<h2 class="post-title"> Journal and Conference Articles </h2>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=false]* %}
</div>

