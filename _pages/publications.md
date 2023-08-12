---
layout: page
permalink: /publications/
title: # Publications
description: # preprints and published articles in reverse chronological order
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

Preprints
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=true]* %}
          </div>

Journal and Conference Articles
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[preprint=false]* %}
</div>

