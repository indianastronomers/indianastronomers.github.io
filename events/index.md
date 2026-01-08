---
layout: default
title: Events
---

# Events

This page lists events in reverse chronological order. Each event page contains details including speaker, abstract, date/time, format, and links to recordings or slides when available.

{% raw %}{% assign events = site.pages | where: "event", true | sort: "date" | reverse %}{% endraw %}

{% raw %}{% if events.size > 0 %}{% endraw %}
{% raw %}{% for e in events %}{% endraw %}
- **[{% raw %}{{{% endraw %} e.title {% raw %}}}{% endraw %}]({{ e.url | relative_url }})** — {% raw %}{{ e.date | date: "%Y-%m-%d %H:%M %Z" }}{% endraw %}  
  {% raw %}{{ e.summary }}{% endraw %}
{% raw %}{% endfor %}{% endraw %}
{% raw %}{% else %}{% endraw %}
No events yet. Check back soon.
{% raw %}{% endif %}{% endraw %}
