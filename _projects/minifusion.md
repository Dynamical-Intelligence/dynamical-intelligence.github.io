---
layout: page
title: "Minifusion: Reimagining Sound Design for Live Instruments"
description:
img: assets/img/projects/minifusion_cropped.jpg
importance: 3
category: Current

---

Minifusion is an audio plugin for sound-based transformations of musical instruments that allows you to shape the sound of an incoming audio signal in the likeness of other musical instruments, while running in real time and with low latency. 

<img src="/assets/img/projects/minifusion.png" alt="Minifusion plugin" style="width: 100%; height: auto; margin-bottom: 1rem;">

This project is motivated by the difficulty for musicians playing non-keyboard musical instruments (e.g. guitarists, vocalists, percussionists) to access to a wide variety of sounds. This is because many production tasks such as music sketching, composition in Digital Audio Workstations, and sound design require an interaction paradigm centered around keyboard interfaces and MIDI, which is inherently incompatible with the embodied, continuous, and contextual mechanisms of interaction with non-keyboard instruments.

The plugin and neural network design have been in continuous development in collaboration with musicians and a composer, and to date, affords transformations of different audio sources such as guitar and voice into other specific instruments (like a rompler but without MIDI!). It is also possible to train custom models. Future development includes expanding the sound shaping possibilities.
‍
This plugin implements two main features to afford natural control for instrumentalists, stemming from research conducted at the lab: (1) the use of continuous representations with space for ambiguity, which holds potential for meaning-making when playing live, and (2), such representations are learned in low-latency autoencoders that support low latency and jitter, for intimate instrumental control.

It has been presented at different venues such as Sonar 2025, NIME, WASPAA, and ADC25. It has also been covered by online magazines on audio effects, bedroomproducers and kvraudio. Composer Ziyi Tao used it for his string quartet piece “There is an image by Paul Klee,” or, Recursivity and Simultaneity (2025)”, presented at Juilliard School, NYC, and Hochschule für Musik und Darstellende Kunst Frankfurt.

[Learn more on the project's website](https://minifusion.live)

<br>

#### Related Papers

<div class="publications">
{% bibliography --file minifusion --group_by none %}
</div>
