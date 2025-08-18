---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-09-15
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: Haoan Feng
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Latest CV
        url: uploads/cv_2025_08.pdf
    design:
      css_class: light
      spacing:
        padding:
          top: "2rem"
          bottom: "2rem"
      background:
        color: system
        # image:
        #   # Add your image background to `assets/media/`.
        #   filename: ''
        #   filters:
        #     brightness: 1.0
        #   size: cover
        #   position: center
        #   parallax: false
  - block: markdown
    id: news
    content:
      title: 'News'
      subtitle: ''
      text: |-
        * **[Aug. 2025]** Completed a rewarding summer journey as a **PhD Research Intern** at [Dolby Laboratories – Advanced Technology Group (ATG)](https://www.dolby.com/).  Grateful to my mentor [Harsha Musunuri](https://www.linkedin.com/in/harsha-musunuri/) and manager [Guan-ming Su](https://www.linkedin.com/in/guan-ming-su-74968b5/) for their guidance and support throughout this internship. 🎉
        * **[Mar. 2025]** Our paper **SASNet** that enables sinusoidal neural networks with spatial-awareness is now available on [Arxiv](https://arxiv.org/abs/2503.09750). 🎉
        * **[Oct. 2024]** Our paper [scale space for TINs](https://fengyee.github.io/tin-scale-space) received the **best paper runner-up** at [ACM SIGSPAITAL2024](https://sigspatial2024.sigspatial.org/). 🎉
        * **[Aug. 2024]** We have one [paper](https://arxiv.org/abs/2409.06638) accepted as **Oral presentation** at [ACM SIGSPAITAL2024](https://sigspatial2024.sigspatial.org/) See you @Georgia. 🎉
        * **[Apr. 2024]** Our paper [ImplicitTerrain](https://fengyee.github.io/implicit-terrain/) is accepted as **Oral presentation** at [INRV2024 (CVPR2024)](https://inrv.github.io/). See you @Seattle. 🎉
        * **[Aug. 2021]** First day at [University of Maryland, College Park](https://www.umd.edu/), working with [Prof. Leila De Floriani](https://users.umiacs.umd.edu/~deflo/). 🎉
    design:
      background:
        color: "#f7f7f7"
        text_color_light: false
      spacing:
        padding:
          top: "2rem"
          bottom: "2rem"
  - block: collection
    id: publications
    content:
      title: Recent Publications
      text: ""
      count: 4
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: card
      style:
        max-width: 500px
      spacing:
        padding:
          top: "2rem"
          bottom: "2rem"
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Presentations
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 2
      background:
        color: "#f7f7f7"
        text_color_light: false
---
