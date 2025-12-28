---
layout: page
title: (A)Dock News
permalink: /news/
---
<ul>
  {% for post in site.posts %}
    {% if post.published != false %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>({{ post.date | date: "%B %d, %Y" }})</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>
