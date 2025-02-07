---
title: "News"
layout: single
permalink: /news/
author_profile: false
---

{% for news in site.news reversed %}
  <h2>{{ news.title }}</h2>
  <p>{{ news.date | date: "%Y-%m-%d" }}</p>
  <p>{{ news.excerpt }}</p>
{% endfor %}