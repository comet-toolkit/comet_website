---
# widget: blank
# headless: true
# ... Put Your Section Options Here (title etc.) ...
title: curepy
# subtitle:
# weight: 10  # section position on page
# design:
#   # Choose how many columns the section has. Valid values: 1 or 2.
#   columns: '1'
authors:
  - admin
date: 2026-03-31

---

## ❔ What is *curepy*?


**curepy** is a Python package designed to propagate uncertainties through inverse problems. 
The name *curepy* stands for **“Comet Uncertainties for REtrievals in PYthon”**. 

Currently, only a *beta* version is available for *curepy*. Please use with caution. 


## 📍 Where can *curepy* be found?

Curepy can be installed via pip, and is available through:
- Github [here](https://github.com/comet-toolkit/curepy)
- *curepy* documentation [here](https://curepy.readthedocs.io/en/latest/)
- Example jupyter notebook in the [example section](/user-guide/examples/).

## 📋 What can *curepy* be used for?

**curepy** provides tools to solve inverse problems in which a state vector and its associated uncertainties is retrieved from measurements, optional prior information, and optionally taking into account any required ancillary parameters.

In inverse problems, uncertainties arise not only from measurement noise but also from the ill‑posedness of the retrieval. To obtain meaningful results, these uncertainties must be rigorously characterised and propagated through the inversion process. This includes handling **error-correlations** in the measurement data, as well as uncertainties introduced by priors, forward‑model assumptions, and model sensitivities. curepy quantifies how each of these factors affects the retrieved state, providing a robust framework for assessing retrieval reliability and uncertainty.

To make this process straightforward, curepy implements tools that allows users to propagate uncertainties through any measurement or forward model function written in Python, ranging from simple analytical expressions to full numerical processing chains (including external components such as radiative‑transfer models), as long as they can be wrapped in a Python function.

Uncertainty propagation through the retrieval can be performed using:

- Markov Chain Monte Carlo (MCMC)
- Optimal Estimation (OE)

Measurement values and uncertainties can be supplied manually or via an *obsarray* dataset. **curepy** also provides tools to analyse retrieval outputs, quantify uncertainties, compare results, and export them again as obsarray datasets.