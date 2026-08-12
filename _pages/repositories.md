---
layout: page
permalink: /repositories/
title: Open Source Contributions
description: My contributions to open-source scientific computing and machine learning projects.
nav: true
nav_order: 4
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

### 1.QMCPy

**Added Latin Hypercube, Korobov Lattice, and Hammersley samplers**  
[Pull Request #582](https://github.com/QMCSoftware/QMCSoftware/pull/582) · **Merged**

Contributed three new sampling methods to **QMCPy**, an open-source Python library for quasi-Monte Carlo methods. 
The contribution included the implementation of the new samplers, integration with the existing sampler infrastructure, tests and documentation, as well as a demonstration notebook.

This is my first accepted and merged contribution to a major open-source scientific computing project.
