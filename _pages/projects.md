---
layout: page
title: Projects
permalink: /projects/
description: A growing collection of my personal and team projects. Click on the tabs below to view the projects. The brain tumor classification, TSP algorithms, and wage analysis projects link to Python notebooks on my GitHub, where you can easily follow along with the code.
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
