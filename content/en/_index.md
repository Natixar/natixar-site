---
title: 'Home'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: hero
    id: top
    content:
      title: Every atom has a story. We make it legible.
      text: 'Track your critical raw materials with unprecedented precision: blockchain, satellite data, material fingerprinting, carbon analysis.'
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: bg-triangles.svg
          filters:
            brightness: 0.5
        lottie:
          src: /media/atom.lottie
  - block: features
    content:
      # title: 
      # text: 
      items:
        - name: "🔁 Blockchain"
          #icon: clock
          #description: 
        - name: "🛰️ Satellite monitoring"
        - name: "♻️ Decarbonization"
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: Our Technologies
          id: solutions 
          text: 'A modular platform to build trust across complex supply chains:'
          feature_icon: check
          features:
            - Real-time carbon accounting
            - Blockchain traceability & digital product passports
            - Multispectral and geospatial satellite monitoring
            - AI modeling for emission reduction
            - Physical & digital material fingerprinting
           # Upload image to `assets/media/` and reference the filename here
          image: technology.jpg
          button:
            # Text the is too short and vague decreases SEO mark - avoid "Learn more"
            text: Learn more on our blog
            url: /blog/
            
    design:
      # Section background color (CSS class)
      #css_class: "bg-gray-100 dark:bg-gray-900"
      background:
        color: "rgb(132, 164, 180)"
      spacing:
        padding: ['2rem', '0', '0px', '0']
  - block: cta-image-left-paragraph
    id: applications 
    content:
      items:
        - title: Application Areas
          text: "Our solutions are designed for high-value, high-risk supply chains:"
          feature_icon: check
          features:
            - "🔋 Battery minerals (lithium, cobalt, nickel…)"
            - "🪙 Precious metals (gold, platinum, silver…)"
            - "🌸 Perfumery & luxury products – traceability and sustainability of rare ingredients"
          # Upload image to `assets/media/` and reference the filename here
          image: luxury.png
          # button:
          #   text: "Join Discord"
          #   url: https://discord.gg/z8wNYzb
    design:
      # Section background color (CSS class)
      #css_class: "bg-green-100 dark:bg-green-900"
      # background:
      #   color: "rgb(176, 218, 209)"
      spacing:
        padding: ['0px', '0', '0px', '0']
  - block: hero
    id: vision 
    content:
      title: "We develop operational solutions tailored to each industry, need, and geography."
      text: "Natixar's approach is based on data automation, system interoperability, transparency, and regulatory foresight."
      # button:
      #   text: Get Started
      #   url: https://hugoblox.com/templates/
    design:
      css_style: "color: #ff0000;"
      background:
        color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: bg-triangles.svg
          filters:
            brightness: 0.7
      # card:
      #   # Card background color (CSS class)
      #   css_class: "bg-primary-700"
      #   css_style: ""
  - block: markdown
    design:
      background:
        lottie:
          src: /media/NATIXAR.lottie
          loop: false
  # - block: testimonials
  #   id: about
  #   content:
  #     title: ""
  #     text: ""
  #     items:
  #       - name: "Hugo Smith"
  #         role: "Marketing Executive at X"
  #         # Upload image to `assets/media/` and reference the filename here
  #         image: "testimonial-1.jpg"
  #         text: "Awesome, so easy to use and saved me so much work with the swappable pre-designed sections!"
  #   design:
  #     spacing:
  #       # Reduce bottom spacing so the testimonial appears vertically centered between sections
  #       padding: ["6rem", 0, 0, 0]
---
