---
title: Kooperationen
date: "2018-06-28T00:00:00Z"
type: landing

# # Optional header image (relative to `assets/media/` folder).
# header:
#   caption: ""
#   image: ""

sections:
  - block: markdown
    id: intro
    content:
      title:
      subtitle:
      text: Auf dieser Seite findet Ihr unsere verschiedenen Kooperationspartner
  - block: collection
    id: cooperations
    content:
      # Display content from the folder `/verein/kooperation`
      filters:
        folders:
          - verein/kooperation
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: showcase
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: false
---