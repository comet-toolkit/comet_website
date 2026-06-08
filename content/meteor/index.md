---
title: MetEOR Toolkit
summary: An open-source Python ecosystem for EO comparison and uncertainty-aware calibration and validation workflows.
date: 2025-11-01

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:

authors:
  - admin
---

## MetEOR Toolkit

## ❔ What is MetEOR?
The MetEOR Toolkit (Metrology for Earth Observation and Radiometry) is an open-source Python toolkit for the comparison of satellite and reference measurements. The development of the MetEOR toolkit was funded through a number of different project, most notably the ESA [**Met4EO**](https://www.QA4EO.org/met4eo) project.

It supports scalable, reproducible, and uncertainty-aware Earth Observation (EO) calibration and validation workflows, helping users work consistently across large and diverse EO data archives.

### Availability
MetEOR is released as open-source software ([https://github.com/meteor-toolkit](https://github.com/meteor-toolkit)), with code, documentation (click on package name below), and training materials available to support uptake by the EO community. Each of the open source tools is also installable via pip. 

Currently, the following tools are available as open source:

- [orbitx](https://meteor-toolkit.github.io/orbitx/): Propagates satellite orbits using Two Line Element (TLE) data to identify potential matchup events by finding spatiotemporal intersections between satellite ground tracks.
- [scrappi](https://meteor-toolkit.github.io/scrappi/): Queries, retrieves, and organises Earth observation products from multiple APIs and catalogues using a unified interface, enabling metadata-based filtering before download.
- [eoio](https://meteor-toolkit.github.io/eoio/): Provides a harmonised data-access framework that reads diverse EO products, extracts collocated regions of interest, and outputs standardised datasets with measurements, metadata, and uncertainties.
- [eomatch](https://meteor-toolkit.github.io/eomatch/): Acts as the orchestration layer that links matchup discovery, product association, and catalogue representation into a unified, reusable workflow for EO comparison analyses.
- [pydirectional](https://meteor-toolkit.github.io/pydirectional/): Models and corrects bidirectional reflectance effects by simulating and fitting BRDF behaviour to account for viewing and illumination geometry differences in comparisons.
- [processor_tools](https://meteor-toolkit.github.io/processor_tools/): A set of modular processing utilities within EO data workflows that apply transformations such as interpolation, coordinate generation, and unit conversion to enrich datasets.
- [matheo](https://matheo.readthedocs.io/en/latest/): The matheo module is a Python package providing mathematical tools for Earth observation data, including functionality for spectrally integrating measurements using sensor spectral response functions.
Provide your feedback on BizChat 

There are also two tools under development, which are not yet open source:
- scene_forge: Scene-modelling component intended to support radiative transfer and synthetic scene generation within comparison workflows.
- eoalign: A python package for preparing comparison samples for uncertainty-quantified comparisons of satellite and reference data. 

### Why MetEOR?
Comparison of EO measurements is central to calibration and validation, but generating robust matchup datasets across modern archives is often complex, computationally intensive, and fragmented.

MetEOR was developed to address this by providing a single, flexible framework that enables:

- Systematic and scalable generation of matchup datasets
- Consistent, uncertainty-aware comparison workflows
- Integration with modern EO data standards and catalogues
- Accessible, reusable tools for the wider community

### What It Provides
MetEOR is designed as a modular toolkit, allowing users to adopt individual components or build complete workflows.

Core functionality includes:

- Identification of satellite matchup opportunities
- Product search, filtering, and retrieval across EO catalogues
- Harmonised access to satellite and reference data
- Automated construction of comparison-ready datasets
- Support for uncertainty handling and analysis
- brdf and atmospheric corrections

The toolkit integrates key steps of EO comparison into a coherent and reproducible workflow.

### Demonstrated Capability
MetEOR has been applied to both large-scale and targeted comparison studies, including Sentinel-2 and Landsat-8 analyses.

These demonstrate that the toolkit can:

- Identify large volumes of cloud-free matchups
- Generate high-quality subsets for calibration studies
- Produce standardised, analysis-ready outputs

This enables consistent comparison workflows across a wide range of EO applications.
All the tools in the matchup pipeline used for the [**CEOS-PVP**](https://www.ceos-pvp.org/), are part of the MetEOR toolkit.  

### Impact
The MetEOR Toolkit lowers the barrier to rigorous, reproducible EO comparison studies, supporting:

- Improved consistency across satellite missions
- More traceable calibration and validation workflows
- Scalable analysis of multi-mission datasets

