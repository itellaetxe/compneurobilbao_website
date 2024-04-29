---
title: News
permalink: "/allnews.html"
layout: textlay
excerpt: CompNeuro Lab at IIS Biobizkaia
sitemap: false
---

# News



{% for article in site.data.news %}
<div style="display: flex; align-items: flex-start; margin-bottom: 20px;">
  <div style="margin-right: 20px;">
    <img src="{{ article.image }}" class="img-responsive">
  </div>
  <div style="flex-grow: 1;">
    <p><strong>{{ article.date }}</strong></p>
    <p>{{ article.headline | markdownify }}</p>
    <p>{{ article.description }}</p>
  </div>
</div>
{% endfor %}
