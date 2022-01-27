---
layout: single
permalink: /teaching
---

# Teaching

I'm really passionate about teaching, it is one of my favorite activities is my work as an academic!
On this page, you'll find lists of the courses I've been involved in and the students I supervised.

To learn more about my teaching philosophy, have a look at my [teaching statement](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/teaching.pdf).

## Courses

<!-- [https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf) -->
<!-- <object data="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf" type="application/pdf" width="100%" height="150px">
<a href="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf">Courses list (PDF)</a>
</object> -->


<table class="large_skip">
{% for course in site.data.courses.list -%}
    <tr>
        <td style="text-align:right;">{{course.years}}&nbsp;&nbsp;&nbsp;&nbsp;</td>
        <td style="white-space:pre;">{{course.title}}
<span class="muted">{{course.place}}</span>
{{course.position}}{%- if course.details %}<span class="muted"> -- {{course.details}}</span>{%- endif %}</td>
    </tr>
{%- endfor -%}
</table>

## Students

<!-- [https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf) -->
<!-- <object data="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/students.pdf" type="application/pdf" width="100%" height="150px"> -->
<!-- <a href="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/students.pdf">Students list (PDF)</a> -->
<!-- </object> -->

> Doctoral [ D ], master [ M ] semester [ S ] and bachelor theses [ B ] that I (co-)supervised.  
> Undergraduate projects that led to a peer-reviewed publication are marked with <i class="fas fa-circle highlight"></i>.

<table class="large_skip">
{% for student in site.data.students.list -%}
    <tr>
        <td width="10%" style="text-align:right;">{{student.year}}</td>
        <td width="10%" style="text-align:center; white-space:pre;" class="muted">[ {{student.type}} ]{% if student.thesis-title %}
{%if student.lead-to-pub%}<i class="fas fa-circle highlight"></i>{%endif%}
{%endif%}</td>
        <td style="white-space:pre">{{student.name}}
{% if student.thesis-title %}<a href="{{student.thesis-url}}">{{student.thesis-title}}</a>{%endif%}</td>
    </tr>
{%- endfor -%}
</table>