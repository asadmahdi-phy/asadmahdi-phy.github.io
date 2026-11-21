
---
layout: page
title: projects
permalink: /projects/
description: A collection of my research and academic projects.
nav: true
nav_order: 2
display_categories: [research, academic]
horizontal: false
---

<!-- pages/projects.md -->

<div class="projects">

  <!-- ============================= -->
  <!-- RESEARCH PROJECTS             -->
  <!-- ============================= -->

  <h2 class="category">Research Projects</h2>

  {%- assign research_projects = site.projects | where: "category", "research" | sort: "importance" -%}

  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">
        {%- for project in research_projects -%}
          {% include projects_horizontal.html %}
        {%- endfor -%}
      </div>
    </div>
  {% else %}
    <div class="grid">
      {%- for project in research_projects -%}
        {% include projects.html %}
      {%- endfor -%}
    </div>
  {% endif %}


  <!-- ============================= -->
  <!-- ACADEMIC PROJECTS             -->
  <!-- ============================= -->

  <h2 class="category">Academic Projects</h2>

  {%- assign academic_projects = site.projects | where: "category", "academic" | sort: "importance" -%}

  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">
        {%- for project in academic_projects -%}
          {% include projects_horizontal.html %}
        {%- endfor -%}
      </div>
    </div>
  {% else %}
    <div class="grid">
      {%- for project in academic_projects -%}
        {% include projects.html %}
      {%- endfor -%}
    </div>
  {% endif %}

</div>
