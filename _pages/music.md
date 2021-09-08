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
        <font color="#778899"><h2>{{ post.date | date: '%Y %b' }}</h2></font>
      {% endif %}
   {% include archive-single.html %}
  {% endfor %}
