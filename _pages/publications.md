---
layout: page
permalink: /publications/
title: Publications
description: publications and pre-prints in reverse chronological order
nav: true
nav_order: 2
---

<article>
<!-- _pages/publications.md -->
<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} %}


 <!-- Selected papers -->
          {% if page.selected_papers -%}
            <h2><a href="{{ '/publications/' | relative_url }}" style="color: inherit;">selected publications</a></h2>
            {%- include selected_papers.html %}
          {%- endif %}

</div>
</article>
