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

## Current Students

<div class="row">
{% for student in site.data.students %}
  {% if student.status == "current" %}
  <div class="col-md-4 student">
    <div class="card mb-4 shadow-sm">
      <img class="bd-placeholder-img card-img-top img-fluid" style="width:100px;height:100px;" src="{{ site.baseurl }}/assets/img/{{ student.image }}" alt="{{ student.name }}">
      <div class="card-body">
        <h2 class="card-title"><a href="{{ student.website }}">{{ student.name }}</a></h2>
        <p class="card-text">{{ student.affiliation }}</p>
      </div>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>

## Past Students

<div class="row">
{% for student in site.data.students %}
  {% if student.status == "past" %}
  <div class="col-md-4 student">
    <div class="card mb-4 shadow-sm">
      <img class="bd-placeholder-img card-img-top img-fluid" style="width:100px;height:100px;" src="{{ site.baseurl }}/assets/img/{{ student.image }}" alt="{{ student.name }}">
      <div class="card-body">
        <h2 class="card-title"><a href="{{ student.website }}">{{ student.name }}</a></h2>
        <p class="card-text">{{ student.affiliation }}</p>
      </div>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>
