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

<div class="row">

  <!-- Carte pour POT -->
  <div class="col-md-6">
    <div class="card mb-4">
      <img src="{{ '/assets/img/logo_pot.svg' | relative_url }}" class="card-img-top" alt="POT Logo" style="padding: 20px; max-height: 150px; object-fit: contain; background-color: #f8f9fa;">
      <div class="card-body">
        <h5 class="card-title">POT: Python Optimal Transport</h5>
        <p class="card-text">
          <strong>Contribution:</strong> Merged pull request #838.
          <br><br>
          <a href="https://github.com/PythonOT/POT/pull/838" target="_blank" class="btn btn-primary btn-sm">
            View Pull Request #838
          </a>
        </p>
      </div>
    </div>
  </div>

  <!-- Carte pour QMCPy -->
  <div class="col-md-6">
    <div class="card mb-4">
      <img src="{{ '/assets/img/qmcpy.logo.png' | relative_url }}" class="card-img-top" alt="QMCPy Logo" style="padding: 20px; max-height: 150px; object-fit: contain; background-color: #f8f9fa;">
      <div class="card-body">
        <h5 class="card-title">QMCPy: Quasi-Monte Carlo Python</h5>
        <p class="card-text">
          <strong>Contribution:</strong> Merged pull request #582.
          <br><br>
          <a href="https://github.com/QMCSoftware/qmcpy/pull/582" target="_blank" class="btn btn-primary btn-sm">
            View Pull Request #582
          </a>
        </p>
      </div>
    </div>
  </div>

</div>

For more, visit my [GitHub profile](https://github.com/Samuel-Vangu).
