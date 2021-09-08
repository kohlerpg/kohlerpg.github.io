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
  {% include archive-single.html %}
{% endfor %}
</ul>
