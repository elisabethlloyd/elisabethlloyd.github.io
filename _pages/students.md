---
published: true
layout: page
permalink: /students/
title: students
description:
nav: true
nav_order: 4
---

Here is a list of my students, past and present:

{% for student in site.data.students %}
<div class="student">
  <img src="{{ site.baseurl }}/assets/img/{{ student.image }}" alt="{{ student.name }}" style="width:150px;height:150px;">
  <h2><a href="{{ student.website }}">{{ student.name }}</a></h2>
  <p>{{ student.affiliation }}</p>
</div>
{% endfor %}
