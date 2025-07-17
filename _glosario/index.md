---
layout: single
title: Glosario de Términos Migratorios
permalink: /glosario/
lang: es
alt_url: /glossary/
---

Este glosario ofrece definiciones sencillas de términos comunes en el derecho migratorio de los EE. UU. Cada entrada enlaza a una página con más información.

{% assign glossary_entries = site.glosario | sort: "title" %}
<ul>
  {% for entry in glossary_entries %}
    <li><a href="{{ entry.url | relative_url }}">{{ entry.title }}</a></li>
  {% endfor %}
</ul>