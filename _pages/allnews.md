---
title: News
permalink: "/allnews/"
layout: textlay
excerpt: CompNeuro Lab at IIS Biobizkaia
sitemap: false
---

# News

{% for article in site.data.news %}
<div style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <div style="margin-right: 20px;">
  <img src="{{ site.url }}{{ site.baseurl }}/images/newspic/{{ article.image }}" style="max-width: 250px; height: auto; display: block;">
  </div>
  <div style="flex-grow: 1;">
  <h3>{{ article.headline }}</h3>
  <h4>{{ article.date }}</h4> 
  <h5>{{ article.description }}</h5>
  </div>
</div>
{% endfor %}



