---
title: 'Adaptive Training of INRs via Pruning and Densification'
authors:
- Diana Aldana
- João Paulo Lima
- Daniel Csillag
- Daniel Perazzo
- Haoan Feng
- Luiz Velho
- Tiago Novello

date: '2025-10-27'
publishDate: '2025-10-27'
publication_types:
- article
publication: 'Preprint'

# Slug kept from the earlier "Structured Pruning in INRs (work in progress)" entry so its URL keeps working
# (the site sets disableAliases).

abstract: 'Encoding input coordinates with sinusoidal functions into multilayer perceptrons (MLPs) has proven effective for implicit neural representations (INRs) of low-dimensional signals, enabling the modeling of high-frequency details. However, selecting appropriate input frequencies and architectures while managing parameter redundancy remains an open challenge, often addressed through heuristics and heavy hyperparameter optimization schemes. In this paper, we introduce AIRe (Adaptive Implicit neural Representation), an adaptive training scheme that refines the INR architecture over the course of optimization. Our method uses a neuron pruning mechanism to avoid redundancy and input frequency densification to improve representation capacity, leading to an improved trade-off between network size and reconstruction quality. For pruning, we first identify less-contributory neurons and apply a targeted weight decay to transfer their information to the remaining neurons, followed by structured pruning. Next, the densification stage adds input frequencies to spectrum regions where the signal underfits, expanding the representational basis. Through experiments on images and SDFs, we show that AIRe reduces model size while preserving, or even improving, reconstruction quality.'

tags:
  - INR
  - Structured Pruning
  - Model Compression
  - Neural Representation
  - Sinusoidal Neural Network

featured: false

summary: 'AIRe adapts a sinusoidal INR during training: it prunes low-contribution neurons and adds input frequencies where the signal underfits, giving smaller models at the same or better reconstruction quality on images and SDFs.'

url_pdf: 'https://arxiv.org/pdf/2510.23943'

links:
 - name: arXiv
   url: 'https://arxiv.org/abs/2510.23943'
---
