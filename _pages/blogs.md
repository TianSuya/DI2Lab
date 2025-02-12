---
layout: splash
title: "DI²Lab Blogs"
permalink: /blogs/
header:
  overlay_image: "https://tiansuya.github.io/DI2Lab/assets/home-1.jpg"  # 可以使用实验室相关的头图
  caption: "Welcome to our lab blog!"
excerpt: "We will share interesting information about DI²Lab here!"
---

{% for post in site.blogs reversed %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
{% endfor %}