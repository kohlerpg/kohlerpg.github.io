---
layout: archive
permalink: /music/
published: true
author_profile: true
---

<ul>
  {% for post in site.categories.music %}
    {% if post.url %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
