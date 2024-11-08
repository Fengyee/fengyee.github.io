---
title: Critical Features Tracking on Triangulated Irregular Networks by a Scale-Space
  Method
authors:
- Haoan Feng
- Yunting Song
- Leila De Floriani

highlight_name: true

date: '2024-09-14'
# publishDate: '2024-09-15'
publication_types:
- paper-conference
publication: In *The 32nd ACM International Conference on Advances in Geographic Information Systems (SIGSPATIAL ’24)*. **(Oral Presentation)**
doi: '10.1145/3678717.3691218'

abstract: 'The scale-space method is a well-established framework that constructs a hierarchical representation of an input signal and facilitates coarse-to-fine visual reasoning. Considering the terrain elevation function as the input signal, the scale-space method can identify and track significant topographic features across different scales. The number of scales a feature persists, called its life span, indicates the importance of that feature. In this way, important topographic features of a landscape can be selected, which are useful for many applications, including cartography, nautical charting, and land-use planning. The scale-space methods developed for terrain data use gridded Digital Elevation Models (DEMs) to represent the terrain. However, gridded DEMs lack the flexibility to adapt to the irregular distribution of input data and the varied topological complexity of different regions. Instead, Triangulated Irregular Networks (TINs) can be directly generated from irregularly distributed point clouds and accurately preserve important features. In this work, we introduce a novel scale-space analysis pipeline for TINs, addressing the multiple challenges in extending grid-based scale-space methods to TINs. Our pipeline can efficiently identify and track topologically important features on TINs. Moreover, it is capable of analyzing terrains with irregular boundaries, which poses challenges for grid-based methods. Comprehensive experiments show that, compared to grid-based methods, our TIN-based pipeline is more efficient, accurate, and has better resolution robustness.'

tags:
  - Geospatial
  - Topology
  - TIN
  - Scale-Space

featured: true


links:
 - name: Arxiv
   url: 'https://arxiv.org/abs/2409.06638'

url_poster: ''
url_project: 'https://fengyee.github.io/tin-scale-space'
url_slides: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  focal_point: 'Center'
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---
{{% callout note %}}
You can find the slides and a 15 mins presentation on the project page [here](https://fengyee.github.io/tin-scale-space).
{{% /callout %}}
