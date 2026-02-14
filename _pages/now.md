---
layout: single
author_profile: false
permalink: /now/
classes: wide
title: What I'm Doing Now
---

##  Things I'm currently working on

{% if page.last_modified_at %}
  <p class="page__date"><strong>{{ site.data.ui-text[site.locale].date_label | default: "Updated:" }}</strong> <time datetime="{{ page.last_modified_at | date: "%Y-%m-%d" }}">{{ page.last_modified_at | date: "%B %d, %Y" }}</time></p>
{% elsif page.date %}
  <p class="page__date"><strong>{{ site.data.ui-text[site.locale].date_label | default: "Updated:" }}</strong> <time datetime="{{ page.date | date_to_xmlschema }}">{{ page.date | date: "%B %d, %Y" }}</time></p>
{% endif %}
