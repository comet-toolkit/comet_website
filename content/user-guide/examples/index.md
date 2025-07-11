---
title: Examples
summary: How to utilise the various tools within the CoMet Toolkit?
date: 2024-03-19

authors:
  - admin
  - RasmaOrmane
tags:
  - CoMet
  - punpy
  - comet_maths
  - obsarray

image:
    caption: 'Image credit: [**Unsplash**](https://unsplash.com)'
---

Below is a collection of example use cases, each with an accompanying Jupyter notebook featuring detailed commentary. All CoMet tools can be used individually or together, depending on your needs. For additional information on  individual packages, refer to the linked documentation and resources throughout the site.

## 📦 Punpy as a Standalone Package

### 🗸 General use cases

An example showcasing the capabilitites of the [punpy](/tools/punpy) package can be found [here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/punpy_standalone_example_overview.ipynb).

This Jupyter notebook covers the following concepts:

  1. **Calibration** of L0 data to L1
  2. Propagation of various types of uncertainties:
    - **uncorrelated** (random) uncertainties
    - **fully correlated** (systematic) uncertainties
    - uncertainties associated with **structured errors**
  3. **Correlation** along one, two, or more dimensions of a variable
  4. **Multidimensional** input quantities, where a certain correlation structure is known along one dimension, while the other dimensions are random or systematic.

### 🗸 Punpy vs. NIST

We also have compiled a set of **validation examples** [here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/NIST_example.ipynb), where results from [punpy]({{< relref "/tools/punpy" >}}) are compared against the well-established **NIST Uncertainty Machine**.

The following **examples** from the NIST Uncertainty Machine [user manual](https://uncertainty.nist.gov/NISTUncertaintyMachine-UserManual.pdf) have been replicated: 

  1. End-gauge calibration
  2. Dynamic viscosity
  3. Resistance
  4. Stefan-Boltzmann constant
  5. Voltage reflection coefficient

❕ The results obtained using *punpy* are in full agreement with those from the NIST Uncertainty Machine.

## 📋 Digital Effects Tables (DET)

### 🗸 Defining DET

A Jupyter notebook with examples on defining **digital effects tables** is available [here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/defining_digital_effects_table.ipynb). 

It demonstrates how to:

  - Use [obsarray](/tools/obsarray) as a templater for efficiently creating ***xarray* datasets**, with and without uncertainty information.
  - Use [obsarray's](/tools/obsarray) **special variable types** (e.g., uncertainties and flags), to build datasets that include structured uncertainty and error-covariance information. 
  - Constructing a digital effects table for a physical system involving gas temperature, pressure, and amount of substance - where uncertainties be efficiently and easily propagated through a **measurement function** using [*punpy*](/tools/punpy). [Try the full example here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/master/training/punpy_digital_effects_table_example.ipynb).

### 🗸 Using *obsarray* & *punpy* Together

1. Example: [*obsarray* in practice]((https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/obsarray_example.ipynb))

2. Example: [Propagating DETs with *punpy*](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/defining_digital_effects_table.ipynb).

This example shows how digital effects tables created with obsarray can be directly used in punpy to propagate uncertainties through a measurement function.

This notebook outlines how digital effects tables that are created with [obsarray](/tools/obsarray), can be propagated through a measurement function using [punpy](/tools/punpy). 

Specifically, this example includes:

- Calculating the uncertainty on the gas volume using the ideal gas law.
- Quantifying the uncertainties and error correlations of the gas temperature, pressure, and substance amount.

## ☄️ *comet_maths* Interpolation 

### 🗸 How to interpolate data with uncertainties?

A Jupyter notebook demonstrating **interpolation with uncertainties** is available [here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/interpolation_example.ipynb).

This example walks through:

  - **Interpolation** methods:
    1. Linear
    2. Quadratic
    3. Cubic
  - **Known** measurment uncertainties
  - **Unknown** input/model uncertainties
  - **Uncertainty propagation** using the Monte Carlo approach
  - **Extrapolation** of values
  - **1D interpolation** along a high-resolution reference

## 🗂️ Project specific examples

In this section, we have compiled a selection of external projects and examples that have made use of the CoMet Toolkit. 

### 🗸 **HYPERNETS example** 

- 🛰️ LANDHYPERNET flags and uncertainty propagation (through band integration over Sentinel-2 MSI SRF) is available [here](https://colab.research.google.com/github/comet-toolkit/comet_training/blob/main/hypernets_surface_reflectance.ipynb).
