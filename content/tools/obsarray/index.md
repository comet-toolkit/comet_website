---
# ... Put Your Section Options Here (title etc.) ...
title: obsarray
# subtitle:
# weight: 10  # section position on page
# design:
#   # Choose how many columns the section has. Valid values: 1 or 2.
#   columns: '1'

authors:
  - SamHunt

date: 2024-03-19
---

## ❔ What is *obsarray*?

*obsarray* is an extension to xarray that enables:

- Defining,
- Storing, and
- Interfacing 

with uncertainty and measurement error-covariance information in NetCDF files, using standardised metadata. 

Datasets created using *obsarray* include this standardised uncertainty and error-covariance information in so-called **'digital effects tables'**.

## 📍 Where can *obsarray* be found?

- The *obsarray* documentation is available [here](https://obsarray.readthedocs.io/en/latest/).
- Jupyter notebooks demonstrating its usage can be found in the [examples section](/user-guide/examples/).

## 📋 What can the *obsarray* tool be used for?

Based on methods defined by the CoMet [UNC Specification](https://comet-toolkit.github.io) - which establishes uncertainty metadata naming conventions - *obsarray* allows users to parameterise error-covariance information by storing it as attributes attached to uncertainty variables - creating so-called 'digital effects tables'. 

A key goal of the CoMet Toolkit is to abstract away the complexity of managing error covariances. When measurement datasets are structured using *obsarray*, users can:

* Read and write datasets while preserving error-correlation information.
* Propagate dataset uncertainties via *punpy* - which can directly use the 'digital effects tables' - so users rarely need to handle these complexities manually.
