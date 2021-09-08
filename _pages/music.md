---
layout: archive
permalink: /music/
published: true
author_profile: true
---


{% for post in site.categories.music %}
      {% capture year %}{{ post.date | date: '%Y %b' }}{% endcapture %}
      {% capture nyear %}{{ post.next.date | date: '%Y %b' }}{% endcapture %}
      {% if year != nyear %}
        <h2>{{ post.date | date: '%Y %b' }}</h2>
      {% endif %}
   {% include archive-single.html %}
  {% endfor %}
