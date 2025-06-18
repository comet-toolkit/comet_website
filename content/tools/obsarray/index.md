---
# ... Put Your Section Options Here (title etc.) ...
title: obsarray
# subtitle:
# weight: 10  # section position on page
# design:
#   # Choose how many columns the section has. Valid values: 1 or 2.
#   columns: '1'

authors:
  - admin
date: 2024-03-19
---

## ❔ What is *obsarray*?

*obsarray* is an extension to xarray for

- defining
- storing
- interfacing 

with uncertainty and measurement error-covariance information in NetCDF files using standardised metadata. 

These datasets that include standardised uncertainty and error-covariance information in so-called **'digital effects tables'**.

## 📍 Where can *obsarray* be found?

- The *obsarray* documentation is available [here](https://obsarray.readthedocs.io/en/latest/).
- There are also jupyter notebooks available in the [example section](user-guide/examples/).

## 📋 What can *obsarray* tool be used for?

Using methods defined by the CoMet [UNC Specification](https://comet-toolkit.github.io) (uncertainty metadata naming conventions), *obsarray* enables users to parameterise their error-covariance information by storing it as attributes to uncertainty variables - creating 'digital effects tables'. 

One important aim of the CoMet Toolkit is to abstract away the complexity of dealing with error-covariances. Using measurement datasets defined in this way using *obsarray*, you can for example:

* read/write datasets in a way that error-correlation information is preserved.
* propagate dataset uncertainty using *punpy* -- which can directly use the 'digital effects tables', so that users typically never have to interact with it.
