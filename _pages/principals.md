---
layout: single
title: "Principals"
permalink: /principals/
author_profile: false
share: true
---

{% for collection in site.collections %}

  {% for post in collection.docs %}
    {% if collection.label == "principals" %}
      {% include archive-single.html %}
    {% endif %}
  {% endfor %}
{% endfor %}
