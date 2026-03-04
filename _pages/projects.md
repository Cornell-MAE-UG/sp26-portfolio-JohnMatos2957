---
layout: default
title: John Matos - Portfolio
permalink: https://cornell-mae-ug.github.io/portfolio-sp26-sp26-portfolio-portolios-1/sp26-portfolio-JohnMatos2957/projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
          <p>{{ project.title}}</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>