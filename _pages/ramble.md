---
title: The Ramble
layout: default
permalink: /ramble/
---

# The Ramble

<ul>
{% assign entries = site.ramble | sort: "date" | reverse %}
{% for item in entries %}
  <li>
    <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    <small>— {{ item.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>