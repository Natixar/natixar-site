---
#title: Contact
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

header:
  navbar:
    enable: true
    blox: "navbar"
    align: "center"
    fixed_to_top: true
    logo:
      text: ""
      # Logo filename in `assets/media/` folder
      filename: "logo_natixxar_black.png"
    button:
      enable: false
      text: "Get Started"
      url: "https://hugoblox.com/templates/"
    show_search: true
    show_theme_chooser: true
    show_translations: true
    hide_language_name: false

sections:
  - block: contact
    id: contact
    content:
      title: Contact us
      subtitle: ''
      text: ''
      # Contact details - edit or remove options as needed
      email: test@example.org
      phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      address:
        street: 450 Serra Mall
        city: Stanford
        region: CA
        postcode: '94305'
        country: United States
        country_code: US
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      office_hours:
        - 'Monday 10:00 to 13:00'
        - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
---
<!-- 
Check out my shortcode:

{{% github_rodrigoalcarazdelaosa_lottie src="https://assets5.lottiefiles.com/packages/lf20_q4nxakl0.json" width="100%" %}} -->