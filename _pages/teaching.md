---
layout: default
permalink: /teaching/
title: Teaching
description:
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<h1 class="post-title"> Preprints </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[class=true]* %}
          </div>
