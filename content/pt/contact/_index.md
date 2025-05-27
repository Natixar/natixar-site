---
title: Contact
date: 2025-05-20
type: landing

# Natixar's address in France
address_locale: fr-fr

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: contact
    id: contact
    content:
      title: Contact us
      subtitle: ''
      text: 'natixar'
      image: 
        filename: carte_marseille.png
        caption: map of Marseilles
      # Contact details - edit or remove options as needed
      email: info@natixar.com
      # phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      address:
        street: 31 rue Raphael
        city: Marseille
        region: 
        postcode: '13008'
        country: France
        country_code: FR
      # directions: 
      office_hours:
        - 'Mon. - Fri. 08:00 to 20:00 CET'
        - 'Saturday 09:00 to 21:00 CET'
        - 'Closed on Sundays'
      # contact_links:
      #   - icon: twitter
      #     icon_pack: fab
      #     name: DM Me
      #     link: 'https://twitter.com/Twitter'
      #   - icon: skype
      #     icon_pack: fab
      #     name: Skype Me
      #     link: 'skype:echo123?call'
      #   - icon: video
      #     icon_pack: fas
      #     name: Zoom Me
      #     link: 'https://zoom.com'
      # Automatically link email and phone or display them just as text?
      autolink: true
      # Choose an email form provider (netlify/formspree)
      form:
        provider: netlify
        formspree:
          # If using Formspree, enter your Formspree form ID
          id: ''
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: true
          # TODO Too fast! Must add a Thank you! page.
          success_url: '/#top'
      # Coordinates to display a map - set your map provider in `params.yaml`
      coordinates:
        latitude: '37.4275'
        longitude: '-122.1697'
    design:
      # Choose how many columns the section has. Valid values: '1'.
      columns: '1'
      # Choose if you want padding around the customized message
      no_padding: true
      # Background
      background:
        color: #2020A040
        # image:
        #   # Add your image background to `assets/media/`.
        #   filename: bg-triangles.svg
        #   filters:
        #     brightness: 0.2
        #     transparency: 0.5
---
Check out my shortcode:

{{% github_rodrigoalcarazdelaosa_lottie src="https://assets5.lottiefiles.com/packages/lf20_q4nxakl0.json" width="100%" %}}