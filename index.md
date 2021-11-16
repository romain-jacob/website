---
layout: single
author_profile: true
---

> I'm currently migrating my personal webpage.  
> This is a work-in-progress. Sorry in advance for missing pieces and glitches!

I am a postdoctoral researcher at ETH Zurich in the group of [Prof. Laurent Vanbever](https://nsg.ee.ethz.ch/people/laurent-vanbever/). My current research interests are focused on computer networks, communication protocols, (real-time) scheduling theory, and statistics applied to experimental design.
You can find out more about my research interests and past activities in [my resume]() and [research page](/research).

In 2019, I completed my doctoral studies under the supervision of Prof. Lothar Thiele, also at ETH. My dissertation is entitled [Leveraging Synchronous Transmissions for the Design of Real-time Wireless Cyber-Physical Systems](https://github.com/romain-jacob/doctoral-thesis). Before joining ETH, I obtained a Master of Science in Engineering of Complex Systems (2015) and Master for Faculty Training for Higher Education (2013) both from École Normale Supérieure de Cachan (now ENS Paris-Saclay). In 2014, I spent a year in UC Berkeley as visiting scholar under the supervision of Prof. Karl Hedrick.

I am an [Open Science enthusiast](https://www.romainjacob.net/pledge-to-open-science/) and try to advocate for it whenever I can. When time allows, I am also involved in [science communication](http://www.romainjacob.net/science-communication/) projects.

## Want to find out more about me?

- [Resumé](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/cv_narrative.pdf) (narrative, short)
<!-- - [Research statement](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/research.pdf) -->
- [Teaching statement](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/teaching.pdf)
<!-- - [Publications](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/publications.pdf) -->

## Highlights

<table>
{% for post in site.posts limit:50 %}
{% if post.type == "news" %}
  <tr>
      <td width="12%">
          <span class="post-meta">{{ post.date | date: "%Y %b" }}</span>
      </td>
      <td> 
        {{ post.title }}
      </td>
      <td rowspan="2" width="15%" class="image_column bottom_row">
        {% if post.image %}
        <a href="{{post.image_link}}"><img src="{{post.image}}" alt="{{post.image_title}}"></a>
        {% endif %}
      </td>
  </tr>
  <tr>
      <td></td>
      <td width="58%" class="bottom_row">
          {{ post.content }}
      </td>
  </tr>
{% endif %}
{% endfor %}
</table>
