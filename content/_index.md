---
title: ""
# <title> / og:title for the homepage
seo:
  title: 'Haoan Feng · 3D Vision & Neural Representations · UMD'
date: 2024-09-15
type: landing
design:
  spacing: "0"
sections:
  - block: academic-home
    id: about
    content:
      username: Haoan Feng
      cv: uploads/cv_2026_11.pdf
      tagline: 'Spatial intelligence through world models built on **explicit 3D representations**: neural fields, Gaussian splats, and triangulated meshes, where scene structure is something you can query, differentiate, and edit.'
      status: 'Open to full-time Research Scientist / Engineer roles in 3D vision'
      status_detail: 'Graduating Summer 2027'
      # Hero media: `feature` plays that paper's `home_video`; `caption` says what the demo shows.
      hero:
        feature: feng-2026-ffgausstype
        caption: 'Text and icons become relightable Gaussian assets inside 4D-Gaussian video, in one 9.1 ms forward pass.'
      highlights:
        - label: Papers at
          items:
            - CVPR 2026
            - ACM SIGSPATIAL 2026
            - ACM TSAS
        - label: Research internships
          items:
            - Dolby Laboratories ATG (2025, 2026)
        - label: Recognition
          items:
            - SIGSPATIAL ’24 Best Paper Runner-up
            - OASIS ’26 Top-10 Finalist
        - label: Reviewer
          items:
            - CVPR
            - ICCV
            - ECCV
            - NeurIPS
      # Cards under "Outside the lab" (content/project/<slug>/).
      outside_projects:
        - meowverse
      # Card next to the outside-the-lab projects (image under assets/).
      life:
        image: media/bella.jpg
        alt: 'Bella the cat, asleep on a blue blanket'
        text: '**Bella**, my cat, and the muse behind Meowverse.'
      # Homepage shows the first N news items; the full list stays on /news/.
      news_count: 4
      # Homepage shows the N most recent talks; the full list stays on /event/.
      talks_count: 4
      selected:
        - feng-2026-ffgausstype
        - feng-2026-sasnet
        - feng-2026-implicitterrain-v2
        - feng-2026-tsas-scale-space
        - feng-2026-geometry-guided-camera-motion
      news:
        - date: Nov. 2026
          text: 'New preprint [FFGaussType: Feed-Forward Conversion of Glyph and SVG Geometry into Compact Gaussian Assets](/publication/feng-2026-ffgausstype/), from my 2026 internship at [Dolby Laboratories – Advanced Technology Group (ATG)](https://www.dolby.com/). It brings text and icons into volumetric videos built on 4D Gaussians: one 9.1 ms forward pass turns a glyph or SVG outline into a relightable Gaussian asset. Paper on [arXiv](https://arxiv.org/abs/2611.26431), videos on the [project page](https://fengyee.github.io/FFGaussType/).'
        - date: Nov. 2026
          text: 'At **ACM SIGSPATIAL in Riverside**, I presented [ImplicitTerrainV2](/publication/feng-2026-implicitterrain-v2/) in an oral session and [our work on amortized terrain representations](/publication/feng-2026-amortized-terrain/) in a lightning talk and poster session. Xin Xu, Yutian Tao, and I also participated in the [OASIS Student Challenge](/publication/tao-2026-topology-guided-geoai/) as a team with our urban flood screening project.'
        - date: Oct. 2026
          text: 'The [preprint](https://arxiv.org/abs/2610.30660) for our [topology-guided GeoAI agent](/publication/tao-2026-topology-guided-geoai/) is now available. The project is a **top-10 finalist at [OASIS 2026](https://rsvp.withgoogle.com/events/oasis-2026/)**, the ACM SIGSPATIAL student challenge. Our team received a **Google DeepMind Student Travel Grant** and was selected for an on-site presentation and demo.'
        - date: Aug. 2026
          text: '[ImplicitTerrainV2](https://arxiv.org/abs/2605.22556) (full paper) and [Amortized Terrain](https://arxiv.org/abs/2606.00404) (poster) accepted at **ACM SIGSPATIAL 2026**.'
        - date: Aug. 2026
          text: 'Our [parallel scale-space method for TINs](https://dl.acm.org/doi/10.1145/3812549) is published in **ACM TSAS**.'
        - date: May 2026
          text: 'Returned to **Dolby ATG** to lead research on text and icons as native Gaussian-splatting assets.'
        - date: May 2026
          text: 'New [Amortized Terrain preprint](https://arxiv.org/abs/2606.00404): compact neural representations for terrain heightfields.'
        - date: May 2026
          text: 'New [ImplicitTerrainV2 preprint](https://arxiv.org/abs/2605.22556): wavelet-guided, spatially adaptive neural terrain modeling.'
        - date: Mar. 2026
          text: '[Geometry-Guided Camera Motion Understanding](https://arxiv.org/abs/2603.13119) accepted at **CVPR 2026 Workshop PVUW**.'
        - date: Mar. 2026
          text: '[SASNet](https://arxiv.org/abs/2503.09750) accepted at **CVPR 2026**. See you in Denver!'
        - date: Aug. 2025
          text: 'Completed my first **Dolby ATG research internship**, working on camera motion understanding in VideoLLMs.'
    design:
      spacing:
        padding:
          top: "0"
          bottom: "0"
---
