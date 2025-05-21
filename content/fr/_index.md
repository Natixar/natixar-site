---
title: 'Accueil'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: hero
    id: top
    content:
      title: 'Chaque atome a une histoire. Nous la rendons lisible.'
      text: 'Suivez vos matières premières critiques avec une précision inégalée : blockchain, données satellites, empreintes de matériaux, analyse carbone.'
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
      # title: Our Technologies
      # text: 'A modular platform to build trust across complex supply chains:'
      items:
        - name: "🔁 Blockchain"
          #icon: clock
          #description: 
        - name: "🛰️ Surveillance par satellite"
        - name: "♻️ Décarbonation"
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: Nos technologies
          id: solutions 
          text: "Une plateforme modulaire pour instaurer la confiance dans les chaînes d'approvisionnement complexes :"
          feature_icon: check
          features:
            - Comptabilité carbone en temps réel
            - Traçabilité blockchain & passeport numérique produit
            - Surveillance satellite multispectrale et géospatiale
            - Modélisation IA pour la réduction des émissions
            - Empreintes physiques et numériques des matériaux
           # Upload image to `assets/media/` and reference the filename here
          image: technology.jpg
          button:
            text: En savoir plus
            url: /blog/
    design:
      # Section background color (CSS class)
      #css_class: "bg-gray-100 dark:bg-gray-900"
      background:
        color: "rgb(132, 164, 180)"
      spacing:
        padding: ['2rem', '0', '0', '0']
  - block: cta-image-left-paragraph
    id: applications 
    content:
      items:
        - title: "Domaines d'application"
          text: "Nos solutions sont conçues pour les chaînes critiques à haute valeur ajoutée:"
          feature_icon: check
          features:
            - "🔋 Minéraux pour batteries (lithium, cobalt, nickel…)"
            - "🪙 Métaux précieux (or, platine, argent…)"
            - "🌸 Parfumerie & produits de luxe – traçabilité et soutenabilité des ingrédients"
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
      title: "Nous développons des solutions opérationnelles adaptées à chaque secteur, besoin et géographie."
      text: "L’approche de Natixar repose sur l’automatisation des données, l’interopérabilité des systèmes, la transparence et l’anticipation réglementaire."
      # button:
      #   text: Get Started
      #   url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
