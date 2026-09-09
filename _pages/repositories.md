---
layout: page
permalink: /repositories/
title: Open Source Contributions
description: My contributions to open-source scientific computing and machine learning projects.
nav: true
nav_order: 4
---

<style>
  .oss-hero {
    position: relative;
    padding: 2.5rem 1.5rem 2.25rem;
    margin-bottom: 2.75rem;
    border-radius: 6px;
    overflow: hidden;
    background: var(--global-card-bg-color, rgba(127, 127, 127, 0.04));
  }

  .oss-hero-points {
    position: absolute;
    inset: 0;
    z-index: 0;
    opacity: 0.5;
    pointer-events: none;
  }

  .oss-hero-points circle {
    fill: currentColor;
    opacity: 0.35;
  }

  .oss-hero-content {
    position: relative;
    z-index: 1;
    max-width: 620px;
  }

  .oss-hero-content p {
    margin: 0;
    line-height: 1.65;
    font-size: 1.02rem;
  }

  .oss-hero-content p + p {
    margin-top: 0.6rem;
    opacity: 0.75;
    font-size: 0.92rem;
  }

  .oss-section-title {
    font-size: 1.05rem;
    font-weight: 600;
    letter-spacing: 0.01em;
    margin: 0 0 1.25rem;
    padding-bottom: 0.5rem;
    border-bottom: 1px solid rgba(127, 127, 127, 0.22);
  }

  .oss-projects {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.75rem;
    max-width: 900px;
    margin-bottom: 2.5rem;
  }

  @media (max-width: 700px) {
    .oss-projects {
      grid-template-columns: 1fr;
    }
  }

  .oss-card {
    display: flex;
    flex-direction: column;
    border: 1px solid rgba(127, 127, 127, 0.22);
    border-radius: 8px;
    overflow: hidden;
    background: var(--global-bg-color, transparent);
    transition: border-color 0.15s ease;
  }

  .oss-card:hover {
    border-color: rgba(127, 127, 127, 0.45);
  }

  .oss-card-header {
    display: flex;
    align-items: flex-start;
    gap: 0.9rem;
    padding: 1.35rem 1.35rem 1rem;
  }

  .oss-logo-chip {
    flex-shrink: 0;
    width: 46px;
    height: 46px;
    border-radius: 8px;
    border: 1px solid rgba(127, 127, 127, 0.2);
    background: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 8px;
    box-sizing: border-box;
  }

  .oss-logo-chip img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
  }

  .oss-card-heading {
    min-width: 0;
    padding-top: 2px;
  }

  .oss-card-heading h3 {
    margin: 0;
    font-size: 1.02rem;
    font-weight: 600;
    line-height: 1.3;
  }

  .oss-card-heading .oss-tagline {
    font-size: 0.82rem;
    opacity: 0.65;
    margin-top: 0.15rem;
    line-height: 1.4;
  }

  .oss-card-body {
    padding: 0 1.35rem 1.35rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .oss-card-summary {
    font-size: 0.88rem;
    margin: 0 0 0.85rem;
    line-height: 1.55;
  }

  .oss-card-details {
    list-style: none;
    margin: 0 0 1.1rem;
    padding: 0;
    font-size: 0.83rem;
    line-height: 1.55;
    opacity: 0.85;
  }

  .oss-card-details li {
    padding-left: 0.95rem;
    position: relative;
  }

  .oss-card-details li + li {
    margin-top: 0.3rem;
  }

  .oss-card-details li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0.6em;
    width: 4px;
    height: 4px;
    border-radius: 50%;
    background: currentColor;
    opacity: 0.5;
  }

  .oss-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin: 0 0 1.15rem;
  }

  .oss-tag {
    font-size: 0.72rem;
    padding: 0.2rem 0.55rem;
    border-radius: 4px;
    background: rgba(127, 127, 127, 0.1);
    opacity: 0.85;
  }

  .oss-card-link {
    margin-top: auto;
    font-size: 0.83rem;
    font-weight: 600;
    text-decoration: none;
  }

  .oss-card-link:hover {
    text-decoration: underline;
  }
</style>

