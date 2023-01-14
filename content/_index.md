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
        padding: ["20px", "0", "20px", "0"] #margin
  - block: features
    content:
      title: Empowerment
      subtitle:
      text: Digitale Selbsthilfe etc..
      items:
        - name: Zoom Epilepsie-Meeting
          description: Einmal im Monat treffen sich von Epilepsie betroffene  Menschen zum Zoom-Meeting um sich auzutauschen. Du möchtest über deine Erfahrungen mit der Krankheit sprechen oder einfach mal zuhören was andere über sich zu berichten haben? Mach mit Link
          icon: camera-web
          icon_pack: fas
        - name: Slack Online-Forum
          description: Disktuieren mit anderen über ..
          icon: slack
          icon_pack: fab
        - name: Patientenarbeit
          description: 10%
          icon: users-medical
          icon_pack: fas
    design:
        columns: '2'
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
