---
# widget: blank
# headless: true
# ... Put Your Section Options Here (title etc.) ...
title: punpy
# subtitle:
# weight: 10  # section position on page
# design:
#   # Choose how many columns the section has. Valid values: 1 or 2.
#   columns: '1'
authors:
  - admin
date: 2024-03-19

---

## ❔ What is *punpy*?

*punpy* stands for **“Propagation of UNcertainties in Python”**. 

It's a flexible and powerful tool designed to propagate uncertainties from input quantities through any Python-based measurement function, ultimately evaluating the uncertainty on the resulting output. 

Input uncertainties can be provided manually or read directly from *obsarray*-formatted datasets using digital effects tables.


## 📍 Where can *punpy* be found?

- The *punpy* documentation is available [here](https://punpy.readthedocs.io/en/latest/), including examples for both [standalone punpy](https://punpy.readthedocs.io/en/latest/content/punpy_standalone.html) and [usage with digital effects tables](https://punpy.readthedocs.io/en/latest/content/punpy_digital_effects_table.html).
- Practical Jupyter notebooks can be found in the [example section](/user-guide/examples/).

## 📋 What can *punpy* be used for?

In any **processing chain** - also referred to as a measurement function in metrology - uncertainties on input quantities must be correctly propagated to the ouputs. This includes accounting for **error-correlation** between inputs, which can significantly affect the resulting uncertainties. Standard metrological (science of measurement) methods from the Guide to the expression of Uncertainty in Measurement (GUM) can be used to propagate the uncertainties from the input quantities to uncertainties on the measurand (the processed data). 

*punpy* makes this process straightforward by implementing two GUM-compliant methods for uncertainty propagation:

- Monte Carlo (MC) method 
- Law of Propagation of Uncertainty (LPU)

These can be applied to any Python function, whether it's:
* A simple algebraic expression
* A complex multi-step processing chain (e.g., involving complex external software such as radiative transfer simulations)

*punpy* has been validated against analytical reference cases and benchmarked with tools like the **NIST** Uncertainty Machine.


## ✔️ Using *punpy* with *obsarray*

*punpy* works both as a standalone tool, and in combination with *obsarray* digital effects tables. 

* **Standalone:** Input quantities, their uncertainties, and correlation structures must be manually specified.
* **With obsarray:** All uncertainty metadata and correlation information defined via the UNC Specification is automatically parsed by *punpy*, making propagation much simpler.

In typical workflows, random, systematic, and structured uncertainties are treated separately and propagated independently. The final result is returned as an *obsarray* dataset that includes the measurand, its uncertainties and any associsted covariance information. 

Together, *punpy* and *obsarray* provide a robust and user-friendly pipeline for propagating and handling uncertainty - without requiring users to manually deal with the underlying complexity.