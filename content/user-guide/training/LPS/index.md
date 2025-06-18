---
title: LPS training
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: CoMet
      text: Uncertainties made easy!
      primary_action:
        text: Get Started
        url: user-guide/getting-started
        icon: rocket-launch
      # secondary_action:
      #   text: Read the docs
      #   url: https://docs.hugoblox.com
      announcement:
        text: "For the latest updates"
        link:
          text: "click here"
          url: "latest-news/"
    design:
      spacing:
        padding: [300, 100, 300, 100]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: background.jpg
          filters:
            brightness: 0.5
  - block: cta-image-paragraph
    id: about
    content:
      items:
        - title: Hands-on training session at LPS
          text: On this page we will provide links to the training material for the CoMet tutorial at ESA's Living Planet Symposium. The tutorial will include:
          feature_icon: check
          features:
            - "Uncertainties 101: some basic background on uncertainties and the CoMet toolkit"
            - [Exercise 1](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)
            - [Exercise 2](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)
            - [Exercise 3](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)

          # Upload image to `assets/media/` and reference the filename here
          image: featured.jpg
          caption: 'Image credit: ESA'
          button:
            text: download slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download
---
