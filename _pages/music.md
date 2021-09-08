---
layout: archive
permalink: /music/
published: true
author_profile: true
---

My Music related posts..
<ul> 
  {% for post in site.categories.music %}
    {% if post.url %}
      <font color="#778899"><h2>{{ post.date | date: '%Y %b' }}</h2></font>
  <a href="{{ post.url}}">{{ post.title }}</a>
    {% endif %}
  {% endfor %}
</ul>