<div class="oss-hero">
  <svg class="oss-hero-points" viewBox="0 0 600 120" preserveAspectRatio="none" aria-hidden="true">
    <!-- Low-discrepancy point set, purely decorative -->
    <circle cx="18" cy="94" r="2.4"/><circle cx="311" cy="12" r="2.4"/><circle cx="162" cy="53" r="2.4"/>
    <circle cx="461" cy="76" r="2.4"/><circle cx="87" cy="27" r="2.4"/><circle cx="386" cy="105" r="2.4"/>
    <circle cx="237" cy="88" r="2.4"/><circle cx="536" cy="41" r="2.4"/><circle cx="49" cy="63" r="2.4"/>
    <circle cx="349" cy="34" r="2.4"/><circle cx="199" cy="8" r="2.4"/><circle cx="498" cy="98" r="2.4"/>
    <circle cx="124" cy="112" r="2.4"/><circle cx="424" cy="59" r="2.4"/><circle cx="274" cy="21" r="2.4"/>
    <circle cx="574" cy="70" r="2.4"/><circle cx="6" cy="45" r="2.4"/><circle cx="150" cy="100" r="2.4"/>
    <circle cx="450" cy="16" r="2.4"/><circle cx="300" cy="65" r="2.4"/>
  </svg>
  <div class="oss-hero-content">
    <p>
      I contribute quasi-Monte Carlo and low-discrepancy sampling methods
      to open-source scientific Python libraries &mdash; the code that
      decides how evenly a computer explores a space it can never fully
      cover.
    </p>
    <p>Contributions below are reviewed and merged into their upstream codebases.</p>
  </div>
</div>

<h2 class="oss-section-title">GitHub</h2>

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center" style="margin-bottom: 2.5rem;">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>
{% endif %}

<h2 class="oss-section-title">Contributions</h2>

<div class="oss-projects">

  <!-- POT -->
  <div class="oss-card">
    <div class="oss-card-header">
      <div class="oss-logo-chip">
        <img src="/assets/img/logo_pot.svg" alt="POT logo">
      </div>
      <div class="oss-card-heading">
        <h3>POT</h3>
        <div class="oss-tagline">Python Optimal Transport</div>
      </div>
    </div>
    <div class="oss-card-body">
      <p class="oss-card-summary">
        Added quasi-Monte Carlo sampling for the Sliced Wasserstein distance.
      </p>
      <ul class="oss-card-details">
        <li>Low-discrepancy directions on the sphere via generalized spiral points (Rakhmanov&ndash;Saff&ndash;Zhou), deterministic and randomly rotated</li>
        <li>Unbiased estimator for use in stochastic optimization</li>
        <li>Verified across all four backends: NumPy, PyTorch, JAX, TensorFlow</li>
      </ul>
      <div class="oss-tags">
        <span class="oss-tag">Python</span>
        <span class="oss-tag">Quasi-Monte Carlo</span>
        <span class="oss-tag">Optimal transport</span>
        <span class="oss-tag">Multi-backend numerics</span>
      </div>
      <a class="oss-card-link" href="https://github.com/PythonOT/POT/pull/838" target="_blank" rel="noopener">
        View PR #838 &nearr;
      </a>
    </div>
  </div>

  <!-- QMCPy -->
  <div class="oss-card">
    <div class="oss-card-header">
      <div class="oss-logo-chip">
        <img src="/assets/img/qmcpy.logo.png" alt="QMCPy logo">
      </div>
      <div class="oss-card-heading">
        <h3>QMCPy</h3>
        <div class="oss-tagline">Quasi-Monte Carlo in Python</div>
      </div>
    </div>
    <div class="oss-card-body">
      <p class="oss-card-summary">
        Added three low-discrepancy point set generators.
      </p>
      <ul class="oss-card-details">
        <li>Latin Hypercube sampling</li>
        <li>Korobov lattice sequences</li>
        <li>Hammersley point sets</li>
      </ul>
      <div class="oss-tags">
        <span class="oss-tag">Python</span>
        <span class="oss-tag">Quasi-Monte Carlo</span>
        <span class="oss-tag">Numerical methods</span>
      </div>
      <a class="oss-card-link" href="https://github.com/QMCSoftware/QMCSoftware/pull/582" target="_blank" rel="noopener">
        View PR #582 &nearr;
      </a>
    </div>
  </div>

</div>
