---
title: Journal
subtitle: Essays, studies, field notes, and public research from Anthem.
kicker: Public writing
permalink: /journal/
---

<div class="listing">
  {% for post in site.posts %}
    {% include post-card.html post=post %}
  {% endfor %}
</div>
