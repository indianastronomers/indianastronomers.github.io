---
layout: default
title: Events
---

# Events

This page lists all **past, ongoing, and upcoming events** organized under the Indian Astronomers Around the World initiative.

Events are listed in **reverse chronological order**.

---

{% assign sorted_events = site.pages | where_exp:"p","p.path contains 'events/'" | sort: "date" | reverse %}
{% for event in sorted_events %}
{% if event.event %}
### {{ event.title }}
**Date:** {{ event.date | date: "%d %B %Y" }}  
{{ event.summary }}  
[View details →]({{ event.url }})

---
{% endif %}
{% endfor %}