---
title: Welcome to the CoMet Toolkit!
summary: What is the CoMet Toolkit and what can it be used for?
date: 2024-03-19

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com)'

authors:
  - RasmaOrmane
  - admin

# tags:
#   - CoMet
#   - Metrology
#   - Uncertainties
---

<!-- Welcome 👋 -->

## ❔ What is the CoMet Toolkit?

  The **Community Metrology** (CoMet) **Toolkit** is a suite of open-source software tools designed to handle, process, and store measurement data uncertainties and error-correlation information.
 
  Its key strength lies in managing the complexity of combining individual uncertainties from various sources, propagating them through any Python- based measurement function, and quantifying and storing the resulting uncertainty and error-correlation information. 
  
  The toolkit is designed to integrate seamlessly within your workflow - ensuring quality-assured results while handling much of the complexity behind the scenes. This makes it accessible and effective for both experienced users and those new to working with measurement uncertainties.  

## 💡 Why is the CoMet Toolkit relevant?

  To ensure credible and reliable data interpretation, uncertainty information must be provided alongside measurements. This uncertainty is typically made up of a multitude of sources combined throughout a processing chain, with each source influencing the final product to varying degrees.
  
  When combining measurements with uncertainties - whether through temporal or spatial averaging, integration, or model fitting - it is also essential to account for error correlation. Depending on the nature of that correlation, the resulting uncertainty can vary significantly. For example, random uncertainties may be reduced by averaging, whereas systematic uncertainties are not. 
  
  To correctly evaluate the uncertainty on the final measurand, it is necessary to consider the error correlation across all relevant dimensions.

  The CoMet Toolkit is designed to manage exactly this. It accounts for case- and source-specific characteristics of the measurement uncertainties and can handle:

- Any measurement function that can be written in Python
- Data of any dimension (float/1D/2D/3D/…)
- Multiple sources of uncertainty
- A wide range of error correlation structures
- Different probability distribution functions
- _And more_

## 📋 What can the CoMet Toolkit be used for?

With the CoMet toolkit, you can:
  
- Define measurement functions in Python
- Propagate uncertainties 
- Create and work with Digital Effects Table (DTEs)
- Automatically parse and propagate uncertainties through DTEs
- Propagate uncertainties through temporal or spatial operations (e.g., averaging, integration)
- Handle and combine both random and systemic uncertainties
- Calculate full uncertainty budgets
- _And more_

CoMet was designed to meet the requirements of the Quality Assurance framework for Earth Observation ([**QA4EO**](https://www.QA4EO.org/)).
These guidelines require that all Satellite Earth Observations (EO) and in-situ measurements are provided with their corresponding uncertainty information. 

While developed with the EO community in mind, the CoMet Toolkit is highly adaptable and can be applied to any field that requires uncertainty propagation. 

## 📍 Where can I access the CoMet Toolkit?

  The CoMet Toolkit is open-source and freely available on [**GitHub**](https://github.com/comet-toolkit). All packages can be easily installed via pip from the Python Package Index.
  **Examples** demonstrating the capabilities of this toolkit are available [**here**](https://www.comet-toolkit.org/examples/). 

## 👋 Authors & Citations

  **Developed by:** National Physical Laboratory (NPL)
  
  **Funded by:** 
  - **IDEAS-QA4EO:** Instrument Data quality Evaluation and Assessment Service - Quality Assurance for Earth Observation (IDEAS-QA4EO) contract funded by ESA-ESRIN (n. 4000128960/19/I-NS)
  - **NMS:** The UK’s Department for Business, Energy and Industrial Strategy’s (BEIS) National Measurement System (NMS) programme
  
  **Citation:** _De Vis, P. & Hunt, S. E. CoMet Toolkit. [online] National Physical Laboratory. Available at: [(https://www.comet-toolkit.org)](https://www.comet-toolkit.org)_
