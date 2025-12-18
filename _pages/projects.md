---
title: Projects
layout: archive
permalink: /projects/
---

{% comment %}
  Assign all posts with category "projects" to a variable
{% endcomment %}
{% assign projects = site.categories.projects | sort: "date" | reverse %}

{% if projects.size > 0 %}
  {% for post in projects %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p>No projects have been published yet.</p>
{% endif %}
