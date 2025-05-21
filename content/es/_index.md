---
title: 'Inicio'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: hero
    id: top
    content:
      title: Cada átomo tiene una historia. Nosotros la hacemos legible.
      text: 'Rastree sus materias primas críticas con una precisión sin precedentes: blockchain, datos satelitales, huellas de materiales, análisis de carbono.'
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
  - block: features
    content:
      # title: 
      # text: 
      items:
        - name: "🔁 Blockchain"
          #icon: clock
          #description: 
        - name: "🛰️ Monitoreo satelital"
        - name: "♻️ Descarbonización"
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: Nuestras Tecnologías
          id: solutions 
          text: 'Una plataforma modular para generar confianza en cadenas de suministro complejas:'
          feature_icon: check
          features:
            - Contabilidad de carbono en tiempo real
            - Trazabilidad por blockchain & pasaportes digitales de productos
            - Monitoreo satelital multiespectral y geoespacial
            - Modelado de IA para reducción de emisiones
            - Huellas físicas y digitales de materiales
           # Upload image to `assets/media/` and reference the filename here
          image: technology.jpg
          button:
            text: Saber más
            url: /blog/
    design:
      # Section background color (CSS class)
      #css_class: "bg-gray-100 dark:bg-gray-900"
      background:
        color: "rgb(132, 164, 180)"
      spacing:
        padding: ['6rem', '0', '0px', '0']
  - block: cta-image-left-paragraph
    id: applications 
    content:
      items:
        - title: Ámbitos de Aplicación
          text: "Nuestras soluciones están diseñadas para cadenas de suministro de alto valor y alto riesgo:"
          feature_icon: check
          features:
            - "🔋 Minerales para baterías (litio, cobalto, níquel…)"
            - "🪙 Metales preciosos (oro, platino, plata…)"
            - "🌸 Perfumería & productos de lujo – trazabilidad y sostenibilidad de ingredientes raros"
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
  - block: cta-card
    id: vision 
    content:
      title: "Desarrollamos soluciones operativas adaptadas a cada sector, necesidad y geografía."
      text: "El enfoque de Natixar se basa en la automatización de datos, interoperabilidad de sistemas, transparencia y previsión regulatoria."
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
