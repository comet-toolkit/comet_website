---
title: LPS training
date: 2025-06-20
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: lps
    content:
      items:
        - title: Hands-on training session at LPS
          text: "On this page you'll find links to the training material for the CoMet tutorial held at ESA's Living Planet Symposium 2025. 
            The session covers key concepts around uncertainties, error correlation and how to handle these with the CoMet toolkit.
            There will first be a presentation with some theoretical background, and an introduction to the CoMet toolkit, followed by 3 guided exercises using the CoMet toolkit. Participants will:"
          feature_icon: check
          features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
    
            - Learn how to use the CoMet tools in practical workflows.
    
            - Apply methods through interactive notebooks hosted on Google Colab.
          # Upload image to `assets/media/` and reference the filename here
          image: LPS.jpg
          caption: 'Image credit: ESA'
          button:
            text: Download Slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download
  - block: features
    id: tools
    content:
      title: Tools
      text: A list of tools which abstract away the complexity of dealing with uncertainties.
      items:
        - name: "[**Exercise 1**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)"
          icon: code-bracket
          description: "Introduction to Punpy Capabilities 
              • Get familiar with the punpy tool \n
              • Propagate uncertainties on manually provided input data through a simple measurement functions using punpy \n
              • Explore the various ways uncertainties with different error correlations can be propagated"
        - name: "[**Exercise 2**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)"
          icon: star
          description: "Multi-Dimension Datasets 
              • Store error-correlation information for multi-dimensional measurement datasets using obsarray \n
              • Practice on a multi-dimensional Earth Observation dataset example \n
              • Propagate uncertainties from these datasets through measurement functions using punpy"
        - name: "[**Exercise 3**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)"
          icon: sparkles
          description: "HYPERNETS Use Case
              • Get familiar with a sample EO data (HYPERNETS) \n
              • Use the previous exercises to add uncertainties to the HYPERNETS data processing chain \n
              • Generate and interpret uncertainty-aware outputs"
    design:
    #   # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
---