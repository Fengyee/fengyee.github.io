---
title: 'ImplicitTerrainV2: Wavelet-Guided Spatially Adaptive Neural Terrain Representation'
authors:
- Haoan Feng
- Xin Xu
- Leila De Floriani

highlight_name: true

date: '2026-11-03'
publishDate: '2026-08-08'
publication_types:
- paper-conference
publication: 'In *Proceedings of the 34th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems (**SIGSPATIAL ''26**)*, to appear'
publication_short: 'In *ACM SIGSPATIAL 2026*, to appear'
# ACM DOI not yet assigned (camera-ready in preparation); fill in once available.
doi: ''

abstract: 'Digital elevation models (DEMs) underpin terrain analysis in Geographic Information Systems (GIS), but in their common raster form, they rely on interpolation for off-grid sampling and finite-difference operators for derivative-based analysis. Implicit neural representations (INRs) offer a continuous alternative, but prior terrain INRs lack explicit frequency control, neglect the gradient structure of terrain, and remain too large and costly to train for practical deployment. We present ImplicitTerrainV2, which advances terrain INRs toward a compact, efficient neural terrain data format by combining a spectral control mechanism with wavelet-guided spatial adaptivity, derivative-aware supervision, and post-training model compression. At its core, a wavelet complexity field (WCF) derives spatially-adaptive frequency masks from analytically computed wavelet coefficients, localizing high-frequency capacity to complex terrain regions. The same field guides complexity-aware adaptive sampling that concentrates training in high-complexity regions, while gradient matching applies extra supervision to enforce the smooth manifold structure of terrain DEMs for improved derivative fidelity. Post-training mixed-precision quantization and entropy coding reduce storage to 1.23 bpp with a 0.28 dB PSNR drop. On 50 Swiss terrain tiles, ImplicitTerrainV2 reaches 66.25 dB end-to-end PSNR, improving over the prior work by 5.70 dB while using 3.2x fewer parameters and training in 55 s per tile on a single GPU. Our compressed neural format is competitive with several established DEM codecs in rate-distortion performance, while additionally supporting off-grid point queries, closed-form derivative evaluation, and resolution-independent reconstruction, which may benefit many downstream GIS applications.'

tags:
  - INR
  - Terrain
  - Geospatial
  - Neural Representation
  - Compression

featured: true

summary: 'A wavelet-guided, spatially adaptive implicit neural representation for digital elevation models. A wavelet complexity field localizes high-frequency capacity to complex terrain, and post-training compression reaches 1.23 bpp — 66.25 dB PSNR on Swiss terrain tiles, +5.70 dB over prior work with 3.2x fewer parameters.'

links:
 - name: arXiv
   url: 'https://arxiv.org/abs/2605.22556'
---

{{% callout note %}}
**Accepted as a full (research track) paper at [ACM SIGSPATIAL 2026](https://sigspatial2026.sigspatial.org/)**, Riverside, CA, November 3–6, 2026.

A follow-up to [ImplicitTerrain](https://fengyee.github.io/implicit-terrain/) (CVPR 2024 INRV Workshop), advancing terrain INRs toward a compact, efficient neural terrain data format with wavelet-guided spatial adaptivity, derivative-aware supervision, and post-training compression.
{{% /callout %}}
