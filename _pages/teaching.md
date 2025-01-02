---
layout: page
title: teaching
permalink: /teaching/
description: A collection of classes, workshops, tutorials, and teaching materials
nav: true
nav_order: 6
---

<div class="container">
  {% for course in site.teaching %}
    <div class="card mt-3">
      <div class="p-3">
        <div class="row">
          <div class="col-sm-10">
            <h5 class="font-weight-bold">
              <a href="{{ course.url }}">{{ course.course_code }}: {{ course.title }}</a>
            </h5>
          </div>
          <div class="col-sm-2 text-left text-sm-right">
          </div>
        </div>
        <h6 class="font-italic mt-2 mt-sm-0">
          {{ course.semester }}
        </h6>
        <p>{{ course.description }}</p>
      </div>
    </div>
  {% endfor %}
</div>