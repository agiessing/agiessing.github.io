---
layout: default
permalink: /teaching/
title: Teaching
description:
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<h1 class="post-title"> Courses </h1>
<div class="publications">
            {% bibliography -f {{ site.scholar.bibliography }} -q @*[course=true]* %}
          </div>
