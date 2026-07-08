---
layout: page
title: Collaborations
permalink: /collaborations/
nav: true
nav_order: 5
description: We work with a range of academic institutions, industry partners, and research networks. We believe that great research happens through open collaboration.

# --- YOUR DATA SECTION ---
# You can easily add, remove, or reorder partners right here:
academic_partners:
  - name: "Example University"
    url: "https://example-university.ac.uk"
    subtext: "Department of Computer Science"
    description: "Brief description of the collaboration — joint projects, shared PhD students, etc."
    contact: "Prof. Example Name"
  - name: "Another Institution"
    url: "https://another-institution.edu"
    subtext: "Music Technology Group"
    description: "Brief description of the collaboration."
    contact: "Dr. Another Name"

industry_partners:
  - name: "Example Company"
    url: "https://example-company.com"
    description: "Brief description of the industry collaboration — internships, sponsored research, joint projects."

research_networks:
  - name: "Network Name"
    url: "https://example.com"
    description: "Brief description of the network and our role in it."
  - name: "Another Network"
    url: "https://example.com"
    description: "Brief description."
---

{% if page.academic_partners %}
## Academic Partners
<div class="row row-cols-1 row-cols-md-2 g-4 mb-5">
  {% for partner in page.academic_partners %}
  <div class="col">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h5><a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></h5>
      {% if partner.subtext %}
        <p class="text-muted small mb-2">{{ partner.subtext }}</p>
      {% endif %}
      <p>{{ partner.description }}</p>
      {% if partner.contact %}
        <p class="mb-0"><strong>Contact:</strong> {{ partner.contact }}</p>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>
<hr>
{% endif %}

{% if page.industry_partners %}
## Industry Partners
<div class="row row-cols-1 row-cols-md-2 g-4 mb-5">
  {% for partner in page.industry_partners %}
  <div class="col">
    <div class="card h-100 border-0 shadow-sm p-3">
      <h5><a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></h5>
      <p>{{ partner.description }}</p>
    </div>
  </div>
  {% endfor %}
</div>
<hr>
{% endif %}

{% if page.research_networks %}
## Research Networks
<ul class="mb-5">
  {% for network in page.research_networks %}
  <li>
    <strong><a href="{{ network.url }}" target="_blank">{{ network.name }}</a></strong> — {{ network.description }}
  </li>
  {% endfor %}
</ul>
<hr>
{% endif %}

## Interested in collaborating?

We are always open to new collaborations with researchers and industry partners working on related topics. Please [get in touch](/get-involved/).