---
title: News
permalink: "/allnews.html"
layout: textlay
excerpt: CompNeuro Lab at IIS Biobizkaia
sitemap: false
---

# News

{% for article in site.data.news %}
<div style="display: flex; margin-bottom: 20px;">
  <div style="flex: 1; margin-right: 20px;">
    <img src="{{ article.image }}" alt="News image" style="width: 100%;">
  </div>
  <div style="flex: 2;">
    <p><strong>{{ article.date }}</strong><br>{{ article.headline | markdownify }}</p>
    <p>{{ article.description }}</p>
  </div>
</div>
{% endfor %}
