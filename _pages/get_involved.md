---
layout: page
title: Get Involved
permalink: /get-involved/
nav: true
nav_order: 8
description: We are always looking for motivated researchers to join the lab. Below you'll find information on open positions and how to get in touch.

# --- YOUR DATA SECTION ---
phd_positions:
  - title: "[Project Title]"
    deadline: "DD Month YYYY"
    funder: "EPSRC"
    description: "Description of the PhD project — research questions, methods, expected outcomes. Typically 2–3 sentences."
    requirements: "MSc or first-class BSc in a relevant field; experience in X, Y, Z."
    contact_email: "j.smith@qmul.ac.uk"

postdoc_positions: [] # Leave empty [] if none are currently available

contact_info:
  email: "j.smith@qmul.ac.uk"
  name: "Prof. Jane Smith"
  lab: "Digital Intelligence Systems Lab"
  school: "School of Electronic Engineering and Computer Science"
  university: "Queen Mary University of London"
  address: "Mile End Road, London E1 4NS"
  website_url: "https://disl.github.io"
  website_display: "disl.github.io"
---

<!-- Open Positions Section -->
## Open Positions

### PhD Studentships
{% if page.phd_positions and page.phd_positions.size > 0 %}
  {% for position in page.phd_positions %}
  <div class="card border-0 shadow-sm p-4 mb-4">
    <h5>PhD Position: {{ position.title }}</h5>
    <p class="text-muted small">📅 Application deadline: <strong>{{ position.deadline }}</strong> &nbsp;·&nbsp; 🏛 Funded by: {{ position.funder }}</p>
    <p>{{ position.description }}</p>
    <p><strong>Requirements:</strong> {{ position.requirements }}</p>
    <div>
      <a href="mailto:{{ position.contact_email }}?subject=PhD Enquiry: {{ position.title | url_encode }}" class="btn btn-sm btn-outline-primary">
        Apply / Enquire
      </a>
    </div>
  </div>
  {% endfor %}
{% else %}
  <p><em>No PhD positions are currently advertised. Check back soon or send an expression of interest.</em></p>
{% endif %}

---

### Postdoctoral Positions
{% if page.postdoc_positions and page.postdoc_positions.size > 0 %}
  {% for position in page.postdoc_positions %}
  <div class="card border-0 shadow-sm p-4 mb-4">
    <h5>Postdoc Position: {{ position.title }}</h5>
    <p class="text-muted small">📅 Application deadline: <strong>{{ position.deadline }}</strong></p>
    <p>{{ position.description }}</p>
    <div>
      <a href="mailto:{{ position.contact_email }}?subject=Postdoc Enquiry: {{ position.title | url_encode }}" class="btn btn-sm btn-outline-primary">
        Apply / Enquire
      </a>
    </div>
  </div>
  {% endfor %}
{% else %}
  <p><em>No postdoctoral positions are currently advertised. Check back soon or send an expression of interest.</em></p>
{% endif %}

---

### MSc / Final Year Projects

We regularly supervise MSc and final-year undergraduate projects aligned with our research themes. If you are a QMUL student interested in working with us, please email us with your CV and a short paragraph describing your interests.

---

### Visiting Researchers

We welcome visiting researchers and research interns. If you are interested in a research visit, please get in touch with the relevant lab member directly.

---

## How to Apply

Please send the following to [<span class="text-nowrap">{{ page.contact_info.email }}</span>](mailto:{{ page.contact_info.email }}):

1. A **CV** (including publications if applicable)
2. A **cover letter** describing your research interests and why you want to join DISL
3. For PhD applicants: a **research proposal** (1–2 pages)
4. Contact details for **two referees**

We aim to respond to all enquiries within two weeks.

---

## Contact

**{{ page.contact_info.name }}**  
{{ page.contact_info.lab }}  
{{ page.contact_info.school }}  
{{ page.contact_info.university }}  
{{ page.contact_info.address }}  

📧 [{{ page.contact_info.email }}](mailto:{{ page.contact_info.email }})  
🌐 [{{ page.contact_info.website_display }}]({{ page.contact_info.website_url }})