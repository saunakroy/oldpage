---
layout: page
title: Projects
permalink: /projects/
description: A growing collection of my personal and team projects. 
nav: true
nav_order: 3
horizontal: false
---

<div class="projects">
  <div class="row row-cols-1 row-cols-md-3">
    {% assign sorted_projects = site.projects | sort: "importance" %}
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
