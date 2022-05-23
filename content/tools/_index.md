---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: CoMet Toolkit overview
subtitle: 
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

Datasets need to have uncertainty information associated with them to ensure their credible and reliable interpretation. However, this uncertainty information can be rather complex, with many sources of error affecting the final products. Often, multiple measurements are combined throughout the processing chain (e.g. performing temporal or spatial averages). In such cases, it is key to understand error-covariances in the data (e.g., random uncertainties do not combine in the same way as systematic uncertainties). 

Presented here is the Python CoMet Toolkit, which stands for Community Metrology toolkit, which has been developed to enable easy handling and processing of dataset error-covariance information. This toolkit aims to abstract away the complexity of dealing with uncertainties. 
There are a number of tools included in this toolkit (listed below), which are available on [github](https://github.com/comet-toolkit) and are installable via pip. More modules are planned to extend the toolkit capabilities.

The current included tools are:



