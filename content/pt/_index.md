---
title: 'Início'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: hero
    id: top
    content:
      title: "Cada átomo tem uma história. Nós a tornamos legível."
      text: "Acompanhe suas matérias-primas críticas com precisão sem precedentes: blockchain, dados de satélite, impressão digital de materiais, análise de carbono."
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
        - name: "🛰️ Monitoramento por satélite"
        - name: "♻️ Descarbonização"
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: 'Nossas Tecnologias'
          id: solutions 
          text: "Uma plataforma modular para construir confiança em cadeias de suprimento complexas:"
          feature_icon: check
          features:
            - Contabilidade de carbono em tempo real
            - Rastreabilidade por blockchain & passaportes digitais de produtos
            - Monitoramento satelital multiespectral e geoespacial
            - Modelagem de IA para redução de emissões
            - Impressões físicas e digitais de materiais
           # Upload image to `assets/media/` and reference the filename here
          image: technology.jpg
          button:
            text: Saiba mais
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
        - title: Áreas de Aplicação
          text: "Nossas soluções são projetadas para cadeias de suprimento de alto valor e alto risco:"
          feature_icon: check
          features:
            - "🔋 Minerais para baterias (lítio, cobalto, níquel…)"
            - "🪙 Metais preciosos (ouro, platina, prata…)"
            - "🌸 Perfumaria & produtos de luxo – rastreabilidade e sustentabilidade de ingredientes raros"
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
      title: "Desenvolvemos soluções operacionais adaptadas a cada setor, necessidade e geografia."
      text: "A abordagem da Natixar baseia-se na automação de dados, interoperabilidade de sistemas, transparência e antecipação regulatória."
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
  - block: markdown
    design:
      background:
        lottie:
          src: /media/NATIXAR.lottie
          loop: false
---
