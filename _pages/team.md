---
title: CompNeuro Lab - Team
permalink: "/team/"
layout: gridlay
excerpt: 'CompNeuro Lab: Team members'
sitemap: false
---

<!-- JavaScript to toggle the visibility of team member details -->
<script type="text/javascript">
  // Function to toggle the display of detailed information
  function toggleDetails(memberId) {
    var details = document.getElementById(memberId);
    details.style.display = details.style.display === 'block' ? 'none' : 'block';
  }
</script>

# Team Members
Meet the minds behind our research! Our dedicated team spans [Principal Investigators](#principal-investigators), [Postdoctoral Researchers](#postdocs), [PhD Students](#phd-students), [Bachelor and Master Students](#bachelor-and-master-students) , and [Esteemed Alumni](#alumni), all collaborating to advance the frontiers of computational neuroimaging."

Jump to: [Group](#group), [Workshops](#workshops), [Conferences](#conferences), [NeuroTxoko Day](#neurotxoko-day)

# Principal Investigators
{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <!-- The name is now a clickable element that calls toggleDetails with the appropriate ID -->
  <h4 id="header-{{ member.name | slugify }}" onclick="toggleDetails('details-{{ member.name | slugify }}', 'header-{{ member.name | slugify }}')">{{ member.name }}</h4>  <div class="social-icons">
  {% if member.user %}
  <a href="{{ member.user }}" target="_blank" class="fab-icon">
  <i class="fa fa-user" aria-hidden="true"></i>
  </a>
  {% endif %}
  {% if member.twitter %}
  <a href="{{ member.twitter }}" target="_blank" class="fab-icon">
    <i class="fab fa-twitter"></i>
  </a>
  {% endif %}
  {% if member.linkedin %}
  <a href="{{ member.linkedin }}" target="_blank" class="fab-icon">
    <i class="fab fa-linkedin"></i>
  </a>
  {% endif %}
  {% if member.orcid %}
  <a href="{{ member.orcid }}" target="_blank" class="fab-icon">
    <i class="fab fa-orcid"></i>
  </a>
  {% endif %}
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  {% if member.github %}
  <a href="{{ member.github }}" target="_blank" class="fab-icon">
  <i class="fab fa-github"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <!-- The detailed information is initially hidden and has an ID that corresponds to the member's name -->
  <div id="details-{{ member.name | slugify }}" style="display: none;">
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
  {% endif %}
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
  </div>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<div class="section-space"></div>
<div class="section-space"></div> <!-- Espacio añadido aquí -->
<div class="section-space"></div> <!-- Espacio añadido aquí -->

<!-- ... Further content ... -->


# Postdocs
{% assign number_printed = 0 %}
{% for member in site.data.postdoc %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <!-- The name is now a clickable element that calls toggleDetails with the appropriate ID -->
  <h4 id="header-{{ member.name | slugify }}" onclick="toggleDetails('details-{{ member.name | slugify }}', 'header-{{ member.name | slugify }}')">{{ member.name }}</h4>  <div class="social-icons">
  {% if member.user %}
  <a href="{{ member.user }}" target="_blank" class="fab-icon">
  <i class="fa fa-user" aria-hidden="true"></i>
  </a>
  {% endif %}
  {% if member.twitter %}
  <a href="{{ member.twitter }}" target="_blank" class="fab-icon">
    <i class="fab fa-twitter"></i>
  </a>
  {% endif %}
  {% if member.linkedin %}
  <a href="{{ member.linkedin }}" target="_blank" class="fab-icon">
    <i class="fab fa-linkedin"></i>
  </a>
  {% endif %}
  {% if member.orcid %}
  <a href="{{ member.orcid }}" target="_blank" class="fab-icon">
    <i class="fab fa-orcid"></i>
  </a>
  {% endif %}
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  {% if member.github %}
  <a href="{{ member.github }}" target="_blank" class="fab-icon">
  <i class="fab fa-github"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <!-- The detailed information is initially hidden and has an ID that corresponds to the member's name -->
  <div id="details-{{ member.name | slugify }}" style="display: none;">
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
  {% endif %}
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
  </div>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<div class="section-space"></div>
<div class="section-space"></div> <!-- Espacio añadido aquí -->
<div class="section-space"></div> <!-- Espacio añadido aquí -->

<!-- ... Further content ... -->


# PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <!-- The name is now a clickable element that calls toggleDetails with the appropriate ID -->
  <h4 id="header-{{ member.name | slugify }}" onclick="toggleDetails('details-{{ member.name | slugify }}', 'header-{{ member.name | slugify }}')">{{ member.name }}</h4>  <div class="social-icons">
  {% if member.user %}
  <a href="{{ member.user }}" target="_blank" class="fab-icon">
  <i class="fa fa-user" aria-hidden="true"></i>
  </a>
  {% endif %}
  {% if member.twitter %}
  <a href="{{ member.twitter }}" target="_blank" class="fab-icon">
    <i class="fab fa-twitter"></i>
  </a>
  {% endif %}
  {% if member.linkedin %}
  <a href="{{ member.linkedin }}" target="_blank" class="fab-icon">
    <i class="fab fa-linkedin"></i>
  </a>
  {% endif %}
  {% if member.orcid %}
  <a href="{{ member.orcid }}" target="_blank" class="fab-icon">
    <i class="fab fa-orcid"></i>
  </a>
  {% endif %}
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  {% if member.github %}
  <a href="{{ member.github }}" target="_blank" class="fab-icon">
  <i class="fab fa-github"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <!-- The detailed information is initially hidden and has an ID that corresponds to the member's name -->
  <div id="details-{{ member.name | slugify }}" style="display: none;">
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
  {% endif %}
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
  </div>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<div class="section-space"></div>
<div class="section-space"></div> <!-- Espacio añadido aquí -->
<div class="section-space"></div> <!-- Espacio añadido aquí -->

<!-- ... Further content ... -->


# Bachelor and Master Students

{% assign number_printed = 0 %}
{% for member in site.data.bachelor_master %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <!-- The name is now a clickable element that calls toggleDetails with the appropriate ID -->
  <h4 id="header-{{ member.name | slugify }}" onclick="toggleDetails('details-{{ member.name | slugify }}', 'header-{{ member.name | slugify }}')">{{ member.name }}</h4>  <div class="social-icons">
  {% if member.user %}
  <a href="{{ member.user }}" target="_blank" class="fab-icon">
  <i class="fa fa-user" aria-hidden="true"></i>
  </a>
  {% endif %}
  {% if member.twitter %}
  <a href="{{ member.twitter }}" target="_blank" class="fab-icon">
    <i class="fab fa-twitter"></i>
  </a>
  {% endif %}
  {% if member.linkedin %}
  <a href="{{ member.linkedin }}" target="_blank" class="fab-icon">
    <i class="fab fa-linkedin"></i>
  </a>
  {% endif %}
  {% if member.orcid %}
  <a href="{{ member.orcid }}" target="_blank" class="fab-icon">
    <i class="fab fa-orcid"></i>
  </a>
  {% endif %}
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  {% if member.github %}
  <a href="{{ member.github }}" target="_blank" class="fab-icon">
  <i class="fab fa-github"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <!-- The detailed information is initially hidden and has an ID that corresponds to the member's name -->
  <div id="details-{{ member.name | slugify }}" style="display: none;">
  <ul style="overflow: hidden">
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}
  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
  {% endif %}
  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}
  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}
  {% if member.number_educ == 6 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  <li> {{ member.education6 }} </li>
  {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
  </div>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<div class="section-space"></div>
<div class="section-space"></div> <!-- Espacio añadido aquí -->
<div class="section-space"></div> <!-- Espacio añadido aquí -->

<!-- ... Further content ... -->


# Alumni
{% assign number_printed = 0 %}
{% for member in site.data.previous_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> {{ member.info }}</i>
  <ul style="overflow: hidden"> </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


