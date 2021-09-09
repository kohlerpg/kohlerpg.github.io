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
      <h3>
          <a href="{{ post.url | post.relative_url }}" rel="permalink">{{ post.title }}</a></h3>
          <br>
          <p class="post_date">{{ post.date | date: "%B %e, %Y" }}</p>
      
      
        <p class="archive__item-excerpt" itemprop="description">{{ post.excerpt | markdownify | strip_html | truncate: 160 }}</p>
  
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">
          Read More
      </a>
    </article>
  {% endfor %}
</div>
