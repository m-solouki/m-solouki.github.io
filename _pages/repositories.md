---
layout: page
permalink: /repositories/
title: repositories
description: My GitHub repositories and projects.
nav: false
nav_order: 4
---

<div class="repositories">
  {% if site.github_users %}
  {% for user in site.github_users %}
  {% include repository/user.html username=user %}
  {% endfor %}
  {% endif %}

  {% if site.github_repos %}
  {% for repo in site.github_repos %}
  {% include repository/repo.html repository=repo %}
  {% endfor %}
  {% endif %}
</div>