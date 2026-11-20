---
title: 'FFGaussType: Feed-Forward Conversion of Glyph and SVG Geometry into Compact Gaussian Assets'
authors:
- Haoan Feng
- Tianfu Wang
- Peimeng Guan
- Dae Yeol Lee
- Guan-Ming Su

highlight_name: true

date: '2026-11-19'
publishDate: '2026-11-19'
publication_types:
- article
publication: 'Preprint'

abstract: 'Immersive 3D content allows text and graphical elements, such as subtitles, annotations, and icons, to be placed inside a scene rather than displayed as flat overlays. Placed this way, they respect occlusion and perspective and take on user-assigned materials and lighting while preserving their original shapes. In Gaussian scenes, however, each new glyph or icon requires its own iterative optimization, which limits scalable content creation. We present FFGaussType, which converts extruded glyph and SVG outlines into Gaussian assets in a single forward pass. A point encoder maps anchors sampled on the known surface to a single feature plane, from which a decoder shared by all assets predicts neural Gaussians carrying surface normals. This separates geometric conversion from material and lighting choices, and the feature plane supports image and video coding for compact delivery. We construct a paired dataset of 27,221 glyph and SVG icon assets with anchors and calibrated normal and silhouette renderings, holding out font families for evaluation. Conversion from prepared anchors takes 9.1 ms per asset, at a fraction of the compute and memory of prior baselines. On unseen font families and test icons, FFGaussType achieves 1.62° normal error and 0.985 silhouette IoU, the best among the compared feed-forward converters, matching the fidelity that per-asset fitting needs thousands of steps to reach. The code and dataset will be released after publication.'

tags:
  - Gaussian Splatting
  - 4D Gaussians
  - Volumetric Video
  - Feed-Forward 3D
  - Typography

featured: true

summary: 'Bring text and icons into volumetric videos built on 4D Gaussians. FFGaussType converts a glyph or SVG outline into a relightable Gaussian asset in a single 9.1 ms forward pass, so creators can restyle material and lighting freely.'

url_pdf: 'https://arxiv.org/pdf/2611.26431'
url_project: 'https://fengyee.github.io/FFGaussType/'
links:
  - name: arXiv
    url: 'https://arxiv.org/abs/2611.26431'
---

{{% callout note %}}
Developed during my 2026 summer internship at Dolby Laboratories – Advanced Technology Group (ATG). Paper on [arXiv](https://arxiv.org/abs/2611.26431); videos and results on the [project page](https://fengyee.github.io/FFGaussType/).
{{% /callout %}}
