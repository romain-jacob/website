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

## Students

<!-- [https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf](https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/courses.pdf) -->
<!-- <object data="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/students.pdf" type="application/pdf" width="100%" height="150px"> -->
<!-- <a href="https://nbviewer.jupyter.org/github/romain-jacob/doc_public/blob/main/students.pdf">Students list (PDF)</a> -->
<!-- </object> -->

> Doctoral [ D ], master [ M ] semester [ S ] and bachelor theses [ B ] that I (co-)supervised.  
> Undergraduate projects that led to a peer-reviewed publication are marked with <i class="fas fa-circle highlight"></i>.

<table>
{% for student in site.data.students.list -%}
    <tr>
        <td width="10%" style="text-align:right">{{student.year}}</td>
        <td width="10%" style="text-align:center">[ {{student.type}} ]</td>
        <td>{{student.name}}</td>
    </tr>
    {% if student.thesis-title -%}
    <tr>
        <td></td>
        <td style="text-align:center">{% if student.lead-to-pub %} <i class="fas fa-circle highlight"></i> {% endif %}</td>
        <td>
        <a href="{{student.thesis-url}}">{{student.thesis-title}}</a>
        </td>
    </tr>
    {% endif -%}
{%- endfor -%}
</table>