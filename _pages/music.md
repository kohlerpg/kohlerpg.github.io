---
permalink: /music/
published: true
layout: archive
author_profile: true
title: Music
subtitle: Music found in various places
---



<ul>
  {% for post in site.categories.music %}
    {% if post.url %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
