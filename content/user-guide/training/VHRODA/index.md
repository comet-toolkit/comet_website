---
title: VH-RODA training
date: 2025-10-01
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: vhroda
    content:
      items:
        - title: "VH-RODA hands-on training session"
          text: "On this page you'll find links to the training material for the CoMet tutorial held at ESA's VH-RODA 2025 workshop. 
            The session covers key concepts around uncertainties, error correlation and how to handle these with the CoMet toolkit.
            There will first be a presentation with some theoretical background, and an introduction to the CoMet toolkit, followed by 2 guided exercises using the CoMet toolkit. Participants will:"
          feature_icon: check
          features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
    
            - Learn how to use the CoMet tools in practical workflows.
    
            - Apply methods through interactive notebooks hosted on Google Colab.
          # Upload image to `assets/media/` and reference the filename here
          image: VHRODA.jpg
          caption: 'Image credit: ESA'
          button:
            text: Download Slides
            url: VHRODA_introduction_CoMet_toolkit.pdf
            icon: hero/download
  - block: features
    id: exercises
    content:
      title: Exercises
      text: Links and descriptions to the three exercises for this training session, hosted on google colab.
      items:
        - name: "[**Exercise 1**: Introduction to Punpy Capabilities     (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/VHRODA_training_exercise1.ipynb)"
          icon: code-bracket
          description: "• Get familiar with the punpy tool \n
    
              • Propagate uncertainties on manually provided input data through a simple measurement functions using punpy \n
    
              • Explore the various ways uncertainties with different error correlations can be propagated"
        - name: "[**Exercise 2**: Multi-Dimension Datasets      (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/VHRODA_training_exercise2.ipynb)"
          icon: star
          description: "• Store error-correlation information for multi-dimensional measurement datasets using obsarray \n
    
              • Practice on a multi-dimensional Earth Observation dataset example \n
    
              • Propagate uncertainties from these datasets through measurement functions using punpy \n
              "
    design:
    #   # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
---