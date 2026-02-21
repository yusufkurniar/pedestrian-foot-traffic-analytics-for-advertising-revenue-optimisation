---
editor_options: 
  markdown: 
    wrap: 72
---

# Pedestrian Foot Traffic Analytics for Advertising Revenue Optimisation

**Urban mobility analytics to support infrastructure design and
advertising pricing decisions (Melbourne case study).**

This project analyses pedestrian foot traffic at three major Melbourne
CBD locations: 

- QV Melbourne 
- Southern Cross Station 
- Flinders Street Station

The analysis is designed to support **evidence-based decision making**
for: 

1) **Pedestrian infrastructure design**, and 
2) **Performance-based advertising revenue optimisation** under uncertainty.

This project is presented as a **portfolio case study**, adapted from
postgraduate analytics coursework and professional practice.

------------------------------------------------------------------------

## 🔍 Project Objectives

-   Model pedestrian foot traffic using appropriate **count data
    models**
-   Quantify **uncertainty and variability** in pedestrian demand
-   Evaluate whether **multiple sites can share a single crossing
    design** within engineering tolerance
-   Estimate **expected advertising value** using probabilistic and
    Bayesian approaches
-   Translate statistical results into **actionable planning and pricing
    insights**

------------------------------------------------------------------------

## 📌 Key Findings (Executive Summary)

-   **QV Melbourne** consistently records the highest pedestrian
    volumes, averaging approximately **2,300 people per hour**, with
    strong peak demand and variability.
-   **Southern Cross Station** and **Flinders Street Station** have
    substantially lower and statistically similar pedestrian counts
    (both below **1,000 people per hour** on average).
-   The mean difference between **Southern Cross** and **Flinders
    Street** pedestrian counts falls **within an engineering tolerance
    of 80 people/hour**, supporting the use of a **single pedestrian
    crossing design** for both sites.
-   Pedestrian counts exhibit **significant over-dispersion**, making
    **Poisson models unsuitable**. A **Negative Binomial model** is used
    throughout the analysis.
-   From an advertising perspective, **QV Melbourne** provides the
    highest expected exposure and revenue potential under a
    performance-based contract structure.

------------------------------------------------------------------------

## 📊 Data

-   **Source:** Pedestrian count dataset provided for analytical
    coursework
-   **Format:** Daily pedestrian counts for three Melbourne CBD
    locations
-   **Pre-processing:** Converted from wide to tidy (long) format for
    modelling and visualisation

------------------------------------------------------------------------

## 🧠 Methods & Techniques

-   Exploratory data analysis (EDA) and distribution diagnostics
-   Count data modelling:
    -   Poisson vs **Negative Binomial** comparison
    -   Dispersion assessment and model selection using AIC
-   High-traffic threshold estimation (e.g. **90th percentile**)
-   **Equivalence testing** using an engineering tolerance framework
-   Probabilistic revenue estimation
-   **Bayesian expected revenue modelling** for performance-based
    advertising contracts

------------------------------------------------------------------------

## 🌐 GitHub Pages

This project is published via **GitHub Pages** as a reproducible
analytics report.

➡️ **Live report:** [Pedestrian Foot Traffic Analytics for Advertising
Revenue
Optimisation](https://yusufkurniar.github.io/pedestrian-foot-traffic-analytics-for-advertising-revenue-optimisation/)

The report is generated using **Quarto**, ensuring: - Reproducibility -
Transparent methodology - Clear communication of uncertainty and
assumptions

------------------------------------------------------------------------

## ▶️ How to Reproduce the Analysis

1.  Open the RStudio project file:
    pedestrian-foot-traffic-analytics-for-advertising-revenue-optimisation.Rproj
2.  Open `Analysis.qmd` and render the report using:

-   **RStudio → Render**, or

``` r
quarto::quarto_render("Analysis.qmd")
```

3.  Required R packages include (not exhaustive): tidyverse, ggplot2,
    MASS, boot, binom, broom, patchwork

------------------------------------------------------------------------

## 📝 Notes

-   This project is intended for portfolio and demonstration purposes.
-   Results are interpreted within the context of planning and
    advertising decision support.
-   All assumptions and limitations are explicitly documented in the
    report.

------------------------------------------------------------------------

## 👤 Author

Yusuf Kurnia Romadhon
