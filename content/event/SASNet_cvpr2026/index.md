---
title: 'Presentation of SASNet @ CVPR 2026'

event: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR 2026)'
event_url: https://cvpr.thecvf.com/Conferences/2026

location: 'Colorado Convention Center, Denver, CO, USA'

summary: 'We present our CVPR 2026 paper "SASNet: Spatially-Adaptive Sinusoidal Networks for INRs" at the IEEE/CVF Conference on Computer Vision and Pattern Recognition.'

# Talk start and end times.
date: '2026-06-03'
date_end: '2026-06-07'
all_day: true

authors:
  - Haoan Feng

tags: ['INR', 'Neural Representation', 'Sinusoidal Neural Network', 'Spatial-Adaptive']

# Is this a featured talk? (true/false)
featured: true

url_project: 'https://fengyee.github.io/SASNet_inr/'
url_slides: ''
url_video: 'https://www.youtube.com/watch?v=mds9ux0_X-8'
---

### Abstract

<span style='font-size:15px'>*Sinusoidal neural networks (SIRENs) are powerful implicit neural representations (INRs) for low-dimensional signals in vision and graphics. By encoding input coordinates with sinusoidal functions, they enable high-frequency image and surface reconstruction. However, training SIRENs is often unstable and highly sensitive to frequency initialization: small frequencies produce overly smooth reconstructions in detailed regions, whereas large ones introduce spurious high-frequency components that manifest as noise in smooth areas such as image backgrounds. To address these challenges, we propose SASNet, a Spatially-Adaptive Sinusoidal Network that couples a frozen frequency embedding layer, which explicitly fixes the network's frequency support, with jointly learned spatial masks that localize neuron influence across the domain. This pairing stabilizes optimization, sharpens edges, and suppresses noise in smooth areas. Experiments on 2D image and 3D volumetric data fitting as well as signed distance field (SDF) reconstruction benchmarks demonstrate that SASNet achieves faster convergence, superior reconstruction quality, and robust frequency localization -- assigning low- and high-frequency neurons to smooth and detailed regions respectively -- while maintaining parameter efficiency.*</span>

More can be found on the [project page](https://fengyee.github.io/SASNet_inr/) and in the [paper](../../publication/feng-2026-sasnet/). Here is a short presentation of the work:

{{< youtube mds9ux0_X-8 >}}
