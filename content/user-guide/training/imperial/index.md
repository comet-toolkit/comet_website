---
title: Imperial training
date: 2026-03-16
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: lps
    content:
      items:
        - title: 🙌 Hands-on training session
          text: >
            Welcome to the CoMet tutorial held at Imperial College London!
            
            On this page you'll find links to the training materials.
            
            This session covers key concepts around uncertainties, with guided exercises using the CoMet toolkit. You will:
          feature_icon: check
          features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
    
            - Learn how to use the CoMet tools in practical workflows.
    
            - Apply methods through interactive notebooks hosted on Google Colab.
  
            - "📃 **Uncertainties 101**: A short introduction to key concepts, why they matter, and how CoMet helps with uncertainty handling"
            
          # Upload image to `assets/media/` and reference the filename here
          image: imperial.jpg
          caption: 'Image credit: Imperial'
          button:
            text: Download Slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download

  - block: features
    id: exercises
    content:
      title: Exercises
      text: Links and descriptions to the three exercises for this training session, hosted on google colab.
      items:
        - name: "[**Exercise 1**: Introduction to Punpy Capabilities     (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)"
          icon: code-bracket
          description: "• Get familiar with the punpy tool \n
    
              • Propagate uncertainties on manually provided input data through a simple measurement functions using punpy \n
    
              • Explore the various ways uncertainties with different error correlations can be propagated"
        - name: "[**Exercise 2**: Multi-Dimension Datasets      (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)"
          icon: star
          description: "• Store error-correlation information for multi-dimensional measurement datasets using obsarray \n
    
              • Practice on a multi-dimensional Earth Observation dataset example \n
    
              • Propagate uncertainties from these datasets through measurement functions using punpy \n
    
              [**solution**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2_solution.ipynb)"
        - name: "[**Exercise 3**: HYPERNETS Use Case       (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)"
          icon: sparkles
          description: "• Get familiar with a sample EO data (HYPERNETS) \n
    
              • Use the previous exercises to add uncertainties to the HYPERNETS data processing chain \n
    
              • Generate and interpret uncertainty-aware outputs \n
    
              [**solution**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3_solution.ipynb)"
    design:
    #   # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
---