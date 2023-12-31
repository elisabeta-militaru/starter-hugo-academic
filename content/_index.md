---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: 
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Social Science Researcher
          company: Cabinet Office
          company_url: ''
          company_logo:
          location: London
          date_start: '2021-05-01'
          date_end: '2021-08-01'
          description: |2-
              * Scientific Reports
              * Public Policy
        - title: Co-founder, Head of Research and Product 
          company: Advance Careers
          company_url: ''
          company_logo: 
          location: London
          date_start: '2017-03-01'
          date_end: '2021-08-01'
          description: |2-
              * Built cognitive-behavioural online games for recruitment
              * UXR
              * Data Science
      columns: '3'
  - block: markdown
    content:
      title: 
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    id: post
    content:
      title: Talks
      filters:
        folders:
          - post
    design:
      columns: '2'
      view: compact
---
