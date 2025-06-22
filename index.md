---
layout: layout.njk
title: "Welcome"
---

<p style="font-size: 1.2em; line-height: 1.8;">
  This is a quiet corner of the web for anonymous writing — thoughts on philosophy, startups, economics, books, and life.
</p>

<hr>

<h2>Writings</h2>
<ul>
  {% for post in collections.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.data.title }}</a>
      <small>({{ post.date | date: "%b %d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>
