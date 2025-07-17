---
title: Glosario de Términos Legales
layout: single
lang: es
alt_url: /glossary/
permalink: /glosario/
---

Este glosario proporciona definiciones claras y concisas de términos comunes utilizados en procesos legales y de inmigración en los Estados Unidos. Está diseñado para ayudarle a comprender mejor sus derechos, formularios y procedimientos legales.

---

{% assign sorted_glossary = site.glosario | sort: 'title' %}

<ul class="glossary-list">
  {% for entry in sorted_glossary %}
    {% unless entry.url == page.url %}
      <li><a href="{{ entry.url }}">{{ entry.title }}</a></li>
    {% endunless %}
  {% endfor %}
</ul>