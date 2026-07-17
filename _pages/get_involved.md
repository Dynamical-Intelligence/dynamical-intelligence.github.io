---
layout: page
title: Get Involved
permalink: /get-involved/
nav: true
nav_order: 8

# --- YOUR DATA SECTION ---
open_positions:
  - title: "Research Assistant in Multimodal Machine Perception & Generative AI"
    body: |
      The core bottleneck in spatial computing is real-world multimodal data. Existing datasets are either spatially blurred, too narrow in scope, or synthetic. We're capturing our own: 360° video, 64-channel full-sphere audio, egocentric perspective with head-tracked signals, and sub-millimetre source tracking; across real kitchens, lounges, and meeting rooms.

      You'll use this to train latent diffusion models and multimodal transformers for scene synthesis, enhancement, and object segmentation. Your models will anchor generative multimodal AI workshops and challenges at international venues.
    requirements_label: "Skills"
    requirements: "multimodal signal processing, generative modelling (diffusion models, transformers), data capture and pipeline engineering. Prior experience with multimodal signal processing is a real advantage."
    # terms: "Optional — overrides the shared contract terms above for this position only."
  - title: "Research Assistant in Dynamically-Grounded Neural Architectures"
    body: |
      Gradient descent keeps accidentally discovering mathematical structures (limit cycles, coupled oscillators, attractor geometry) that we already have precise theories for. It rediscovers them blindly, expensively, and in a form that remains analytically inaccessible after training. This project starts from the other end: networks with units that are known dynamical-systems equations, interpretable by design rather than reverse-engineered after the fact.
    requirements_label: "You'll need"
    requirements: "experience scaling deep learning training and solid mathematical foundations in linear algebra and dynamical systems theory. You will be turning theory into concrete architectures, experiments, and evidence."
    # terms: "Optional — overrides the shared contract terms above for this position only."
---

We are always looking for motivated people to join the lab, whether as a research assistant, postdoc, PhD student, masters or undergraduate researcher, or short-term visitor. The lab is based in the [School of Electronic Engineering and Computer Science (EECS)](https://www.qmul.ac.uk/eecs/) at [Queen Mary University of London](https://www.qmul.ac.uk/), on the Mile End campus in East London. Get in touch with the PI to discuss how you could get involved.

## Open positions

Two Research Assistant positions (6-month contracts; part time or full time) starting as soon as possible. You must have the right to work in the UK. Apply to one position only.

**To apply**: email [i.roman@qmul.ac.uk](mailto:i.roman@qmul.ac.uk) including a short note with your interest and fit & a 1-page resume. Also feel free to email me if you have questions.

{% for position in page.open_positions %}

<div class="card border-0 shadow-sm p-4 mb-4" markdown="1">

#### {{ position.title }}

{{ position.body }}

{% if position.requirements %}**{{ position.requirements_label }}:** {{ position.requirements }}{% endif %}

{% if position.terms %}**Terms:** {{ position.terms }}{% endif %}

</div>

{% endfor %}

## Postdoctoral researchers

The lab welcomes postdocs via funding mechanisms such as:

- [Marie Skłodowska-Curie Actions Postdoctoral Fellowships](https://marie-sklodowska-curie-actions.ec.europa.eu/actions/postdoctoral-fellowships)
- [Royal Academy of Engineering Research Fellowships](https://raeng.org.uk/research-fellowships)
- [Royal Society grants and fellowships](https://royalsociety.org/grants/), such as the University Research Fellowship and Newton International Fellowship
- [UKRI funding opportunities](https://www.ukri.org/opportunity/), including grants naming you as a co-investigator

Get in touch with the PI well ahead of the application deadline to discuss a joint research grant submission to fund your postdoctoral work in the lab.

## PhD students

The lab welcomes enthusiastic PhD students from diverse backgrounds. You would apply to the PhD in Computer Science at Queen Mary through [EECS's research degrees programme](https://www.qmul.ac.uk/eecs/phd/), following the school's [how-to-apply guide](https://www.qmul.ac.uk/eecs/phd/how-to-apply/).

Funding routes include:

- **Funded studentships** – advertised under [Open Positions](#open-positions) above when available
- **Competitive QMUL funding** – see [Funding a PhD](https://www.qmul.ac.uk/postgraduate/research/funding_phd/) and the [scholarships database](https://www.qmul.ac.uk/scholarships/database/)
- **External funding** – PhD fellowships or scholarships from bodies outside Queen Mary
- **Self-funding**

Get in touch with the PI to explore options, discuss potential projects, or ask any questions.

If you're already a PhD student at another institution, you're welcome to collaborate with the lab, including through a research visit (see Visiting researchers below).

## Masters students

**Queen Mary students** can do their masters thesis in the lab. Space is limited each year and offered based on project fit and on a first-come, first-served basis, so get in touch with the PI as early as possible.

**Masters students from other universities** are also welcome and may be eligible for funding through programmes such as the [IEEE SPS Signal Processing Mentorship Academy (SigMA)](https://signalprocessingsociety.org/professional-development/signal-processing-mentorship-academy-sigma-program).

## Undergraduate students

Queen Mary undergraduates can do their thesis project in the lab. As with masters projects, space is limited each year and offered based on project fit and on a first-come, first-served basis. Get in touch with the PI to discuss.

Paid Research Assistant positions are advertised under [Open Positions](#open-positions) above.

## Visiting researchers

PhD students and researchers from universities, industry, and other organisations are welcome to visit the lab for research stays ranging from a few weeks to several months, depending on the nature of the collaboration. Get in touch with the PI to discuss potential research visits.
