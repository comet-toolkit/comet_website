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
            The session covers key concepts around uncertainties, with guided exercises using the CoMet toolkit. Participants will:"
            feature_icon: check
            features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.\n
    
            - Learn how to use the CoMet tools in practical workflows.\n
    
            - Apply methods through interactive notebooks hosted on Google Colab.\n"
          # Upload image to `assets/media/` and reference the filename here
          image: LPS.jpg
          caption: 'Image credit: ESA'
          button:
            text: Download Slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download
    
  - block: features
    id: exercises
    content:
      title: Exercises
      text: Links to each of the exercises, with a short description what they are about.
      items:
        - "[🔗 **Exercise 1**: Introduction to Punpy Capabilities](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb) \n

          • Get familiar with the punpy tool \n

          • Propagate uncertainties on manually provided input data through a simple measurement functions using punpy \n

          • Explore the various ways uncertainties with different error correlations can be propagated" 
        
        - "[🔗 **Exercise 2**: Multi-Dimension Datasets](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)

          • Store error-correlation information for multi-dimensional measurement datasets using obsarray \n

          • Practice on a multi-dimensional Earth Observation dataset example \n

          • Propagate uncertainties from these datasets through measurement functions using punpy" 
        
        - "[🔗 **Exercise 3**: HYPERNETS Use Case](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb) \n

          • Get familiar with a sample EO data (HYPERNETS) \n

          • Use the previous exercises to add uncertainties to the HYPERNETS data processing chain \n

          • Generate and interpret uncertainty-aware outputs" 

          

[comment]: <> (- 📃 **Uncertainties 101**: A short introduction to key concepts and why they matter. \n )
          
[comment]: <> (          • Why uncertainty matters? \n)

[comment]: <> (          • What is the CoMet Toolkit? \n)

[comment]: <> (          • How CoMet helps with uncertainty handling)
---