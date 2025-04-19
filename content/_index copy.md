---
title: ""
type: landing
layout: landing

design:
  spacing: "6rem"

sections:

  - block: resume-biography-3
    content:
      username: admin
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: collection
    id: news
    content:
      title: Recent News
      filters:
        page_type: post
      count: 5
    design:
      view: date-title-summary
      columns: 1      # <--- 这行是关键
      spacing:
        padding: [0, 0, 0, 0]


  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publication
    design:
      view: citation
      columns: 1

  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - talk
    design:
      view: article-grid
      columns: 1

  - block: collection
    id: teaching
    content:
      title: Teaching
      filters:
        folders:
          - teaching
    design:
      view: card
      columns: 2
---
