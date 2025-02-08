---
layout: page
title: Publications
permalink: /publication/
---

See [here](https://scholar.google.com/citations?user=4vbLax8AAAAJ&hl=en) for a full-list of all publications.

# Selected Publications :

Note: (α-β) indicates alphabetical ordering

<ul>
  {% for pub in site.data.publications %}
    <li>
      <strong>{{ pub.title }}</strong> <br>
      <em>{{ pub.authors }}</em><br>
      {{ pub.venue }} ({{ pub.year }}) <br>
      {% if pub.link %}
        <a href="{{ pub.link }}">[Paper Link]</a>
      {% endif %}
      {% if pub.code_link %}
        <a href="{{ pub.code_link }}">[Code]</a>
      {% endif %}
      {% if pub.description %}
        <p>{{ pub.description }}</p>
      {% endif %} 
    </li><br>
  {% endfor %}
</ul>
