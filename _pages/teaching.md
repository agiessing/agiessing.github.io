---
layout: page
permalink: /teaching/
title: Teaching
description:
nav: true
nav_order: 3
---

<hr> 

<div class="row">
      <div class="col-sm-1 publication">
        {%- if entry.preview -%}
          {% if entry.preview contains '://' -%}
          <img data-zoomable class="preview z-depth-1 rounded" src="{{ entry.preview }}">
          {%- else -%}
            {%- assign entry_path = entry.preview | prepend: '/assets/img/publication_preview/' -%}
            {% include figure.html
            path=entry_path
            class="preview z-depth-1 rounded"
            zoomable=true
            alt=entry.preview -%}
          {%- endif -%}
        {%- elsif entry.abbr -%}
          {%- if site.data.venues[entry.abbr] -%}
            {%- assign venue_style = nil -%}
            {%- if site.data.venues[entry.abbr].color != blank -%}
              {%- assign venue_style = site.data.venues[entry.abbr].color | prepend: 'style="background-color:' | append: '"' -%}
            {%- endif -%}
            <abbr class="badge" {% if venue_style %}{{venue_style}}{% endif %}><a href="{{site.data.venues[entry.abbr].url}}">{{entry.abbr}}</a></abbr>
          {%- else -%}
            <abbr class="badge">{{entry.abbr}}</abbr>
          {%- endif -%}
        {%- endif -%}
            </div>
            <div class="col-sm-9 publication">
                  <p> <span class="font-weight-bolder">STAT 591: Gaussian and Empirical Process Theory for High-Dimensional Data </span> <br>
                        Spring 2023, University of Washington and Pacific Institute for the Mathematical Sciences <a href = "https://www.pims.math.ca" target="_new">(PIMS)</a> <br>
                        <a href="/assets/pdf/STAT 591 - Syllabus.pdf" target="_new"> Syllabus</a>, <a href="https://courses.pims.math.ca/tag/2022-2023/" target="_new">Syllabus PIMS</a>, <a href="https://canvas.uw.edu/courses/1635483" target="_new"> Class Webpage</a> </p>
                   <p>  <span class="font-weight-bolder">STAT 516: Stochastic Modeling of Scientific Data I</span> <br>
                        Fall 2023, University of Washington <br>
                        Syllabus, Class Webpage</p>
                  <p> <span class="font-weight-bolder">  STAT/ MATH 394: Probability I </span> <br> 
                        Spring 2022, University of Washington <br>
                        <a href="/assets/pdf/STAT 394 - Syllabus.pdf" target="_new"> Syllabus</a>, <a href="https://canvas.uw.edu/courses/1548372" target="_new"> Class Webpage</a> </p>
                  <p> <span class="font-weight-bolder"> STAT 390: Statistical Methods in Engineering and Science </span> <br>
                        Fall 2021, 2022, 2023, Winter 2022, 2023, Spring 2022, 2023, University of Washington <br>
                        <a href="/assets/pdf/STAT 390 - Syllabus - long version-2.pdf" target="_new"> Syllabus</a>, <a href="https://canvas.uw.edu/courses/1635461" target="_new"> Class Webpage</a> </p>
                  <p> <span class="font-weight-bolder"> ORF 245: Fundamentals of Statistics </span> <br>
                        Spring 2019, Princeton University<br>
                        <a href="/assets/pdf/ORF 245_Syllabus_Updated.pdf" target="_new"> Syllabus</a></p>
                  <p> <span class="font-weight-bolder"> Workshop on Empirical Process Theory </span> <br>
                        December 2018, Nankai University <br>
                        <a href="https://stat.nankai.edu.cn/2018/1126/c12333a129526/page.htm" target="_new"> Syllabus</a>, <a href=" /assets/pdf/empirical-proc-all-lectures.pdf" target="_new"> Lecture Notes</a> </p>
            </div>
      </div>
<br>

<h1 class="post-title"> Lecture Notes </h1>
<ul class="card-text font-weight-light list-group list-group-flush"> 
      <li class="list-group-item"> 
      <p> <a href=" /assets/pdf/empirical-proc-all-lectures.pdf" class="font-weight-bolder" target="_new"> Lectures on Empirical Process Theory</a> <br>
             <span class="font-weight-bolder"> Gaussian and Empirical Process Theory for High-Dimensional Data </span> (in progress, check back in October) </p>
      </li>
</ul>

