---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: comet_maths
subtitle:
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

*comet_maths* is a python module with useful mathematical algorithms (including interpolation with uncertainties) for general use as well as for use in the other tools in the CoMet toolkit.
The *comet_maths* documentation is available [here](https://comet_maths.readthedocs.io/en/latest/).
There are also jupyter notebooks available in the [example section](/examples).

There are quite a range of different functionalities within *comet_maths*. There are currently three submodules. One for linear algebra (mainly used for matrix operations in both *obsarray* and *punpy*), one for random generators (mainly used for sample generation in *punpy*) and one for interpolation (for general use).

The interpolation submodules focuses on two aspects. First, it aims to provide interpolation uncertainties that are as realistic as possible, and include both a contribution from the uncertainty on the input data point, as well as a contribution from the uncertainty in the model used for interpolation. Second, the interpolation module has functionality to interpolate between some low-resolution data points following a high resolution example. The example spectrum gets scaled in order to go through the low-resolution data points to form a sensible interpolation. For more info, see the [comet_maths documentation](https://comet_maths.readthedocs.io/en/latest/). 
