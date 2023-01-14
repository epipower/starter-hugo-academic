---
title: Epipower
type: landing
sections:
  - block: markdown
    id: home
    content:
        title:
        subtitle:
        text: <img src="cutted.png"/>
    design:
      columns: '2'
      background:
        color: 'rgb(29,35,67)' #rgb(41,41,46)
        text_color_light: true
      spacing:
         # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["20px", "0", "20px", "0"]
  - block: collection
    id: posts
    content:
      title: Aktuelles
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projekte
      filters:
        folders:
          - project
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: contact
    id: contact
    content:
      title: Kontakt
      email: info@epipower.de
      # Automatically link email and phone or display as text
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
