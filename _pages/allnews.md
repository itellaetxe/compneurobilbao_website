---
title: News
permalink: "/allnews.html"
layout: textlay
excerpt: CompNeuro Lab at IIS Biobizkaia
sitemap: false
---

# News


{% for article in site.data.news %}
<table style="width: 100%; margin-bottom: 20px;">
  <tr>
    <td style="width: 30%; padding-right: 20px;">
      <img src="{{ article.image }}" alt="News image" style="width: 100%;">
    </td>
    <td style="vertical-align: top;">
      <p><strong>{{ article.date }}</strong></p>
      <p>{{ article.headline | markdownify }}</p>
      <p>{{ article.description }}</p>
    </td>
  </tr>
</table>
{% endfor %}
