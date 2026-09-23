---
layout: page
permalink: /repositories/
title: Open Source Contributions
description: My contributions to open-source scientific computing and machine learning projects.
nav: true
nav_order: 4
---

<style>
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
    gap: 1.5rem;
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
    transition: border-color 0.15s ease, box-shadow 0.15s ease, transform 0.15s ease;
  }

  .oss-card:hover {
    border-color: rgba(127, 127, 127, 0.45);
    box-shadow: 0 4px 14px rgba(0, 0, 0, 0.06);
    transform: translateY(-2px);
  }

  .oss-card-header {
    display: flex;
    align-items: center;
    gap: 0.75rem;
    padding: 1.1rem 1.1rem 0.85rem;
  }

  .oss-logo-chip {
    flex-shrink: 0;
    width: 40px;
    height: 40px;
    border-radius: 7px;
    border: 1px solid rgba(127, 127, 127, 0.18);
    background: #ffffff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 7px;
    box-sizing: border-box;
  }

  .oss-logo-chip img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
    display: block;
  }

  .oss-card-heading {
    min-width: 0;
  }

  .oss-card-heading h3 {
    margin: 0;
    font-size: 0.95rem;
    font-weight: 700;
    line-height: 1.3;
  }

  .oss-card-heading .oss-tagline {
    font-size: 0.74rem;
    opacity: 0.6;
    margin-top: 0.1rem;
    line-height: 1.3;
  }

  .oss-card-body {
    padding: 0 1.1rem 1.1rem;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
  }

  .oss-contribution + .oss-contribution {
    margin-top: 0.7rem;
    padding-top: 0.7rem;
    border-top: 1px solid rgba(127, 127, 127, 0.14);
  }

  .oss-contribution-title {
    display: flex;
    align-items: baseline;
    gap: 0.4rem;
    margin: 0 0 0.25rem;
    font-size: 0.82rem;
    font-weight: 700;
  }

  .oss-contribution-pr {
    font-size: 0.68rem;
    font-weight: 600;
    opacity: 0.5;
  }

  .oss-card-impact {
    font-size: 0.78rem;
    margin: 0 0 0.5rem;
    line-height: 1.45;
    opacity: 0.82;
  }

  .oss-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.35rem;
    margin: 0.75rem 0 0.85rem;
  }

  .oss-tag {
    font-size: 0.66rem;
    padding: 0.18rem 0.5rem;
    border-radius: 4px;
    background: rgba(127, 127, 127, 0.1);
    opacity: 0.85;
  }

  .oss-card-link {
    display: inline-flex;
    align-items: center;
    gap: 0.3rem;
    font-size: 0.78rem;
    font-weight: 600;
    text-decoration: none;
    width: fit-content;
  }

  .oss-card-link svg {
    width: 11px;
    height: 11px;
    flex-shrink: 0;
    transition: transform 0.15s ease;
  }

  .oss-card-link:hover {
    text-decoration: underline;
  }

  .oss-card-link:hover svg {
    transform: translate(2px, -2px);
  }

  .oss-card > .oss-card-body > .oss-card-link {
    margin-top: auto;
  }
</style>

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

      <div class="oss-contribution">
        <h4 class="oss-contribution-title">
          QSW / RQSW
          <span class="oss-contribution-pr">PR #838</span>
        </h4>
        <p class="oss-card-impact">
          Faster, unbiased distance estimation between probability distributions in 3D, via low-discrepancy directions on the sphere.
        </p>
        <a class="oss-card-link" href="https://github.com/PythonOT/POT/pull/838" target="_blank" rel="noopener">
          View PR #838
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
            <path d="M7 17L17 7"></path>
            <path d="M8 7h9v9"></path>
          </svg>
        </a>
      </div>

      <div class="oss-contribution">
        <h4 class="oss-contribution-title">
          UnifOrtho
          <span class="oss-contribution-pr">PR #853</span>
        </h4>
        <p class="oss-card-impact">
          Extends the same accuracy gain to any dimension, using mutually orthogonal sampling directions.
        </p>
        <a class="oss-card-link" href="https://github.com/PythonOT/POT/pull/853" target="_blank" rel="noopener">
          View PR #853
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true">
            <path d="M7 17L17 7"></path>
            <path d="M8 7h9v9"></path>
          </svg>
        </a>
      </div>

      <div class="oss-tags">
        <span class="oss-tag">Python</span>
        <span class="oss-tag">Quasi-Monte Carlo</span>
        <span class="oss-tag">Optimal transport</span>
      </div>
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
        Three new ways to sample points that cover a space more evenly than random sampling: Latin Hypercube, Korobov lattices, and Hammersley sets.
      </p>
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
