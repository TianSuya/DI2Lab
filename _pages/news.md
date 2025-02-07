---
title: "News"
layout: splash
permalink: /news/
header:
  overlay_image: https://tiansuya.github.io/DI2Lab/assets/home-1.jpg  # 背景图片路径
#   overlay_filter: rgba(0, 0, 0, 0.5)  # 背景图片的遮罩颜色
  caption: "Welcome to our latest news!"
  actions:
    - label: "View Latest Papers"
      url: "/publications/"
    - label: "Join Us"
      url: "/join/"
excerpt: "Keep up to date with the latest research results, events and news announcements from the lab here."
---

{% for news in site.news reversed %}
  <h2>{{ news.title }}</h2>
  <p>{{ news.date | date: "%Y-%m-%d" }}</p>
  <p>{{ news.excerpt }}</p>
{% endfor %}