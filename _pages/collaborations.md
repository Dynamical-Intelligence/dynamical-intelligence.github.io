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
    description: "Working with Dr. McFadden we bring together artificial intelligence and computational ecology to develop new methods for understanding ecological interactions at scale. We jointly supervise doctoral researchers working on multimodal AI, computer vision, machine learning, and network science to analyze biodiversity from visual and acoustic data. Our work aims to move beyond species identification by modeling ecological relationships and interaction networks that support biodiversity across diverse ecosystems. The collaboration combines expertise in AI and ecology to develop scalable computational tools with applications in environmental monitoring, conservation, and biodiversity science."
    lab_members: "Iran R. Roman, Dr. Ian McFadden, Nicole Filippelli, Philipp Gemmingen"

  - name: "Anna Xambó Sedo"
    url: "https://annaxambo.me/"
    subtext: "Centre for Digital Music, Queen Mary University of London"
    description: "Working with Dr. Xambó we explore the intersection of multimodal artificial intelligence, human computer interaction, and creative technologies. We jointly supervise doctoral research that investigates intelligent systems for music, sound, and multimodal interaction, combining machine learning with human centered design approaches. The collaboration emphasizes interdisciplinary research that connects AI with creative practice, interactive media, and real world applications while providing opportunities for students to develop novel methodologies that bridge technical innovation and user experience."
    lab_members: "Iran R. Roman, Dr. Anna Xambó, Anzi Wang"

industry_partners:
  - name: "Meta Platforms Inc"
    url: "https://www.meta.com/"
    description: "Our collaboration with Meta Platforms Inc. focuses on advancing multimodal AI systems that combine audio, vision, and spatial perception for real world understanding. Together we develop foundational technologies for acoustic imaging, sound source localization, self supervised learning, and egocentric sensing using the Aria platform. This collaboration has resulted in open source software, multimodal datasets, and research on computational auditory perception, while supporting the deployment of real time acoustic imaging algorithms on wearable devices. The partnership also contributes to broader community resources and benchmarks that accelerate research in multimodal machine perception and embodied AI."
    lab_members: "Iran R. Roman, Dr. Huw Cheston, Philipp Schmidt, Sohyun Im"

research_networks:
  - name: "The AI Hub in Generative Models"
    url: "https://www.genai.ac.uk/"
    description: "Through the AI Hub in Generative Models, the lab collaborates with researchers and industry partners to advance foundation models for multimodal audio AI. Our funded project develops an open, high fidelity multimodal dataset that captures how sound propagates in real three dimensional environments. The dataset supports research in generative audio synthesis, sound source separation, auditory scene understanding, and embodied AI while enabling reproducible benchmarking and open science. This collaboration strengthens connections between academia and industry and accelerates the development of next generation multimodal generative AI technologies."
    lab_members: "Iran R. Roman"
    external_collaborators: "Meta Platforms Ltd., Sony AI"

---

{% if page.academic_partners %}

## Academic Partners

{% for partner in page.academic_partners %}
<hr>
<h5><a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></h5>
{% if partner.subtext %}
<p class="text-muted" style="font-style: italic; font-size: 1.1rem; margin-top: 0;">{{ partner.subtext }}</p>
{% endif %}
<p>{{ partner.description }}</p>
{% if partner.lab_members %}
<p class="text-muted small"><strong>Lab members involved:</strong> {{ partner.lab_members }}</p>
{% endif %}
{% if partner.external_collaborators %}
<p class="text-muted small"><strong>External collaborators:</strong> {{ partner.external_collaborators }}</p>
{% endif %}
{% endfor %}
{% endif %}

{% if page.industry_partners %}

## Industry Partners

{% for partner in page.industry_partners %}
<hr>
<h5><a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></h5>
<p>{{ partner.description }}</p>
{% if partner.lab_members %}
<p class="text-muted small"><strong>Lab members involved:</strong> {{ partner.lab_members }}</p>
{% endif %}
{% if partner.external_collaborators %}
<p class="text-muted small"><strong>External collaborators:</strong> {{ partner.external_collaborators }}</p>
{% endif %}
{% endfor %}
{% endif %}

{% if page.research_networks %}

## Research Networks

{% for partner in page.research_networks %}
<hr>
<h5><a href="{{ partner.url }}" target="_blank">{{ partner.name }}</a></h5>
<p>{{ partner.description }}</p>
{% if partner.lab_members %}
<p class="text-muted small"><strong>Lab members involved:</strong> {{ partner.lab_members }}</p>
{% endif %}
{% if partner.external_collaborators %}
<p class="text-muted small"><strong>External collaborators:</strong> {{ partner.external_collaborators }}</p>
{% endif %}
{% endfor %}
{% endif %}

## Interested in collaborating?

We are always open to new collaborations with researchers and industry partners working on related topics. Please [get in touch](/get-involved/).
