---
layout: archive
permalink: /music/
published: true
author_profile: true
categories: music
---

My Music related posts..
<div class="posts">
  {% for post in site.categories['music'] %}
    <article class="post">
      <a href="{{ post.url | post.relative_url }}" rel="permalink">{{ post.title }}</a>
      <br>
      {{ post.date | date: "%B %e, %Y" }}
        <p class="archive__item-excerpt" itemprop="description">{{ post.excerpt | markdownify | strip_html | truncate: 160 }}</p>
  
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">
          Read More
      </a>
    </article>
  {% endfor %}
</div>
