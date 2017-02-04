
---

layout: page
title:  "Table of Contents"
creation date:   2017-02-03 19:45:00 -0800
post_variable: footer.html

---

# Table of Contents

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% include {{ page.post_variable }} %}

