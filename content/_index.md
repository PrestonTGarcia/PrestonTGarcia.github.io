---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
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
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-

        My mission is to apply my research objectives to develop innovations that help the communities that I come from, whether that be the world, or where I grew up in - Hawai'i.

        I work on projects relating to the applications of AI, ML, data science, and mathematics to physical science fields such as physics and atmospheric sciences.

        Please feel free to reach out to collaborate.

    design:
      columns: '1'
  - block: markdown
    content:
      title: 'Featured Projects'
      subtitle: ''
      filters:
        folders:
          - project
        featured_only: true
        design:
          view: article-grid
          columns: 3


---
