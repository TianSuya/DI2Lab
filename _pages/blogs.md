---
layout: splash
title: "DI²Lab Blogs"
permalink: /blogs/
header:
  image: "https://tiansuya.github.io/DI2Lab/assets/home-1.jpg"  # 可以使用实验室相关的头图
  caption: "Welcome to our lab blog!"
  excerpt: "We will share interesting information about DI²Lab here!"
---

{% for post in site.posts reversed %}
  <h2>{{ post.title }}</h2>
  <p>{{ post.date | date: "%Y-%m-%d" }}</p>
  <p>{{ post.excerpt }}</p>
{% endfor %}