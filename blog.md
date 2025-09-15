---
layout: page
title: Blog
permalink: /blog/
---

# Software Development Blog

Welcome to my blog where I share insights, tutorials, and thoughts on software development, programming best practices, and industry trends.

---

{% for post in site.posts %}
<article class="blog-post-preview">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
  <a href="{{ post.url | relative_url }}">Read more →</a>
</article>
<hr>
{% endfor %}

{% if site.posts.size == 0 %}
<p>No posts yet. Check back soon for updates on software development, programming tips, and industry insights!</p>
{% endif %}