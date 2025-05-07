---
title: 'Presentation of Scale Space for TINs @ ACM SIGSPATIAL2024'

event: '32nd ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems'
event_url: https://sigspatial2024.sigspatial.org/

location: 'Atlanta, GA, USA'
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: 'Oral presentation of our paper "Critical Features Tracking on Triangulated Irregular Networks by a Scale-Space Method" at the 32nd ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-10-29'
date_end: '2024-11-01'
all_day: true

# Schedule page publish date (NOT talk date).
# publishDate: '2017-01-01T00:00:00Z'/

authors:
  - Haoan Feng

tags: ['Geospatial', 'Topology', 'TIN', 'Scale Space']

# Is this a featured talk? (true/false)
featured: true

image:
  caption: ''
  focal_point: Center

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen

url_project: ''
url_slides: ''
# url_video: 'https://youtube.com'

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects:
#   - example
---

### Abstract

<span style='font-size:15px'>*The scale-space method is a well-established framework that constructs a hierarchical representation of an input signal and facilitates coarse-to-fine visual reasoning. Considering the terrain elevation function as the input signal, the scale-space method can identify and track significant topographic features across different scales. The number of scales a feature persists, called its life span, indicates the importance of that feature. In this way, important topographic features of a landscape can be selected, which are useful for many applications, including cartography, nautical charting, and land-use planning. The scale-space methods developed for terrain data use gridded Digital Elevation Models (DEMs) to represent the terrain. However, gridded DEMs lack the flexibility to adapt to the irregular distribution of input data and the varied topological complexity of different regions. Instead, Triangulated Irregular Networks (TINs) can be directly generated from irregularly distributed point clouds and accurately preserve important features. In this work, we introduce a novel scale-space analysis pipeline for TINs, addressing the multiple challenges in extending grid-based scale-space methods to TINs. Our pipeline can efficiently identify and track topologically important features on TINs. Moreover, it is capable of analyzing terrains with irregular boundaries, which poses challenges for grid-based methods. Comprehensive experiments show that, compared to grid-based methods, our TIN-based pipeline is more efficient, accurate, and has better resolution robustness.*</span>

More can be found at the [project page](https://fengyee.github.io/tin-scale-space/). Here is a 15 mins presentation of the project:
{{< youtube vq5w7P8yFxU >}}
