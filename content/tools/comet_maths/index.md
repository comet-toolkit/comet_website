---
title: comet_maths

authors:
  - admin
date: 2024-03-19

---

## ❔ What is *comet_maths*?

*comet_maths* is a python module with useful mathematical algorithms (including interpolation with uncertainties) for general use as well as for use in the other tools in the CoMet toolkit.

## 📍 Where can *comet_maths* be found?

The *comet_maths* documentation is available [here](https://comet-maths.readthedocs.io/en/latest/).
You can also find Jupyter notebooks demonstrating its usage in the [example section](/user-guide/examples/).

## 📋 What can the *comet_maths* tool be used for?

*comet_maths* offers a variety of functionalities organised into three main submodules:
* Linear algebra: Primarily used for matrix operations within *obsarray* and *punpy*
* Random generators: Mainly used for sample generation in *punpy*
* Interpolation: Designed for general-purpose interpolation tasks.

## ✔️ Interpolation using *comet_maths*

The interpolation submodule focuses on two key aspects:
1. Providing realistic interpolation uncertainties, accounting for both:
   * Uncertainty on the input data points
   * Uncertainty arising from the interpolation model itself
2. Offering functionality to interpolate low-resolution data points guided by a high-resolution reference example. The high-resolution spectrum is scaled to fit the low-resolution data points, producing a sensible and physically meaningful interpolation.

For more details, refer to the [*comet_maths* documentation](https://comet_maths.readthedocs.io/en/latest/). 
