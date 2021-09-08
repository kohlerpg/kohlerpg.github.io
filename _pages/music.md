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
      {% capture year %}{{ post.date | date: '%Y %b' }}{% endcapture %}
      {% capture nyear %}{{ post.next.date | date: '%Y %b' }}{% endcapture %}
    {% endif %}
  {% endfor %}
</ul>
