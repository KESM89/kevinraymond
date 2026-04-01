---
title: Archive
permalink: /archive/
description: Every post on the site.
---

{% if site.posts.size > 0 %}
<div class="archive-list">
  {% for post in site.posts %}
    <article class="archive-item">
      <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      {% if post.description %}
        <p>{{ post.description }}</p>
      {% endif %}
    </article>
  {% endfor %}
</div>
{% else %}
<p>No posts yet.</p>
{% endif %}
