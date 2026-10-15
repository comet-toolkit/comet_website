---
title: TU Wien Training
date: 2026-10-18

type: landing

design:
  spacing: "6rem"

sections:
  - block: cta-image-paragraph
    id: aria
    content:
      items:
        - title: 🎓 Hands-on Training Session
          text: |
            **📅 Date:** Monday 18th October  

            **📍 Location:** Vienna University of Technology (Austria)
            <br> 

            On this page you'll find links to the training materials.

            This session covers key concepts around uncertainties, with guided exercises using the CoMet toolkit. You will:
            <br> 
            
          feature_icon: check
          features:
            - Gain a conceptual overview of uncertainties in Earth Observation data processing.
    
            - Learn how to use the CoMet tools in practical workflows.
    
            - Apply methods through interactive notebooks hosted on Google Colab.
  
          image: tuwien.png
          caption: 'Image credit: TU Wien'
          button:
            text: Download Slides
            url: TUWien_CoMet_toolkit.pdf
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

        - name: "[(If time allows) **Exercise 4**: Uncertainty propagation for inidividual products in a timeseries](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/CoMet_temporal_combined.ipynb)"
          icon: star
          description: "• Often, products are processed one at a time, and thus uncertainties need to align with this\n

              • This exercise explores handling error correlation in such situations."

        - name: "**✅ Solutions**"
          icon: sparkles
          description: "Exercise solutions will be added after the workshop."

    design:
      css_class: "bg-gray-100 dark:bg-gray-900"
---