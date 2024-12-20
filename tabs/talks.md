---
layout: page
title: Talks
permalink: /talks/
---

# Recent Talks :

<ul>
  {% for talk in site.data.talks %}
    <li>
      <strong>{{ talk.title }}</strong> <br>
      <em>{{ talk.event }}</em> <br>
      <span>{{ talk.date | date: "%B %d, %Y" }} - {{ talk.location }}</span> <br>
      {% if talk.link %}
        <a href="{{ talk.link }}">[Slides]</a>
      {% endif %}
      {% if talk.description %}
        <p>{{ talk.description }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>