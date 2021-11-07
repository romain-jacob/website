---
layout: page
menutitle: Blog
permalink: /blog/
---

# Blog

<ul class="post-list">
  {% for post in site.posts limit:5 %}
  {% if post.type == "blog" %}
  <li>
    <h2>{{ post.title }}
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span></h2>
    {{ post.content }}
  </li>
  {% endif %}
  {% endfor %}
</ul>
