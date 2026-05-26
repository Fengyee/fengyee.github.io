---
title: 'A Parallel Scale-Space Method for Critical Features Tracking on Triangulated Irregular Networks'
authors:
- Haoan Feng
- Yunting Song
- Leila De Floriani

highlight_name: true

date: '2026-05-08'
# publishDate: '2026-05-08'
publication_types:
- article-journal
publication: In *ACM Transactions on Spatial Algorithms and Systems* (**TSAS**)
doi: '10.1145/3812549'

abstract: 'The scale-space method is a well-established framework that constructs a hierarchical representation of an input signal and facilitates coarse-to-fine reasoning about its features. Considering the terrain elevation function as the input signal, the scale-space method can identify and track significant topographic features across different scales. The persistence of a feature, called its life span, indicates its importance and enables the automatic selection of critical features for applications such as cartography, nautical charting, and land-use planning. Traditional scale-space methods rely on gridded Digital Elevation Models (DEMs), which lack the flexibility to adapt to irregular input distributions and varied terrain complexity. In contrast, Triangulated Irregular Networks (TINs) can be directly generated from irregular point clouds and naturally preserve key features. In this work, we introduce a novel scale-space analysis pipeline for TINs, addressing the challenges in extending grid-based scale-space methods to irregular meshes. Building on our prior conference version, we further extend the pipeline in several directions: (i) a scale-aware, seam-free sampling strategy (S3) for high-quality TIN construction, (ii) an improved TIN smoothing method that combines virtual neighbors and angle re-weighting with a quantitative evaluation of geometric and gradient fidelity, and (iii) a fully parallel critical point tracking algorithm that eliminates global sorting and achieves substantial GPU speedups. Comprehensive experiments demonstrate that our TIN-based pipeline achieves superior geometric and topological fidelity, improved efficiency, and stronger resolution robustness than grid-based methods, making it a scalable and accurate framework for multi-scale terrain analysis.'

tags:
  - Geospatial
  - Topology
  - TIN
  - Scale-Space
  - CUDA
  - GPU
  - Parallel

featured: true

links:
 - name: ACM
   url: 'https://dl.acm.org/doi/10.1145/3812549'

url_poster: ''
url_project: 'https://fengyee.github.io/tin-scale-space'
url_slides: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  focal_point: 'Center'
  preview_only: false
---
{{% callout note %}}
Published in **ACM Transactions on Spatial Algorithms and Systems (TSAS)**. This is the extended journal version of our SIGSPATIAL'24 conference paper [Critical Features Tracking on Triangulated Irregular Networks by a Scale-Space Method](../feng-2024-critical/), with new contributions in scale-aware seam-free sampling (S3), improved TIN smoothing, and a fully parallel GPU implementation of critical point tracking.
{{% /callout %}}
