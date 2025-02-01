---
layout: page
title: Services
permalink: /services/
---

# Academic Services :

<ul>
  {% for course in site.data.services %}
    <li>
      <strong>{{ course.course }}</strong> ({{ course.term }}) <br>
      <em>{{ course.role }}, {{ course.institution }}</em> <br>
      {% if course.description %}
        <p>{{ course.description }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
