---
layout: single
permalink: /blog
---

# Blog

<table>
{% for post in site.posts %}
{% if post.type == "blog" %}
  <tr>
      <td width="30%">
          <img src="{{post.image}}" alt="{{post.image_title}}">
      </td>
      <td>
        <a href="{% link {{ post.path }} %}">{{ post.title }}</a>
      </td>
  </tr>
{% endif %}
{% endfor %}
</table>