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
  # - block: people
  #   id: team
  #   content:
  #       title: team
  #       subtitle:
  #       text:
  #       user_groups:
  #         - leaderboard
  #   design:
  #     # columns: '2'
  #     # background:
  #     #   color: 'rgb(41,41,86)' #'rgb(29,35,67)'
  #     #   text_color_light: true
  #     # spacing:
  #     #   # Customize the section spacing. Order is top, right, bottom, left.
  #     #   padding: ["20px", "0", "20px", "0"] #margin
  - block: markdown
    id: blog
    content:
      title: Team
      subtitle:
      text: {{/* Initialise */}}
            {{ $page := .wcPage }}
            {{ $block := .wcBlock }}
            {{ $show_social := $block.Params.design.show_social | default false }}
            {{ $show_interests := $block.Params.design.show_interests | default true }}
            {{ $show_organizations := $block.Params.design.show_organizations | default false }}
            {{ $show_role := $block.Params.design.show_role | default true }}
            <div class="row justify-content-center people-widget">
              {{ with $block.Title }}
              <div class="col-md-12 section-heading">
                <h1>{{ . | markdownify | emojify }}</h1>
                {{ if $block.Params.subtitle }}<p>{{ $block.Params.subtitle | markdownify | emojify }}</p>{{ end }}
              </div>
              {{ end }}

              {{ with $block.Content }}
              <div class="col-md-12">
                {{ . }}
              </div>
              {{ end }}

              {{ range $block.Params.content.user_groups }}
              {{ $query := where (where site.Pages "Section" "authors") ".Params.user_groups" "intersect" (slice .) }}

              {{if $query | and (gt (len $block.Params.content.user_groups) 1) }}
              <div class="col-md-12">
                <h2 class="mb-4">{{ . | markdownify }}</h2>
              </div>
              {{end}}

              {{ range $query }}
              {{ $avatar := (.Resources.ByType "image").GetMatch "*avatar*" }}
              {{/* Get link to user's profile page. */}}
              {{ $link := "" }}
              {{ with site.GetPage (printf "/authors/%s" (path.Base .File.Dir)) }}
                {{ $link = .RelPermalink }}
              {{ end }}
                <div class="col-12 col-sm-auto people-person">
                  {{ $src := "" }}
                  {{ if site.Params.features.avatar.gravatar }}
                    {{ $src = printf "https://s.gravatar.com/avatar/%s?s=150" (md5 .Params.email) }}
                  {{ else if $avatar }}
                    {{ $avatar_image := $avatar.Fill "270x270 Center" }}
                    {{ $src = $avatar_image.RelPermalink }}
                  {{ end }}
                  {{ if $src }}
                    {{ $avatar_shape := site.Params.features.avatar.shape | default "circle" }}
                    {{with $link}}<a href="{{.}}">{{end}}<img width="270" height="270" loading="lazy" class="avatar {{if eq $avatar_shape "square"}}avatar-square{{else}}avatar-circle{{end}}" src="{{ $src }}" alt="Avatar">{{if $link}}</a>{{end}}
                  {{ end }}

                  <div class="portrait-title">
                  <h2>{{with $link}}<a href="{{.}}">{{end}}{{ .Title }}{{if $link}}</a>{{end}}</h2>
                  {{ if and $show_organizations .Params.organizations }}{{ range .Params.organizations }}<h3>{{ .name }}</h3>{{ end }}{{ end }}
                  {{ if and $show_role .Params.role }}<h3>{{ .Params.role | markdownify | emojify }}</h3>{{ end }}
                  {{ if $show_social }}{{ partial "social_links" . }}{{ end }}
                  {{ if and $show_interests .Params.interests }}<p class="people-interests">{{ delimit .Params.interests ", " | markdownify | emojify }}</p>{{ end }}
                  </div>
                </div>
                {{ end }}
                {{ end }}
              </div>
    design:
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
