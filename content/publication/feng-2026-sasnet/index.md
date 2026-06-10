---
title: 'SASNet: Spatially-Adaptive Sinusoidal Neural Networks'
authors:
- Haoan Feng
- Diana Aldana
- Tiago Novello
- Leila De Floriani
date: '2026-06-01'
publishDate: '2025-03-12'
publication_types:
- paper-conference
publication: 'In *Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR 2026)*'

abstract: 'Sinusoidal neural networks (SIRENs) are powerful implicit neural representations (INRs) for low-dimensional signals in vision and graphics. By encoding input coordinates with sinusoidal functions, they enable high-frequency image and surface reconstruction. However, training SIRENs is often unstable and highly sensitive to frequency initialization: small frequencies produce overly smooth reconstructions in detailed regions, whereas large ones introduce spurious high-frequency components that manifest as noise in smooth areas such as image backgrounds. To address these challenges, we propose SASNet, a Spatially-Adaptive Sinusoidal Network that couples a frozen frequency embedding layer, which explicitly fixes the network''s frequency support, with jointly learned spatial masks that localize neuron influence across the domain. This pairing stabilizes optimization, sharpens edges, and suppresses noise in smooth areas. Experiments on 2D image and 3D volumetric data fitting as well as signed distance field (SDF) reconstruction benchmarks demonstrate that SASNet achieves faster convergence, superior reconstruction quality, and robust frequency localization -- assigning low- and high-frequency neurons to smooth and detailed regions respectively -- while maintaining parameter efficiency.'

tags:
  - INR
  - Neural Representation
  - Spatial-Adaptive
  - Sinusoidal Neural Network
  - Neural Images

featured: true

links:
 - name: arXiv
   url: 'https://arxiv.org/abs/2503.09750'
 - name: Code
   url: 'https://github.com/Fengyee/SASNet_inr'

url_project: 'https://fengyee.github.io/SASNet_inr/'
# url_poster: ''
# url_slides: ''
---

{{% callout note %}}
SIRENs are powerful implicit neural representations, but they are highly sensitive to frequency initialization: low frequencies over-smooth fine detail, while high frequencies inject noise into smooth regions. **SASNet** addresses this with a fixed frequency embedding paired with jointly learned **spatially-adaptive masks** that localize each sinusoidal neuron's influence across the domain. The result is sharper reconstructions, less noise, and faster convergence across image fitting, 3D volumes, and SDF reconstruction — consistently outperforming INR baselines.

A collaboration between the **University of Maryland** and **IMPA**, with Haoan Feng, Diana Aldana, Tiago Novello, and Leila De Floriani.
{{% /callout %}}

## Cite

```bibtex
@inproceedings{feng2026sasnet,
  title     = {SASNet: Spatially-Adaptive Sinusoidal Neural Networks},
  author    = {Feng, Haoan and Aldana, Diana and Novello, Tiago and De Floriani, Leila},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2026}
}
```
