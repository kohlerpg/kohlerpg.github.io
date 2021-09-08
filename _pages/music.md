---
layout: archive
permalink: /music/
published: true
author_profile: true
---

<ul>
  {% for post in site.categories.music %}
    {% if post.url %}
        {{post.date}}
        <li><a href="{{ post.url }}">{{ post.title }}</a>{{post.excerpt}</li>
    {% endif %}
  {% endfor %}
</ul>
