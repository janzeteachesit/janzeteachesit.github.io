---
layout: default
title:  "Table of Contents"
creation date:   2017-02-03 19:45:00 -0800
post_variable: footer.html
description: list of blog posts
---

<div id="posts">
  <h1>Table of Contents</h1>
  <ul>
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>


<div id="pages">
  <h2>Pages</h2>
  <ul>
    {% for page in site.html_pages %}
      {% if page.title %}
        <li><a href="{{ page.url }}">{{ page.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

[contact](./contact.md) | [other](./other.md) | [about](./about.md)

