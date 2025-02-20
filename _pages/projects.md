---
layout: page
title: Projets
permalink: /projects/
description: Voici une liste des projets que j'ai réalisés ou auxquels j'ai participé.
nav: true
nav_order: 2
display_categories: ["Electronics", "Computer Science", "Mechanical Engineering"]

subcategory_order:
  Computer Science:
    - Firmware Development
    - Cybersecurity
    - Software Development
    - Data Engineering
    - DevOps and Automation
    - Artificial Intelligence
    - Documentation
  Electronics:
    - PCB Design
    - PCB Reverse Engineering
    - Digital Electronics
    - Power Electronics
    - Signal and Image Processing
    - PCB Repair
  Mechanical Engineering:
    - Mechanical Design
    - Analysis and Simulation
    - Fluid Mechanics
    - Materials and Mechanics of Materials
    - Control Systems
---

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Parcours des catégories -->
  {%- for category in page.display_categories %}
    {%- assign categorized_projects = site.projects | where: "category", category -%}

    {%- if categorized_projects.size > 0 %}
      <h2 class="category">{{ category }}</h2>
      
      <!-- Récupération de l'ordre des sous-catégories définies -->
      {%- assign ordered_subcategories = page.subcategory_order[category] -%}

      {%- for subcategory in ordered_subcategories %}
        {%- assign filtered_projects = categorized_projects | where: "subcategory", subcategory | sort: "importance" %}
        
        {%- if filtered_projects.size > 0 %}
          <h3 class="subcategory">{{ subcategory }}</h3>

          <div class="grid">
            {%- for project in filtered_projects -%}
              {% include projects.html %}
            {%- endfor %}
          </div>
        {%- endif %}
      {%- endfor %}
      
    {%- endif %}
  {% endfor %}

{%- else -%}
  <!-- Affichage sans catégories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
{%- endif -%}
</div>
