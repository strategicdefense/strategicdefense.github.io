---
layout: blog
title: Blog
permalink: /blog/
description: The best defense is a good offense.
image: "images/illustrations/colorfulcomputer.webp"
---


<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
      <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
      {{ post.excerpt }}
  {% endfor %}
</ul>


