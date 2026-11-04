---
layout: page
title: research
permalink: /research/
description: Selected research projects and ongoing work.
nav: false
nav_order: 3
display_categories: [research]
horizontal: true
---

<div class="projects">
{% assign research_projects = site.projects | where: "category", "research" | sort: "importance" %}
<div class="row row-cols-1">
  {% for project in research_projects %}
    {% include projects_horizontal.liquid %}
  {% endfor %}
</div>
</div>
