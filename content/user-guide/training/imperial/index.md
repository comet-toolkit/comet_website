---
title: Imperial training
date: 2026-03-19
type: landing

design:
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

            <br><br>

          feature_icon: check

          features:
            - "📃 **Uncertainties 101**: A short introduction to key concepts and why they matter.  
              &nbsp;&nbsp;• Why uncertainty matters  
              &nbsp;&nbsp;• What is the CoMet Toolkit  
              &nbsp;&nbsp;• How CoMet helps with uncertainty handling"
            
            - "[🔗 **Exercise 1**: Introduction to Punpy Capabilities](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise1.ipynb)  
              &nbsp;&nbsp;• Get familiar with the punpy tool  
              &nbsp;&nbsp;• Propagate uncertainties on manually provided input data  
              &nbsp;&nbsp;• Explore different error‑correlation propagation options"
            
            - "[🔗 **Exercise 2**: Multi‑Dimension Datasets](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise2.ipynb)  
              &nbsp;&nbsp;• Store error‑correlation information with obsarray  
              &nbsp;&nbsp;• Work with a multi‑dimensional EO dataset  
              &nbsp;&nbsp;• Propagate uncertainties using punpy"
            
            - "[🔗 **Exercise 3**: HYPERNETS Use Case](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/LPS_training_exercise3.ipynb)  
              &nbsp;&nbsp;• Explore a sample HYPERNETS dataset  
              &nbsp;&nbsp;• Add uncertainties into the processing chain  
              &nbsp;&nbsp;• Generate and interpret uncertainty‑aware outputs"

          image: imperial.png
          caption: "Image credit: Imperial"
          button:
            text: Download Slides
            url: Imperial_CoMet_toolkit.pdf
            icon: hero/download
---