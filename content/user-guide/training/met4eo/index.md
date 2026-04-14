---
title: ARIA 2026 Workshop
date: 2026-05-01

type: landing

design:
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: aria
    content:
      items:
        - title: 🎓 CoMet Training Workshop – Met4EO workshop 2026
          text: |
            **📅 Start:** Thursday 21st May  

            **🕰️ End:** Friday 22nd May 

            **📍 Location:** National Physical Laboratory   
            <br> 

            On this page you'll find links to the training materials.

            This session covers key concepts around uncertainties, with guided exercises using the CoMet toolkit. You will:
            <br> 
            
          feature_icon: check
          features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
    
            - Learn how to use the CoMet tools in practical workflows.
    
            - Apply methods through interactive notebooks hosted on Google Colab.
  
            - "📃 **Uncertainties 101**: A short introduction to key concepts, why they matter, and how CoMet helps with uncertainty handling."

          image: Met4EOtraining.png
          caption: 'Image credit: Met4EO'
          button:
            text: Download Slides
            url: Met4EO_CoMet_toolkit.pdf
            icon: hero/download


  - block: features
    id: exercises
    content:
      title: Exercises
      text: Links and descriptions of the hands‑on exercises for this training session.
      items:
        - name: "[**Exercise 1**: Uncertainty Propagation Basics (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_no_errcorr.ipynb)"
          icon: code-bracket
          description: "• Simple measurement functions \n

              • Manual specification of input uncertainties \n

              • MC and LPU uncertainty propagation methods"

        - name: "[**Exercise 2**: Error Correlation in EO Datasets (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_with_errcorr.ipynb)"
          icon: star
          description: "• Simple measurement functions \n

              • Propagating error correlation information  \n

              • Random and systematic uncertainties"

        - name: "[**Exercise 3**: From Spectrometer Measurements to NDVI (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_exercise_spectrometer.ipynb)"
          icon: sparkles
          description: "• Spectrometer example from demo and uncertainty tree diagram session \n

              • Propagate uncertainties from raw data, to reflectance and NDVI \n

              • Random and systematic uncertainties"

        - name: "[**Exercise 4**: Multi-Dimension Datasets (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/CoMet_Training_Exercise4.ipynb)"
          icon: code-bracket
          description: "• Use obsarray to store error-correlation information for multi-dimensional measurement datasets - such as from Earth Observation.\n

              • Propagate uncertainties from these datasets through measurement functions using punpy."

        - name: "[(optional if time allows) **Exercise 5**: Work on your own use case or HYPERNETS (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/CoMet_HYPERNETS_exercise.ipynb)"
          icon: star
          description: "• Get familiar with a sample EO data (HYPERNETS) \n
    
              • Use the previous exercises to add uncertainties to the HYPERNETS data processing chain \n
    
              • Generate and interpret uncertainty-aware outputs \n"

        - name: "**✅ Solutions**"
          icon: sparkles
          description: "Exercise solutions will be added after the workshop."

    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
---