---
layout: single
title: Glossary of Immigration Terms
permalink: /glossary/
lang: en
alt_url: /glosario/
exclude_from_index: true
---

This glossary provides plain-language explanations of common terms used in U.S. immigration law and processes. Each entry links to a detailed page for further reading.

{% assign glossary_entries = site.glossary | sort: "title" %}
<ul>
  {% for entry in glossary_entries %}
    {% unless entry.exclude_from_index %}
      <li><a href="{{ entry.url | relative_url }}">{{ entry.title }}</a></li>
    {% endunless %}
  {% endfor %}
</ul>