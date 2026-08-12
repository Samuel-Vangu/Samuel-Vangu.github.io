---
layout: page
permalink: /repositories/
title: Open Source Contributions
description: My contributions to open-source scientific computing and machine learning projects.
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

### 🚀 QMCPy

**Added Latin Hypercube, Korobov Lattice, and Hammersley samplers**  
[Pull Request #582](https://github.com/QMCSoftware/QMCSoftware/pull/582) · **Merged**

Contributed three new sampling methods to **QMCPy**, an open-source Python library for quasi-Monte Carlo methods. This involved extending the library's sampler infrastructure, integrating new methods consistently with the existing API, and providing practical examples through an interactive notebook as long as tests and documentation.

This is my first accepted and merged contribution to a major open-source scientific computing project.

---

For more, visit my [GitHub profile](https://github.com/Samuel-Vangu).
