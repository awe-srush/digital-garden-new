---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱 Hi, I am Srushti 👋

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration of my mind.
</p>

This place is my collection of ever evolving ideas, contemplations, half-baked thoughts, strikes of genious merging into rounded wikis. Baring my second brain to the world is quite scary but public validation gets us going! 🙃

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
