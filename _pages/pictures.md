---
title: CompNeuro Lab - Pictures
permalink: "/pictures/"
layout: default
excerpt: CompNeuro Lab -- Pictures
---

# Pictures
Jump to: [Group](#group), [Bilbao Brain Connectivity Workshop](#bilbao_brain_connectivity_workshop), [Conferences](#conferences), [NeuroTxoko Day](#NeuroTxoko_Day)


## Group
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/homepic/home1.jpg" width="60%" >
</figure>


## Workshops
### Bilbao Brain Connectivity Workshop
<img src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/Workshop.JPG" width="60%" >
#### Short video summarizing the workshop day 

<iframe width="560" height="315" src="https://www.youtube.com/embed/nBB1Ah6tvwU?si=yzyyHJi_uswJnJMk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


### 2023 DIPY
<img src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/DIPY.JPG" width="60%" >

## Conferences
### Organization for Human Brain Mapping (OHBM) 2022
(Right-click 'view image' to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/glasgow.JPG}" class="img-responsive" width="95%" style="float: left" />
<iframe width="560" height="315" src="https://www.youtube.com/embed/YimXs4zL4Cs?si=RHTmh7HoknfgRVSS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

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

###  European Cooperation in Science and Technology Conference (COSTNET) 2019
(Right-click 'view image' to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/glasgow.JPG}" class="img-responsive" width="95%" style="float: left" />

<iframe width="560" height="315" src="https://www.youtube.com/embed/4VrIX5HpacY?si=2qugljL9hCDabXyK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

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
<img src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/neurotxoko.JPG" width="60%" >

#### Short video summarizing the Neurotxoko day 
<video class="responsive-video" width="60%" height="60%" style="float: left" controls>
    <source src="{{ site.url }}{{ site.baseurl }}/images/gallerypic/neurotxoko_video.mp4" type="video/mp4">
    Tu navegador no soporta la etiqueta de video.
</video>