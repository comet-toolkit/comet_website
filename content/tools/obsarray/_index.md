---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: Obsarray
subtitle:
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

obsarray, provides an extension to the widely used xarray package to interface with measurement error-covariance information encoded in datasets. Although storage of full error-covariance matrices for large observation datasets is not practical, they are often structured to an extent that allows for simple parameterisation. obsarray makes use of a parameterisation method for error-covariance information, first developed in the FIDUCEO project, stored as attributes to uncertainty variables. In this way the datasets can be written/read in a way that this information is preserved.
