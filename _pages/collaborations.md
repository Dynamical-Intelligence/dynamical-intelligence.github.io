---
layout: page
title: Collaborations
permalink: /collaborations/
nav: true
nav_order: 5


# --- YOUR DATA SECTION ---
# You can easily add, remove, or reorder partners right here:
academic_partners:
  - name: "Ian McFadden"
    url: "https:/mcfaddenecology.com"
    subtext: "School of Biological and Behavioural Sciences, Queen Mary University of London"
    description: "Brief description of the collaboration"

  - name: "Anna Xambó Sedo"
    url: "https://annaxambo.me/"
    subtext: "Centre for Digital Music, Queen Mary University of London"
    description: "Brief description of the collaboration."

industry_partners:
  - name: "Meta"
    url: "https://www.meta.com/"
    description: "Brief description of the collaboration."

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


## Interested in collaborating?

We are always open to new collaborations with researchers and industry partners working on related topics. Please [get in touch](/get-involved/).
