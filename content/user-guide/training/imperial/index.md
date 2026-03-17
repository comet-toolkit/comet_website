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
            
            This session covers key concepts around uncertainties, with guided exercises using the CoMet toolkit. 

            💡 You will:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
            - Learn how to use the CoMet tools in practical workflows.
            - Apply methods through interactive notebooks hosted on Google Colab.

          feature_icon: check
#          features:
#            - "**Uncertainties 101**: A short introduction to key metrological concepts and why they matter."
#            - "[**Exercise 1**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)"
#            - "[**Exercise 2**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)"
#            - "[**Exercise 3**](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)"
          features:
            - "📃 **Uncertainties 101**: A short introduction to key concepts and why they matter.  
              &nbsp;&nbsp;• Why uncertainty matters? 
              &nbsp;&nbsp;• What is the CoMet Toolkit? 
              &nbsp;&nbsp;• How CoMet helps with uncertainty handling"
            
            - "[🔗 **Exercise 1**: Introduction to Punpy Capabilities](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)  
              &nbsp;&nbsp;• Get familiar with the punpy tool 
              &nbsp;&nbsp;• Propagate uncertainties on manually provided input data through a simple measurement functions using punpy 
              &nbsp;&nbsp;• Explore the various ways uncertainties with different error correlations can be propagated"
            
            - "[🔗 **Exercise 2**: Multi-Dimension Datasets](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)  
              &nbsp;&nbsp;• Store error-correlation information for multi-dimensional measurement datasets using obsarray
              &nbsp;&nbsp;• Practice on a multi-dimensional Earth Observation dataset example
              &nbsp;&nbsp;• Propagate uncertainties from these datasets through measurement functions using punpy"
            
            - "[🔗 **Exercise 3**: HYPERNETS Use Case](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)
              &nbsp;&nbsp;• Get familiar with a sample EO data (HYPERNETS)
              &nbsp;&nbsp;• Use the previous exercises to add uncertainties to the HYPERNETS data processing chain
              &nbsp;&nbsp;• Generate and interpret uncertainty-aware outputs"

          # Upload image to `assets/media/` and reference the filename here
          image: imperial.jpg
          caption: 'Image credit: Imperial'
          button:
            text: Download Slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download
---