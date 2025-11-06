---
title: VH-RODA Training
date: 2025-11-19
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: lps
    content:
      items:
        - title: CoMet toolkit training session at VH-RODA
          text: >
            Another CoMet toolkit hands-on training session is taking place at Very High-resolution Radar & Optical Data Assessment (VH-RODA) Workshop. 

            🗓️ Wednesday 19th November
            ⏰ 12:50-13:40
            📍 ESA-ESRIN, Frascati Italy (Room TBC)
            
            This workshop covers key concepts around uncertainties in Earth Observation (EO) data and complete guided exercises using the CoMet tools through interactive notebooks hosted on Google Colab.

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
              &nbsp;&nbsp;• Practice on a multi-dimensional EO dataset example
              &nbsp;&nbsp;• Propagate uncertainties from these datasets through measurement functions using punpy"
            
            - "[🔗 **Exercise 3**: HYPERNETS Use Case](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)
              &nbsp;&nbsp;• Get familiar with a sample EO data (HYPERNETS)
              &nbsp;&nbsp;• Use the previous exercises to add uncertainties to the HYPERNETS data processing chain
              &nbsp;&nbsp;• Generate and interpret uncertainty-aware outputs"

          # Upload image to `assets/media/` and reference the filename here
          image: VH-RODA-2025.jpg
          caption: 'Image credit: ESA'
          button:
            text: Download Slides
            url: LPS_introduction_CoMet_toolkit.pdf
            icon: hero/download
---