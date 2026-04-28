---
title: Projects
subtitle: Protocols, research systems, speculative institutions, and applied frameworks.
kicker: Catalogue
permalink: /projects/
---

<div class="listing">
  {% assign sorted_projects = site.projects | sort: 'order' %}
  {% for project in sorted_projects %}
    {% include project-card.html project=project %}
  {% endfor %}
</div>
