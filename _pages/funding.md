---
layout: page
title: Funding
permalink: /funding/
nav: true
nav_order: 6
description: Our research is generously supported by the following funding bodies and organisations. We are grateful for their continued investment in our work.

# --- YOUR DATA SECTION ---
current_grants:
  - title: "Project Title Here"
    description: "Brief one-line description"
    funder: "EPSRC"
    funder_url: "https://www.ukri.org/councils/epsrc/"
    grant_no: "EP/XXXXXXX/1"
    period: "2023–2026"
    pi: "Prof. Jane Smith"
  - title: "Another Project Title"
    description: "Brief one-line description"
    funder: "European Research Council"
    funder_url: "https://erc.europa.eu"
    grant_no: "ERC-XXXXXXX"
    period: "2022–2027"
    pi: "Prof. Jane Smith"

past_grants:
  - title: "Past Project Title"
    funder: "EPSRC"
    period: "2019–2022"

funders:
  - name: "EPSRC"
    url: "https://www.ukri.org/councils/epsrc/"
    logo: "epsrc.png"
  - name: "ERC"
    url: "https://erc.europa.eu"
    logo: "erc.png"
---

<!-- Current Grants Section -->
{% if page.current_grants %}
## Current Grants

<div class="table-responsive">
<table class="table table-hover">
  <thead>
    <tr>
      <th>Project</th>
      <th>Funder</th>
      <th>Grant No.</th>
      <th>Period</th>
      <th>PI</th>
    </tr>
  </thead>
  <tbody>
    {% for grant in page.current_grants %}
    <tr>
      <td>
        <strong>{{ grant.title }}</strong>
        {% if grant.description %}<br><span class="text-muted small">{{ grant.description }}</span>{% endif %}
      </td>
      <td>
        {% if grant.funder_url %}<a href="{{ grant.funder_url }}" target="_blank">{% endif %}
          {{ grant.funder }}
        {% if grant.funder_url %}</a>{% endif %}
      </td>
      <td>{{ grant.grant_no }}</td>
      <td>{{ grant.period }}</td>
      <td>{{ grant.pi }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
</div>
<hr>
{% endif %}

<!-- Past Grants Section -->
{% if page.past_grants %}
## Past Grants

<div class="table-responsive">
<table class="table table-hover">
  <thead>
    <tr>
      <th>Project</th>
      <th>Funder</th>
      <th>Period</th>
    </tr>
  </thead>
  <tbody>
    {% for grant in page.past_grants %}
    <tr>
      <td><strong>{{ grant.title }}</strong></td>
      <td>{{ grant.funder }}</td>
      <td>{{ grant.period }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
</div>
<hr>
{% endif %}

<!-- Funder Logos Section -->
{% if page.funders %}
## Funders

<div class="row row-cols-2 row-cols-md-4 g-4 align-items-center text-center mt-2">
  {% for funder in page.funders %}
  <div class="col">
    <a href="{{ funder.url }}" target="_blank">
      <img src="{{ '/assets/img/funders/' | append: funder.logo | relative_url }}"
           alt="{{ funder.name }}" class="img-fluid" style="max-height: 60px;">
    </a>
  </div>
  {% endfor %}
</div>
{% endif %}