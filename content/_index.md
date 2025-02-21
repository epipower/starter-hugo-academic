---
title: Epilepsie Empowerment Deutschland e.V.
type: landing
sections:
  - block: markdown
    id: home
    content:
        title:
        subtitle:
        text: <img src="Header_Epipower.png"/>
    design:
      columns: '2'
      background:
        color: 'rgb(41,41,86)' #'rgb(29,35,67)'
        text_color_light: true
      spacing:
         # Customize the section spacing. Order is top, right, bottom, left.
        padding: ["20px", "0", "20px", "0"] #margin
  - block: features
    id: empowerment
    content:
      title: Empowerment
      subtitle:
      text:
      items:
        - name: Wir für dich
          description: <div align="justify"> Wir sind eine Gruppe junger Menschen, die alle von Epilepsie betroffen sind. Wir kümmern uns um den Ausbau von digitalen Selbsthilfeangeboten und vernetzen Menschen. Darüberhinaus arbeiten wir mit anderen Organisationen auf (inter-)nationaler zusammen, sprechen mit Vertretern der Krankenkassen, der Pharmaindustrie oder dem Gesetzgeber. Wir vertreten also deine und gleichzeitig unsere Interessen.</div>
          icon: users
          icon_pack: fas
        - name: Zoom Online Austauschtreffen
          description: <div align="justify"> Jeden ersten Dienstag im Monat starten wir ein Zoom-Meeting für Menschen, die von Epilepsie betroffen sind. Die Teilnehmer können sich in themenspezifischen Breakoutsessions über alle verschiedenen Themen rund um Epilepsie, aber auch Privates austauschen. Wir haben eine sehr lockere Atmosphäre und jeder kann kommen und gehen, wie es persönlich am angenehmsten ist. Über folgendes <a href="https://zoom.us/meeting/register/tJcqfu6tpzwqGtbQlfDq86UGrElPWfePiRjU"><b>Formular</b></a> kannst du dich anmelden.</div>
          icon: video
          icon_pack: fas
        - name: Discord Online Community
          description: <div align="justify"> Wie bewältigst du den Alltag mit deiner Epilepsie? Bist du zufrieden mit deiner Therapie? Kennst du andere Menschen, die von Epilepsie betroffen sind? Wir bieten dir eine Community zum Fragen stellen, Vernetzen und zum sich gegenseitig Austauschen. Dafür nutzen wir einen Discord Server. Bei Ausfüllen des folgenden <a href="https://www.survio.com/survey/d/Z9K5S9D8X4M5U4C5E"><b>Formulars</b></a> erhälst du einen Einladungslink per Mail.</div>
          icon: discord
          icon_pack: fab
    design:
        columns: '2'
  - block: collection
    id: news
    content:
      title: News
      subtitle: <br>
      count: 10
      filters:
        folders:
          - event
          - post
      archive:
        enable: false
    design:
      view: showcase
      #flip_alt_rows: false

    # - block: collection
    #   id: events
    #   content:
    #     title: Events
    #     subtitle:
    #     text:
    #     # Choose how many pages you would like to display (0 = all pages)
    #     count: 3
    #     # Filter on criteria
    #     filters:
    #       folders:
    #         - event
    #       author: ""
    #       category: ""
    #       tag: ""
    #       exclude_featured: false
    #       exclude_future: false
    #       exclude_past: false
    #       publication_type: ""
    #     # Choose how many pages you would like to offset by
    #     offset: 0
    #     # Page order: descending (desc) or ascending (asc) date.
    #     order: desc
    #   design:
    #     # Choose a layout view
    #     view: compact
    #     columns: '2'      
    # - block: portfolio
    #   id: projects
    #   content:
    #     title: Projekte
    #     filters:
    #       folders:
    #         - project
    #   design:
    #     # Choose how many columns the section has. Valid values: '1' or '2'.
    #     columns: '1'
    #     view: showcase
    #     # For Showcase view, flip alternate rows?
    #     flip_alt_rows: false
    # - block: collection
    #   id: blog
    #   content:
    #     title: Blog
    #     subtitle: "[Beitrag einreichen](mailto:info@epipower.de)"
    #     text:
    #     # Choose how many pages you would like to display (0 = all pages)
    #     count: 3
    #     # Filter on criteria
    #     filters:
    #       folders:
    #         - post
    #       author: ""
    #       category: ""
    #       tag: ""
    #       exclude_featured: false
    #       exclude_future: false
    #       exclude_past: false
    #       publication_type: ""
    #     # Choose how many pages you would like to offset by
    #     offset: 0
    #     # Page order: descending (desc) or ascending (asc) date.
    #     order: desc
    #   design:
    #     # Choose a layout view
    #     view: compact
    #     columns: '2'
    # - block: collection
    #   id: news
    #   content:
    #     title: News
    #     # subtitle: ''
    #     # text: 'Check out my recent blog posts below!'
    #     # Choose how many pages you would like to display (0 = all pages)
    #     count: 5
    #     # Filter on criteria
    #     filters:
    #       # The folders to display content from
    #       folders:
    #         - event
    #         - post
    #         - project
    #       author: ""
    #       category: ""
    #       tag: ""
    #       publication_type: ""
    #       featured_only: false
    #       exclude_featured: false
    #       exclude_future: false
    #       exclude_past: True
    #     # Choose how many pages you would like to offset by
    #     # Useful if you wish to show the first item in the Featured widget
    #     offset: 0
    #     # Field to sort by, such as Date or Title
    #     sort_by: 'Date'
    #     sort_ascending: false
    #   design:
    #     # Choose a listing view
    #     view: mansory
    #     # Choose single or dual column layout
    #     columns: '2'
  - block: team
    id: team
    content: 
      title: Team
      subtitle: <br>
      text: " "
      user_groups:
        - leaderboard
    design:
      background:
        color: "rgb(41,41,86)"
        text_color_light: true
      show_interests: false
      show_role: true
      show_organizations: false
      show_social: true
  - block: contact
    id: contact
    content:
      title: Kontakt
      email: info@epipower.de
      # Automatically link email and phone or display as text
      autolink: true
      contact_links:
        - icon: instagram
          icon_pack: fab
          name: epipower.de
          link: https://www.instagram.com/epipower.de/
      address:
        street: Postfach Kaiserstraße 217
        city: Karlsruhe
        postcode: '76133'
        country: Germany
        country_code: DE
    design:
      columns: '2'
---
