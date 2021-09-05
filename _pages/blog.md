---
title: Blogs
layout: posts
permalink: /posts/
author_profile: true
comments: true
published: true
---

##  My Blog Page
Here is were all the posts will go.
{% for post in paginator.posts %}
  {% include posts-tag.html %}
{% endfor %}
