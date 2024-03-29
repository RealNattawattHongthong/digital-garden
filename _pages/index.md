---
layout: page
title: Home
id: home
permalink: /
---

# Welcome To Nattawatt Digital Garden! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
 Hi! I'm Nattawatt, I'm passionate about learning in public, building in the open, and sharing what I know with others.
</p>

This digital garden is a place for me to cultivate my thoughts, ideas, and projects. It's a work in progress, and I'm always adding to it.
<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
