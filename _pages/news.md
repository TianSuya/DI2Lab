---
title: "News"
layout: single
permalink: /news/
author_profile: true
---

{% for news in site.news reversed %}
  <h2><a href="{{ news.url }}">{{ news.title }}</a></h2>
  <p>{{ news.date | date: "%Y-%m-%d" }}</p>
  <p>{{ news.excerpt }}</p>
{% endfor %}