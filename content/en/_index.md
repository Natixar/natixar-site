---
title: 'Home'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "6rem"

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
  # - block: features
  #   id: solutions
  #   content:
  #     title: Our Technologies
  #     text: 'A modular platform to build trust across complex supply chains:'
  #     items:
  #       - name: Real-time carbon accounting
  #         icon: clock
  #         #description: 
  #       - name: Blockchain traceability & digital product passports
  #         icon: magnifying-glass 
  #       - name: Multispectral and geospatial satellite monitoring
  #         icon: globe-alt
  #       - name: AI modeling for emission reduction
  #         icon: sparkles 
  #   design:
  #     # Section background color (CSS class)
  #     css_class: "bg-green-100 dark:bg-green-900"
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
           # Upload image to `assets/media/` and reference the filename here
          image: build-website.png
          button:
            text: Learn more
            url: /blog/
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
  - block: cta-image-paragraph
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
          image: coffee.jpg
          # button:
          #   text: "Join Discord"
          #   url: https://discord.gg/z8wNYzb
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-card
    content:
      title: "We develop operational solutions tailored to each industry, need, and geography."
      text: "Natixar's approach is based on data automation, system interoperability, transparency, and regulatory foresight."
      # button:
      #   text: Get Started
      #   url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
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
