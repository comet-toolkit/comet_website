---
title: Getting started with CoMet
date: 2024-03-21

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com)'

authors:
  - RasmaOrmane
  - admin

tags:
  - CoMet
  - Metrology
  - Uncertainties
  - comet_maths
  - obsarray
  - punpy
---

Welcome 👋

This brief guide walks you through the key prerequisites and steps to get started with CoMet. 

## 1.💡 Get familiar with the toolkit and its capabilities

To understand what the CoMet Toolkit offers, we recommend starting with the [**About Section**]({{< relref "/about" >}}), which outlines the aims and functionality in detail. 

But, in a nutshell, 

  > CoMet stands for **Community Metrology Toolkit**. It is a suite of open-source software tools designed to handle, process, and store measurement data uncertainties and error-correlation information.

The toolkit accounts for case- and source-specific characteristics of measurements, and can be used to:
    * Quantify measurement uncertainties and uncertainty budget
    * Generate digital effects tables
    * Validate measurements

Currently, CoMet consists of three core tools:

    1. obsarray
    2. punpy
    3. comet_maths

Additional modules are in development and will be added over time. For more details on the individual tools, refer to the [**Tools Section**]({{< relref "/#tools" >}}). 

## 2. 🗃️ Characterise the data/measurements that require the uncertainty propagation

The core purpose of the CoMet Toolkit is to propagate uncertainties. To do this effectively, it's essential to have a clear understanding of the type of data/measurements you're working with. 

For a general framework for determining an uncertainty budget, we refer to the Five-step QA4EO approach. See [this page](/user-guide/theory/QA4EO) in our theory section, or refer directly to the [QA4EO process document](https://qa4eo.org/docs/3_Process_Document.pdf).

To help you identify all the relevant information within your dataset, we have compiled a set of guiding questions and practical tips:

### 🗸 General 

  - ❔ What kind of data are you working with?
  - ❔ Does it require any pre-processing or filtering?
  - ❔ How many data points do you have? Is it memory-intensive?

### 🗸 Quantifying uncertainties on input quantities

  - ❔ Can you list all the input quantities involvements in your measurements?
  - ❔ Can you identify all the potential error sources?
  - Errors generally fall into three categories, each with distinct characteristics: 
    1. Random
    2. Systematic
    3. Structured

  ❕ Typically, each input quantity will be affected by **one or more** error effects!

### 🗸 Defining measurement function

  - ❔ What is the analytic expression (i.e. measurement function) that relates your input quantities to your measurand? 
  - ❔ Are you using a more complex processing chain involving external software?
  - ❔ Can your measurement function be written in Python, with your input quantities as arguments, and the measurand as the output? 

  Learn more about defining and using **measurement functions** in our guide on [**propagating uncertainties through a measurement function**](/user-guide/theory/processing-chains/).  

### 🗸 Determining error correlation

Once the error sources have been identified, it's important to consider how these errors correlate across your data.

As described in FIDUCEO's article on ["The origin of error correlation"](https://research.reading.ac.uk/fiduceo/archive/tutorials/the-origin-of-error-correlation/),

  > Correlation is a statistical measure of how two, or more, variables vary together.

To learn more about how error correlation applies to Earth observation data - and how it can be represented - see our page on [error correlation and how to store it](/user-guide/theory/error_correlation).

## 3. 🧾 Identify similarities between your use case and the available examples.

Before diving into implementation, it may be helpful to explore how others have used the toolkit - and how their approaches might apply to your work.

  - Browse through the available [examples]({{< relref "/user-guide/examples" >}}) and documentation. 
  - Consider how the CoMet tools can be applied to your own case study.
  - ❔ Which tools will you need to use - and in what order? 

## 4. 🖥️ Install the tools

All CoMet Toolkit components are open-source and available on [GitHub](https://github.com/comet-toolkit). They can be easily installed via pip:

    - pip install comet_maths
    - pip install punpy
    - pip install obsarray

  _Installing **punpy** will automatically install both comet-maths and obsarray as dependencies._


## 5. ✔️ Perform uncertainty estimation and interpret the results

With your measurement function defined, and all relevant packages and data installed/prepared, you're now ready to harness the full power of the CoMet Toolkit! 

### 🗸 What Can You Do?

Here's an overview of the key capabilities and methods available in CoMet: 

  - store uncertainty and error correlation information
    1. machine readable digital effects tables
    2. UNC specification
  - Propagate uncertainties
    1. 🎲 Monte Carlo (MC)
    2. ⚖️ Law of Propagation of Uncertainty (LPU)
  - Interpolate data & uncertainties
    1. Linear
    2. Quadratic
    3. Cubic 
    4. Gaussian Process Regression (GPR)
    5. Extrapolation

_Many of these methods can be used in combination across different workflows. For detailed examples, refer to the [examples section]({{< relref "/user-guide/examples" >}})._

## 6. 📈 Advanced use

This section outlines tips and guidance for users working with large datasets or performance-critical applications. 

### 🗸 Managing memory and runtime

  Certain datasets - especially those with multiple dimensions, or requiring Monte Carlo propagation - can have substantial RAM and CPU requirements. 
    
  Key tips:
  * Storing full error correlation matrices across all dimensions can be prohibitively memory-intensive.
  * Instead, consider splitting the correlation structures by dimension (e.g. time, wavelength, spatial axes).
  * CoMet supports the use of error correlation dictionaries, which help manage large correlation structures more efficiently during propagation.

  For practical guidance, see the [punpy memory and performance documentation](https://punpy.readthedocs.io/en/latest/content/punpy_memory_and_speed.html). 

  An Example:
  The **HYPERNETS L2A** surface reflectance product includes both a wavelength and time-series dimension. Uncertainty handling for this dataset can be optimised by storing error correlation separately for each dimension, and propagating using correlation dictionaries.
  See the final section of [this jupyter notebook example](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/hypernets_surface_reflectance.ipynb) for implementation details.


