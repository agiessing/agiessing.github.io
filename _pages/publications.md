---
layout: page
permalink: /publications/
title: Publications
description: preprints and published articles in reverse chronological order
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[selected=true]* %}
          </div>


<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[selected=false]* %}
</div>

