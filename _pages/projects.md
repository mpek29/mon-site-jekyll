---
layout: page
title: Projets
permalink: /projects/
description: Voici une liste des projets que j'ai réalisés ou auxquels j'ai participé.
nav: true
nav_order: 2
display_categories: ["Electronics", "Computer Science", "Mechanical Engineering"]
---

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Affichage par catégorie -->
  {%- for category in page.display_categories %}
    <h2 class="category">{{ category }}</h2>
    {%- assign categorized_projects = site.projects | where: "category", category -%}
    
    <!-- Extraction des sous-catégories uniques -->
    {%- assign subcategories = categorized_projects | map: "subcategory" | uniq | sort %}
    
    {%- for subcategory in subcategories %}
      {%- assign filtered_projects = categorized_projects | where: "subcategory", subcategory | sort: "importance" %}
      
      {%- if subcategory != "General" %}
        <h3 class="subcategory">{{ subcategory }}</h3>
      {%- endif %}

      <div class="grid">
        {%- for project in filtered_projects -%}
          {% include projects.html %}
        {%- endfor %}
      </div>
    {%- endfor %}

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
