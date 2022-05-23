---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: punpy
subtitle:
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

*punpy* is a tool for “Propagation of UNcertainties in Python”. It propagates uncertainties on input quantities through any python function, evaluating the uncertainty on the output. These input data uncertainties can be defined using obsarray.
 

Datasets need to have uncertainty information associated with them to ensure their credible and reliable interpretation. However, this uncertainty information can be rather complex, with many sources of error affecting the final products. Often, multiple measurements are combined throughout the processing chain (e.g. performing temporal or spatial averages). In such cases, it is key to understand error-covariances in the data (e.g., random uncertainties do not combine in the same way as systematic uncertainties). 

When data is processed through a processing chain (or through a measurement function in metrological terms), the uncertainties on the input quantities need to be propagated to the ouputs (the measurand). This uncertainty propagation needs to take into account error-correlation information. Standard metrological (science of measurement) methods from the Guide to the expression of Uncertainty in Measurement (GUM) can be used to propagate the uncertainties from the input quantities to uncertainties on the measurand (the processed data). 

Punpy aims to make this simple for users. It allows users to propagate uncertainties through any given measurement function, using either the Monte Carlo (MC) method or the law of propagation of uncertainty. In this way, dataset uncertainties can be propagated through any measurement function that can be written as a python function –  including simple analytical measurement functions, as well as full numerical processing chains (which might e.g. include external radiative transfer simulations), as long as these can be wrapped inside a python function. Both methods have been validated against analytical calculations as well as other tools such as the NIST uncertainty machine.

Punpy can be used as a standalone tool, or in combination with obsarray digital effects tables. When using punpy as a standalone tool, the input quantities and their uncertainties are manually specified.
Alternatively, digital effects tables defined with obsarray can be used. punpy and obsarray have been designed to interface with each other. All the uncertainty information in the obsarray products can be automatically parsed and passed to punpy. A typical approach would be to separately propagate the random uncertainties (potentially multiple components combined), systematic uncertainties and structured uncertainties, and return them as an obsarray dataset that contains the measurand, the uncertainties and the covariance information of the measurand. By combining these tools, handling uncertainties and covariance information has become as straightforward as possible, without losing flexibility. 

The punpy documentation is available [here](https://punpy.readthedocs.io/en/latest/), including some examples for [standalone punpy](https://punpy.readthedocs.io/en/latest/content/examples_standalone.html) and for [using punpy with the digital effects tables](https://punpy.readthedocs.io/en/latest/content/examples_digital_effects_table.html).
There are also jupyter notebooks available from [here](/examples).
