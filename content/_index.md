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
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: View CV
        url: uploads/resume.pdf
    design:
      css_class: light
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
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Please reach out to collaborate 😃
  #   design:
  #     columns: '1'
  - block: markdown
    id: news
    content:
      title: 'News'
      subtitle: ''
      text: |-
        * [date] name1
        * [date] name2
        * [date] name3
    design:
      background:
        color: "#f7f7f7"
        text_color_light: false
  - block: collection
    id: publications
    content:
      title: Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Presentations
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
