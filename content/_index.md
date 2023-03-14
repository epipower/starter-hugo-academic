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
        - name: Zoom Epilepsie-Meeting
          description: <div align="justify"> Jeden ersten Dienstag im Monat starten wir ein Zoom-Meeting für Menschen, die von Epilepsie betroffen sind. Nach einem Impulsvortag über etwas Aktuelles aus der Epilepsie tauschen sich die Teilnehmer anschließend zu verschiedenen Themen aus, spezifisch zur Epilepsie aber auch Privates. Es geht also ganz locker zu. Du hast Interesse? Dann melde dich einfach <a href="mailto:info@epipower.de">hier</a> und du bekommst regelmäßig die Zugangsdaten per Mail.</div>
          icon: video
          icon_pack: fas
        - name: Slack Online-Forum
          description: <div align="justify"> Wie bewältigst du den Alltag mit deiner Epilepsie? Bist du zufrieden mit deiner Therapie? Kennst du andere Menschen, die von Epilepsie betroffen sind? Wir bieten dir eine Community zum Fragen stellen, Vernetzen und zum sich gegenseitig Austauschen. Akutell haben wir hierfür ein Online-Forum auf Slack erstellt. Melde dich einfach <a href="mailto:info@epipower.de">hier</a>, wenn du dabei sein möchtest und wir lassen dir zeitnah einen Einladungslink zukommen. </div>
          icon: slack
          icon_pack: fab
    design:
        columns: '2'
  - block: collection
    id: blog
    content:
      title: Blog
      subtitle: Weitere Artikel im [Archiv](/post)
      text:
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
      contact_links:
        - icon: instagram
          icon_pack: fab
          name: epipower.de
          link: https://www.instagram.com/epipower.de/
        - icon: linkedin
          icon_pack: fab
          name: Epilepsie Empowerment Deutschland e.V.
          link: https://www.linkedin.com/company/epilepsie-empowerment-deutschland-e-v/
    design:
      columns: '2'
---
