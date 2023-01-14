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
    id: empowerment
    content:
      title: Empowerment
      subtitle:
      text:
      items:
        - name: Wir für dich
          description: Wir sind eine Gruppe junger Menschen, die alle Epilepsie betroffen sind. Wir kümmern uns um den Ausbau von digitalen Selbsthilfeangeboten und vernetzen Menschen mit Epilepsie. Darüberhinaus arbeiten wir mit anderen Organisationen auf nationaler und internationaler zusammen, sprechen mit Vertretern der Krankenkassen, der Pharmaindustrie oder dem Gesetzgeber. Wir vertreten also deine und unsere Interessen. Wenn du mehr erfahren willst, klicke dich gerne duch unseren Blog oder folge uns bei Instagram.
          icon: users
          icon_pack: fas
        - name: Zoom Epilepsie-Meeting
          description: Jeden ersten Dienstag im Monat starten wir ein Zoom-Meeting für von Epilepsie betroffene Menschen. Nach einem Impulsvortag von Forschenden, Ärzten oder Patienten, tauschen sich die Teilnehmer zu zu allen möglichen Themen rund um die Epilepsie aus. Du hast Interesse? Dann melde dich einfach hier und du bekommst regelmäßig die Zugangsdaten per Mail.
          icon: video
          icon_pack: fas
        - name: Slack Online-Forum
          description:  Welche Sportarten machst du trotz Epilepsie? Bist du zufrieden mit deiner Therapie? Kennst du andere Menschen, die von Epilepsie betroffen sind? Wir bieten dir eine Community zum Fragen stellen, Vernetzen und zum sich gegenseitigen austauschen. Akutell haben wir hierfür ein Online-Forum auf Slack erstellt. Schreib uns einfach hier, wenn du dabei sein möchtest und wir lassen dir einen Einladungslink zukommen.
          icon: slack
          icon_pack: fab
    design:
        columns: '2'
  - block: collection
    id: blog
    content:
      title: Blog
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
      # email: info@epipower.de
      # Automatically link email and phone or display as text
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree: 
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
      contact_links:
        - icon: instagram
          icon_pack: fab
          link: https://www.instagram.com/epipower.de/
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
    design:
      columns: '2'
---
