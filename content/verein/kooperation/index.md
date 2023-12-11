---
title: Kooperationen
date: "2018-06-28T00:00:00Z"

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?

# Optional header image (relative to `assets/media/` folder).
header:
  caption: ""
  image: ""

sections:
  # A section to display blog posts
  - block: collection
    id: section-1
    content:
      subtitle: Auf dieser Seite findet Ihr unsere verschiedenen Kooperationspartner
      # Display content from the `content/post/` folder
      filters:
        folders:
          - kooperation
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: showcase
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: false
---