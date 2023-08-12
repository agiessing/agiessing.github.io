---
layout: page
permalink: /contact/
title: Contact
description: 
nav: true
nav_order: 4
---
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

/* Create two unequal columns that floats next to each other */
.column {
  float: left;
  padding: 10px;
  height: 300px; /* Should be removed. Only for demonstration */
}

.left {
  width: 25%;
}

.right {
  width: 75%;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}
</style>
</head>
<body>

<div class="row">
  <div class="column left">
    <p> <span class="font-weight-bold">E-mail:</span> <br>
    giessing@uw.edu </p>
    
    <p> <span class="font-weight-bold">Office:</span> <br>
    B-308 Padelford Hall <br>
    4110 E Stevens Way NE <br>
    Seattle, WA 98195 </p>
    
    <p> <span class="font-weight-bold">Mailing address:</span> <br>
    Alexander Giessing <br>
    University of Washington <br>
    Department of Statistics <br>
    Box 354322 <br>
    Seattle, WA 98195 </p>
  </div>
  <div class="column right">

      <!-- Calendly inline widget begin -->
      <div class="calendly-inline-widget" data-url="https://calendly.com/giessing-7xc/30min?hide_gdpr_banner=1" style="min-width:320px;height:1500px;"></div>
      <script type="text/javascript" src="https://assets.calendly.com/assets/external/widget.js" async></script>
      <!-- Calendly inline widget end -->
    
  </div>
</div>

<div class="social">
  <div class="contact-icons">
    {% include social.html %}
  </div>

  <div class="contact-note">
    {{ site.contact_note }}
  </div>

</div>

</body>
