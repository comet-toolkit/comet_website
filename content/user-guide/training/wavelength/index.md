---
title: Wavelength 2026 Workshop
date: 2026-04-07

type: landing

design:
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: wavelength
    content:
      items:
        - title: 🎓 CoMet Training Workshop – Wavelength Conference 2026
          text: |
            **📅 Date:** Thursday 9th April  

            **🕰️ Time:** 15:00–16:10  

            **📍 Location:** National Physical Laboratory (Bushy House)  
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

          image: wavelength.png
          caption: 'Image credit: Wavelength Conference'
          button:
            text: Download Slides
            url: wavelength2026_CoMet_toolkit.pdf
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

        - name: "**✅ Solutions**"
          icon: sparkles
          description: "• [**Exercise 1**(Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_with_errcorr_solution.ipynb) \n

              • [**Exercise 2** (Click here to open exercise)](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_with_errcorr_solution.ipynb)"

    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
---