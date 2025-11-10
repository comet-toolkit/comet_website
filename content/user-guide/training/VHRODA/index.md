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
        - title: CoMet toolkit training session at VH-RODA
          text: "Another CoMet toolkit hands-on training session is taking place at Very High-resolution Radar & Optical Data Assessment (VH-RODA) Workshop. \n
            \n
            🗓️ Wednesday 19th November \n
            ⏰ 12:50-13:40 \n
            📍 ESA-ESRIN, Frascati Italy (Room TBC) \n
            \n
            This workshop covers key concepts around uncertainties in Earth Observation (EO) data and complete guided exercises using the CoMet tools through interactive notebooks hosted on Google Colab."
            
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
      text: Links and descriptions to the two exercises for this training session, hosted on google colab.
      items:
        - name: "[**Exercise 1**: Introduction to Punpy Capabilities     (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/VH-RODA_training_exercise1.ipynb)"
          icon: code-bracket
          description: "• Get familiar with the punpy tool \n
    
              • Propagate uncertainties on manually provided input data through a simple measurement functions using punpy \n
    
              • Explore the various ways uncertainties with different error correlations can be propagated"
        - name: "[**Exercise 2**: Multi-Dimension Datasets      (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/VH-RODA_training_exercise2.ipynb)"
          icon: star
          description: "• Store error-correlation information for multi-dimensional measurement datasets using obsarray \n
    
              • Practice on a multi-dimensional Earth Observation dataset example \n
    
              • Propagate uncertainties from these datasets through measurement functions using punpy \n
              "
      
---