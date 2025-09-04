---
layout: default
title: archive
permalink: /archive/
---

# all writings

<ul>
{% assign posts_sorted = site.posts | sort: "date" | reverse %}
{% for post in posts_sorted %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="muted small">— {{ post.date | date: "%B %d, %Y" }}</span>
  </li>
{% endfor %}
</ul>
