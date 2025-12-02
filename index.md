---
layout: default
title: Weekly Reports
---

<style>
.wrapper {
    max-width: 1000px;
    width: 90%;
}
</style>

# Weekly Reports
<ul>
  {% for post in site.posts %}
    {% if post.tags contains "weekly" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>— {{ post.date | date: "%b %d, %Y" }}</small>
      </li>
    {% endif %}
  {% endfor %}
</ul>

# Files
[Requirements + Testing Plan](files/requirements-and-testing.xlsx)
