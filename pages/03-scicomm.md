---
layout: page
menutitle: Science Communication
permalink: /science-communication/
---

# Science Communication

As a scientist, I consider it is part of my job to communicate about what my research, to an audience as large as possible.

It is not about showing off.
I found that the vast majority of people is genuinely interested in science and research.

You will find here some of my attempts to tell a bit about what I do...

{% for post in site.posts %}{% if post.type == "scicomm" %}
- {{post.title}}{% endif %}{% endfor %}

{% for post in site.posts %}
{% if post.type == "scicomm" %}
## {{ post.title }}
{{post.content}}
{% endif %}
{% endfor %}
