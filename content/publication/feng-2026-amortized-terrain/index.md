---
title: 'Rethinking Amortized Neural Representations for High-Resolution Terrain Elevation Data'
authors:
- Haoan Feng
- Xin Xu
- Leila De Floriani

highlight_name: true

date: '2026-11-03'
publishDate: '2026-08-08'
publication_types:
- paper-conference
publication: 'Poster paper, in *Proceedings of the 34th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems (**SIGSPATIAL ''26**)*, to appear'
publication_short: 'Poster, in *ACM SIGSPATIAL 2026*, to appear'
# ACM DOI not yet assigned (camera-ready in preparation); fill in once available.
doi: ''

abstract: 'Implicit neural representations (INRs) model a signal as a continuous coordinate-to-value function. For terrain elevation data, this supports analytic derivatives, arbitrary-resolution decoding, and a smooth surface model of the underlying heightfield. However, fitting and storing a separate INR for every tile does not scale to large terrain datasets. Amortized neural representations reduce this cost with a shared network: a new tile is mapped to a compact per-tile payload, and a shared decoder reconstructs the heightfield from it. Most such methods are hypernetworks that predict the payload in a single forward pass, while others recover it through a short per-tile optimization. These methods were developed primarily for natural images, and their suitability for terrain heightfields remains unclear. We introduce a controlled benchmark on a 1 m/pixel terrain dataset and evaluate three representative methods under a unified protocol. Observing a clear cross-domain gap, we propose HUVR+SIREN, a hypernetwork that adapts the strongest benchmarked method (HUVR) by replacing its coordinate decoder with a smooth, analytically differentiable one. It attains the best height and derivative fidelity on the benchmark with no additional per-tile storage and lower decode cost, and tolerates aggressive post-training quantization with negligible quality loss, giving a compact terrain neural format. Ablations and diagnostics further identify which design choices transfer to terrain and show that the per-tile bottleneck is already near its useful limit, leaving the remaining gap in the shared hypernetwork''s architectural design.'

tags:
  - INR
  - Terrain
  - Geospatial
  - Neural Representation
  - Amortized Representation
  - Compression

featured: true

summary: 'A controlled benchmark of amortized neural representations on high-resolution (1 m/pixel) terrain elevation data, and HUVR+SIREN — a hypernetwork with a smooth, analytically differentiable decoder that attains the best height and derivative fidelity with no extra per-tile storage.'

links:
 - name: arXiv
   url: 'https://arxiv.org/abs/2606.00404'
---

{{% callout note %}}
**Accepted as a poster paper at [ACM SIGSPATIAL 2026](https://sigspatial2026.sigspatial.org/)**, Riverside, CA, November 3–6, 2026.

A controlled benchmark of amortized neural representations on high-resolution (1 m/pixel) terrain elevation data, and **HUVR+SIREN** — a hypernetwork with a smooth, analytically differentiable decoder that attains the best height and derivative fidelity with no extra per-tile storage. Part of our ongoing work on neural terrain representations, alongside [ImplicitTerrain](https://fengyee.github.io/implicit-terrain/) and ImplicitTerrainV2.
{{% /callout %}}
