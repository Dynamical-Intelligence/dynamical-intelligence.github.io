---
layout: page
title: Funding
permalink: /funding/
nav: true
nav_order: 6
description:

# --- YOUR DATA SECTION ---
current_grants:
  - title: "GenAI Hub Dataset Challenge & Creations Projects"
    funder: "UKRI EPSRC"
    funder_url: "https://www.ukri.org/councils/epsrc/"
    period: "2026–2027"
    image: "ukri_epsrc.png"
  - title: "ICURe Explore"
    funder: "Innovate UK"
    funder_url: "https://www.gov.uk/government/organisations/innovate-uk"
    period: "2026"
    image: "icure_explore.png"
  - title: "Distinguished Faculty Award"
    funder: "Meta"
    funder_url: "https://research.facebook.com/"
    period: "2026"
    image: "meta.png"

past_grants:
  - title: "Underpinning the Pipeline for AI Skills"
    funder: "UKRI EPSRC"
    funder_url: "https://www.ukri.org/councils/epsrc/"
    period: "2025"
    image: "ukri_epsrc.png"
  - title: "Distinguished Faculty Award"
    funder: "Meta"
    funder_url: "https://research.facebook.com/"
    period: "2025"
    image: "meta.png"
  - title: "Signal Processing Mentorship Academy (SigMA)"
    funder: "IEEE SPS"
    funder_url: "https://signalprocessingsociety.org/professional-development/signal-processing-mentorship-academy-sigma-program"
    period: "2023–2024"
    image: "ieee_sps.png"
---

The lab's research is supported through competitively awarded grants and awards from government, industry, and professional societies. Our work has received funding from organisations including UK Research and Innovation (UKRI), the Engineering and Physical Sciences Research Council (EPSRC), Innovate UK, Meta, and the IEEE Signal Processing Society. These awards support research and the development of the next generation of AI researchers.

<!-- Current Grants Section -->

{% if page.current_grants %}

## Current Grants

<div class="d-flex flex-column gap-3 mb-4">
  {% for grant in page.current_grants %}
  <div class="card border-0 shadow-sm">
    <div class="row g-0 align-items-center">
      <div class="col-3 col-md-2 text-center p-3">
        {% if grant.image %}
          <img
            src="{{ '/assets/img/funders/' | append: grant.image | relative_url }}"
            alt="{{ grant.funder }}"
            class="img-fluid mx-auto d-block"
            style="max-height: 80px;"
          />
        {% endif %}
      </div>
      <div class="col-9 col-md-10 p-4">
        <h5>{{ grant.title }}</h5>
        {% if grant.description %}<p class="text-muted small">{{ grant.description }}</p>{% endif %}
        <p class="text-muted small mb-0">
          {% if grant.funder_url %}<a href="{{ grant.funder_url }}" target="_blank">{% endif %}
            {{ grant.funder }}
          {% if grant.funder_url %}</a>{% endif %}
          &nbsp;·&nbsp; {{ grant.period }}
        </p>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}

<!-- Past Grants Section -->

{% if page.past_grants %}

## Past Grants

<div class="d-flex flex-column gap-3 mb-4">
  {% for grant in page.past_grants %}
  <div class="card border-0 shadow-sm">
    <div class="row g-0 align-items-center">
      <div class="col-3 col-md-2 text-center p-3">
        {% if grant.image %}
          <img
            src="{{ '/assets/img/funders/' | append: grant.image | relative_url }}"
            alt="{{ grant.funder }}"
            class="img-fluid mx-auto d-block"
            style="max-height: 80px;"
          />
        {% endif %}
      </div>
      <div class="col-9 col-md-10 p-4">
        <h5>{{ grant.title }}</h5>
        <p class="text-muted small mb-0">
          {% if grant.funder_url %}<a href="{{ grant.funder_url }}" target="_blank">{% endif %}
            {{ grant.funder }}
          {% if grant.funder_url %}</a>{% endif %}
          &nbsp;·&nbsp; {{ grant.period }}
        </p>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}

<!-- Funder Logos Section -->

{% if page.funders %}

## Funders

<div class="row row-cols-2 row-cols-md-4 g-4 align-items-center text-center mt-2">
  {% for funder in page.funders %}
  <div class="col">
    <a href="{{ funder.url }}" target="_blank">
      <img src="{{ '/assets/img/funders/' | append: funder.logo | relative_url }}"
           alt="{{ funder.name }}" class="img-fluid mx-auto d-block" style="max-height: 60px;">
    </a>
  </div>
  {% endfor %}
</div>
{% endif %}
