---
title: '首页'
date: 2025-05-20
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: hero
    id: top
    content:
      title: 每个原子都有一个故事。我们让它变得清晰可见。
      text: '以前所未有的精度追踪您的关键原材料：区块链、卫星数据、材料指纹、碳分析。'
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
        - name: "🔁 区块链"
          #icon: clock
          #description: 
        - name: "🛰️ 卫星监测"
        - name: "♻️ 脱碳"
    design:
      # Section background color (CSS class)
      css_class: "bg-green-100 dark:bg-green-900"
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: 我们的技术
          id: solutions 
          text: '一个模块化平台，建立复杂供应链中的信任：'
          feature_icon: check
          features:
            - 实时碳核算
            - 区块链追踪 & 数字产品护照
            - 多光谱和地理空间卫星监测
            - 用于减排的人工智能建模
            - 材料的物理和数字指纹
           # Upload image to `assets/media/` and reference the filename here
          image: technology.jpg
          button:
            text: 了解更多
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
        - title: 应用领域
          text: "我们的解决方案专为高价值、高风险的供应链设计："
          feature_icon: check
          features:
            - "🔋 电池矿物（锂、钴、镍…）"
            - "🪙 贵金属（黄金、铂金、银…）"
            - "🌸 香水和奢侈品 – 稀有成分的可追溯性和可持续性"
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
      title: "我们开发适用于各行业、需求和地理位置的运营解决方案。"
      text: "Natixar 的方法基于数据自动化、系统互操作性、透明性和法规前瞻性。"
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
