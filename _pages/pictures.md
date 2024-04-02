---

title: "CompNeuro Lab - Pictures"
layout: default
excerpt: "CompNeuro Lab -- Pictures"
permalink: /pictures/

---

# Pictures
Jump to: [Group](#group), [Bilbao Brain Connectivity Workshop](#workshop), [Conferences](#conferences), [NeuroTxoko](#neurotxoko)


## Group
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/homepic/home1.jpg" width="60%" >
</figure>


## Bilbao Brain Connectivity Workshop
#### Short video summarizing the workshop day 
<iframe width="560" height="315" src="https://youtu.be/nBB1Ah6tvwU?si=JPHPeh43LIbsBwDz" frameborder="0" allowfullscreen></iframe>

## Conferences
### Organization for Human Brain Mapping (OHBM) 2022
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

### ISMRM Iberian Chapter Annual Meeting 2023

(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

## NeuroTxoko Day