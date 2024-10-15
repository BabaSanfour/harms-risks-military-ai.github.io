---
layout: page-floatbutton
title: Accepted Abstracts
subtitle: Short abstracts and authors
permalink: /accepted-abstracts
---

# Please find a list of the accepted abstracts.
## Short talks:
{% assign abstracts = site.data.accepted-orals | sample: site.data.accepted-orals.size %}
{% for abstract in abstracts %}
  {% assign side = forloop.index0 | modulo: 2 %}
    {% if side == 0 %}
      {% include abstract-card.html %}
    {% else %}
      {% include abstract-card.html %}
    {% endif %}
{% endfor %}
## Posters:
{% assign abstracts = site.data.accepted-abstracts | sample: site.data.accepted-abstracts.size %}
{% for abstract in abstracts %}
  {% assign side = forloop.index0 | modulo: 2 %}
    {% if side == 0 %}
      {% include abstract-card.html %}
    {% else %}
      {% include abstract-card.html %}
    {% endif %}
{% endfor %}

