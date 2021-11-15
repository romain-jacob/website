---
layout: single
permalink: /sci-comm
pagination: 
  enabled: true
---

<h1>Science Communication</h1>

<p>
As a scientist, I consider it is part of my job to communicate about what my research, to an audience as large as possible.
<br/>
It is not about showing off.
I found that the vast majority of people is genuinely interested in science and research.
</p>

<p>
You will find here some of my attempts to tell a bit about what I do...
</p>

<ul>
{% for post in paginator.posts %}{% if post.type == "scicomm" %}
  <li>{{ post.title }}</li>{% endif %}{% endfor %}
</ul>

{% for post in paginator.posts  %}
<!-- {% if post.type == "scicomm" %} -->
  {{ post.content }}
<!-- {% endif %} -->
{% endfor %}

<!-- {% for entry in include.scicomm %}
- {% include {{entry.title}} %}{% endfor %}


{% for post in site.data.scicomm %}
## {{ post.title }}
{{post.content}}
{% endfor %} -->
