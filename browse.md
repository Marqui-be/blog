---
layout: default
title: Browse
---

# Browse

This page lists all published notes.

You can use your browser search (Ctrl / Cmd + F) to find specific topics.

---

## Meta
{% for page in site.pages %}
  {% if page.path contains "notes/meta/" %}
- [{{ page.title }}]({{ page.url }})
  {% endif %}
{% endfor %}

---

## Systems
{% for page in site.pages %}
  {% if page.path contains "notes/systems/" %}
- [{{ page.title }}]({{ page.url }})
  {% endif %}
{% endfor %}

---

## 2026
{% for page in site.pages %}
  {% if page.path contains "notes/2026/" %}
- [{{ page.title }}]({{ page.url }})
  {% endif %}
{% endfor %}
