---
title: News
permalink: "/allnews.html"
layout: textlay
excerpt: Allan Lab at Leiden University.
sitemap: false
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline | markdownify}}</p>
{% endfor %}
