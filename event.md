---
layout: default
title: Event
---

|Date|Title|Place|
|----|-----|-----|
{% for item in site.data.event -%}
  |{{ item.date }}|[{{ item.title }}]({{ site.url }}/events/{{ item.site }}.html)|{{ item.place }}|
{% endfor %}
