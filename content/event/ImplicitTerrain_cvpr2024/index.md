---
title: 'Presentation of ImplicitTerrain @ CVPR2024 INRV Workshop'

event: '1st Workshop on Implicit Neural Representation for Vision (CVPR2024)'
event_url: https://inrv.github.io/

location: 'Seattle Convention Center - Summit 335-336'
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: 'We present our CVPR 2024 paper "ImplicitTerrain: a Continuous Surface Model for Terrain Data Analysis" at the 1st Workshop on Implicit Neural Representation for Vision'
abstract: 'Digital terrain models (DTMs) are pivotal in remote sensing, cartography, and landscape management, requiring accurate surface representation and topological information restoration. While topology analysis traditionally relies on smooth manifolds, the absence of an easy-to-use continuous surface model for a large terrain results in a preference for discrete meshes. Structural representation based on topology provides a succinct surface description, laying the foundation for many terrain analysis applications. However, on discrete meshes, numerical issues emerge, and complex algorithms are designed to handle them. This paper brings the context of terrain data analysis back to the continuous world and introduces ImplicitTerrain, an implicit neural representation (INR) approach for modeling high-resolution terrain continuously and differentiably. Our comprehensive experiments demonstrate superior surface fitting accuracy, effective topological feature retrieval, and various topographical feature extraction that are implemented over this compact representation in parallel. To our knowledge, ImplicitTerrain pioneers a feasible continuous terrain surface modeling pipeline that provides a new research avenue for our community.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2024-06-18'
# date_end: '2030-06-01T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin

tags: ['INR', 'Geo', 'Topology']

# Is this a featured talk? (true/false)
featured: true

# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
#   focal_point: Right

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen

url_project: 'https://fengyee.github.io/implicit-terrain/'
url_arxiv: 'https://arxiv.org/abs/2406.00227'
url_slides: '/slides/ImpliciTerrain_slides.pdf'
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

{{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Hugo Blox Builder's [_Slides_](https://docs.hugoblox.com/reference/content-types/) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://docs.hugoblox.com/reference/markdown/).

Further event details, including [page elements](https://docs.hugoblox.com/reference/markdown/) such as image galleries, can be added to the body of this page.
