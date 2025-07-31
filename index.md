---
layout: page
title: Small Systems, Big Lessons
---

Every weekend, I build a small project to explore ideas, sharpen my skills, or just follow a hunch. Sometimes it’s a quick prototype. Sometimes it turns into a deep dive. Either way, I document what I learned — and where I’d take it next.

This site is a growing log of those projects. Think of it as a public engineering journal, experiment archive, and reflection space.

---

## 🛠️ Projects

<ul>
  {% assign sorted_projects = site.projects | sort: 'order' %}
  {% for project in sorted_projects %}
    <li>
      <a href="{{ project.url }}">{{ project.title }}</a> — {{ project.summary }}
    </li>
  {% endfor %}
</ul>
