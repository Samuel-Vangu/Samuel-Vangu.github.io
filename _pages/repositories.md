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
    padding: 3rem 1.75rem 2.5rem;
    margin-bottom: 3rem;
    border-radius: 8px;
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
    font-size: 1.05rem;
  }

  .oss-hero-content p + p {
    margin-top: 0.65rem;
    opacity: 0.72;
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
    max-width: 940px;
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
    border-radius: 10px;
    overflow: hidden;
    background: var(--global-bg-color, transparent);
    transition: border-color 0.15s ease, box-shadow 0.15s ease, transform 0.15s ease;
  }

  .oss-card:hover {
    border-color: rgba(127, 127, 127, 0.45);
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.06);
    transform: translateY(-2px);
  }

  .oss-card-header {
    display: flex;
    align-items: flex-start;
    gap: 1rem;
    padding: 1.5rem 1.5rem 1.1rem;
  }

  .oss-logo-chip {
    flex-shrink: 0;
    width: 50px;
    height: 50px;
    border-radius: 9px;
    border: 1px solid rgba(127, 127, 127, 0.18);
    background: #ffffff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 9px;
    box-sizing: border-box;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05);
  }

  .oss-logo-chip img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
    display: block;
  }

  .oss-card-heading {
    min-width: 0;
    padding-top: 3px;
  }

  .oss-card-heading h3 {
    margin: 0;
    font-size: 1.08rem;
    font-weight: 700;
    line-height: 1.3;
  }

  .oss-card-heading .oss-tagline {
    font-size: 0.82rem;
    opacity: 0.62;
    margin-top: 0.2rem;
    line-height: 1.4;
  }

  .oss-card-body {
    padding: 0 1.5rem 1.5rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .oss-card-impact {
    font-size: 0.87rem;
    margin: 0 0 0.95rem;
    line-height: 1.55;
    font-style: italic;
    opacity: 0.8;
  }

  .oss-card-details {
    list-style: none;
    margin: 0 0 1.15rem;
    padding: 0;
    font-size: 0.85rem;
    line-height: 1.6;
    opacity: 0.88;
  }

  .oss-card-details li {
    padding-left: 1rem;
    position: relative;
  }

  .oss-card-details li + li {
    margin-top: 0.35rem;
  }

  .oss-card-details li::before {
    content: "";
    position: absolute;
    left: 0;
    top: 0.62em;
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
    margin: 0 0 1.25rem;
  }

  .oss-tag {
    font-size: 0.72rem;
    padding: 0.22rem 0.6rem;
    border-radius: 4px;
    background: rgba(127, 127, 127, 0.1);
    opacity: 0.85;
  }

  .oss-card-link {
    margin-top: auto;
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    font-size: 0.85rem;
    font-weight: 600;
    text-decoration: none;
    width: fit-content;
  }

  .oss-card-link svg {
    width: 13px;
    height: 13px;
    flex-shrink: 0;
    transition: transform 0.15s ease;
  }

  .oss-card-link:hover {
    text-decoration: underline;
  }

  .oss-card-link:hover svg {
    transform: translate(2px, -2px);
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
      to open-source scientific Python libraries, the code that decides
      how evenly a computer explores a space it can never fully cover.
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
      <p class="oss-card-impact">
        Makes distance estimation between probability distributions more accurate at the same computational cost.
      </p>
      <ul class="oss-card-details">
        <li>Low-discrepancy directions on the sphere via generalized spiral points (Rakhmanov–Saff–Zhou), deterministic and randomly rotated</li>
        <li>Unbiased estimator, suitable for stochastic optimization</li>
        <li>Verified across all four backends: NumPy, PyTorch, JAX, TensorFlow</li>
      </ul>
      <div class="oss-tags">
        <span class="oss-tag">Python</span>
        <span class="oss-tag">Quasi-Monte Carlo</span>
        <span class="oss-tag">Optimal transport</span>
        <span class="oss-tag">Multi-backend numerics</span>
      </div>
      <a class="oss-card-link" href="https://github.com/PythonOT/POT/pull/838" target="_blank" rel="noopener">
        View PR #838
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M7 17L17 7"></path>
          <path d="M8 7h9v9"></path>
        </svg>
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
      <p class="oss-card-impact">
        Adds three ways to sample points that cover a space more evenly than random sampling.
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
        View PR #582
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
          <path d="M7 17L17 7"></path>
          <path d="M8 7h9v9"></path>
        </svg>
      </a>
    </div>
  </div>

</div>
