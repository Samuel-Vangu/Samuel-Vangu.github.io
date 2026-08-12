---
layout: page
permalink: /repositories/
title: Open Source Contributions
description: Some of my contributions to open-source scientific computing and machine learning projects.
nav: true
nav_order: 4
---

I contribute to open-source projects in scientific computing and machine learning.

---

## GitHub Profile

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>
{% endif %}

---

## Notable Contributions

<div class="row row-cols-1 row-cols-md-3">
  {% assign contributions = site.contributions | where: "category", "open-source" | sort: "importance" %}
  {% for contribution in contributions %}
    <div class="col">
      <div class="card h-100">
        {% if contribution.img %}
          <img src="{{ contribution.img | relative_url }}" class="card-img-top" alt="{{ contribution.title }}" style="height: 120px; object-fit: contain; padding: 10px;">
        {% endif %}
        <div class="card-body">
          <h5 class="card-title">{{ contribution.title }}</h5>
          <p class="card-text">{{ contribution.description }}</p>
          <div class="card-text">
            {{ contribution.content | markdownify }}
          </div>
          <a href="{{ contribution.url | default: '#' }}" class="btn btn-primary btn-sm" target="_blank">
            View Contribution
          </a>
        </div>
        <div class="card-footer text-muted">
          🚀 Merged
        </div>
      </div>
    </div>
  {% endfor %}
</div>

---

For more, visit my [GitHub profile](https://github.com/Samuel-Vangu).
