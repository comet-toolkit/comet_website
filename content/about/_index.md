---
widget: blank
headless: true

# ... Put Your Section Options Here (title etc.) ...
title: About
subtitle: 
weight: 10  # section position on page
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

Datasets need to have uncertainty information associated with them to ensure their credible and reliable interpretation. However, this uncertainty information can be rather complex, with many sources of error affecting the final products. Often, multiple measurements are combined throughout the processing chain (e.g. performing temporal or spatial averages). In such cases, **it is key to understand error-covariances in measurement data** (e.g., random uncertainties do not combine in the same way as systematic uncertainties). 

The Quality Assurance framework for Earth Observation (QA4EO) was established and endorsed by the Committee on Earth Observation Satellites (CEOS).  QA4EO ensures credible and reliable interpretation of environmental observations from satellites and in-situ measurements by requiring that associated uncertainty information is provided. It is also key to understand error-covariances in the data (e.g., separate handling of random and systematic uncertainties).

The approaches defined within QA4EO enable the Earth observation (EO) community to develop quantitative characterisation of uncertainty in EO data. However, practically implementing these methods is not trivial and can be time consuming. To facilitate this, **the CoMet Toolkit was developed to provide a means to store and propagate uncertainty and error-correlation information**. These tools allow the user to rely on quality-assured code, rather than having to reinvent the wheel, and lower the barrier to entry for users new to handling uncertainties.

Please have a look in the [tools section](/tools) for information on the individual tools and the [example section](/examples) for some examples on how to use the toolkit. 

The team gratefully acknowledge funding from NPL and the QA4EO project.

{{< figure src="icons/QA4EO_logo_medium.png" alt="QA4EO logo" width="250">}} {{< figure src="icons/national-physical-laboratory-npl-logo.png" alt="NPL logo" width="250">}}

