---
layout: splash
title: "DI²Lab Blogs"
permalink: /blogs/
header:
  image: "https://tiansuya.github.io/DI2Lab/assets/home-1.jpg"  # 可以使用实验室相关的头图
  caption: "Welcome to our lab blog!"
  excerpt: "We will share interesting information about DI²Lab here!"
---

{% include base_path %}

<div class="grid__wrapper">
  {% for post in site.posts %}
    {% if post.categories contains 'blog' %}  <!-- 假设你的博客都包含blog分类 -->
      {% include archive-single.html type="grid" %}
    {% endif %}
  {% endfor %}
</div>