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
    <img src="{{ article.image }}" alt="News image" style="max-width: 200px; height: auto; display: block;">
  </div>
  <div style="flex-grow: 1;">
    <h3>{{ article.date }}</h3>
    <h4>{{ article.headline }}</h4> <!-- Removed the markdownify filter -->
    <h5>{{ article.description }}</h5>
  </div>
</div>
{% endfor %}



