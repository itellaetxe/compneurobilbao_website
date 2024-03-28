---
title: CompNeuro Lab - Team
permalink: "/team/"
layout: gridlay
excerpt: 'CompNeuro Lab: Team members'
sitemap: false
---

# Principal Investigators
{% assign number_printed = 0 %}
{% for member in site.data.pi %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <h4>{{ member.name }}</h4>
  <div class="social-icons">
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
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <ul style="overflow: hidden">
    {% if member.number_educ == 1 %}
    <li>{{ member.education1 }}</li>
    {% endif %}
    {% if member.number_educ >= 2 %}
    <li>{{ member.education1 }}</li>
    <li>{{ member.education2 }}</li>
    {% endif %}
    {% if member.number_educ >= 3 %}
    <li>{{ member.education3 }}</li>
    {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
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

<div class="section-space"></div> <!-- Espacio añadido aquí -->

# PhD students and Postdocs
{% assign number_printed = 0 %}
{% for member in site.data.phd_postdoc %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <h4>{{ member.name }}</h4>
  <div class="social-icons">
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
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <ul style="overflow: hidden">
    {% if member.number_educ == 1 %}
    <li>{{ member.education1 }}</li>
    {% endif %}
    {% if member.number_educ >= 2 %}
    <li>{{ member.education1 }}</li>
    <li>{{ member.education2 }}</li>
    {% endif %}
    {% if member.number_educ >= 3 %}
    <li>{{ member.education3 }}</li>
    {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
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

<div class="section-space"></div> <!-- Espacio añadido aquí -->

# Bachelor and Master Students

{% assign number_printed = 0 %}
{% for member in site.data.bachelor_master %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <div class="team-member">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" />
  </div>
  <div class="team-info">
  <div class="team-info-header">
  <h4>{{ member.name }}</h4>
  <div class="social-icons">
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
  {% if member.google_scholar %}
  <a href="{{ member.google_scholar }}" target="_blank" class="fab-icon">
    <i class="fab fa-google"></i>
  </a>
  {% endif %}
  </div>
  </div>
  <p><i>{{ member.info }}</i></p>
  <ul style="overflow: hidden">
    {% if member.number_educ == 1 %}
    <li>{{ member.education1 }}</li>
    {% endif %}
    {% if member.number_educ >= 2 %}
    <li>{{ member.education1 }}</li>
    <li>{{ member.education2 }}</li>
    {% endif %}
    {% if member.number_educ >= 3 %}
    <li>{{ member.education3 }}</li>
    {% endif %}
    <!-- Add more education levels if necessary -->
  </ul>
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


