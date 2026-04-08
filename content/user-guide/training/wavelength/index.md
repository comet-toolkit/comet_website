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
          text: >
            **📅 Date:** Thursday 9th April  
            **🕰️ Time:** 15:00–16:10  
            **📍 Location:** National Physical Laboratory (Bushy House)  

            This hands‑on workshop introduces **uncertainty handling in Earth Observation**
            using the **CoMet toolkit**.

            The session combines short presentations with guided, practical exercises
            using Google Colab notebooks.

            🔎 **Session outline:**

            - Metrology fundamentals for Earth Observation  

            - Uncertainty propagation with CoMet  

            - Guided hands‑on exercises using Google Colab

          feature_icon: check
          features:
            - Gain an understanding of why uncertainty matters in Earth Observation workflows.

            - Learn core concepts of uncertainty propagation using the CoMet toolkit.

            - Explore practical examples using Punpy and Obsarray in Google Colab.

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

              • propagating error correlation information  \n

              • random and systematic uncertainties"

        - name: "**✅ Solutions**"
          icon: sparkles
          description: "Exercise solutions will be added after the workshop."

    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
---