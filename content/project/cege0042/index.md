---
title: "Comparative Spatio-Temporal Forecasting of Temperature Using ARIMA and STARIMA"
summary: "A spatio-temporal analysis comparing ARIMA and STARIMA models for monthly temperature forecasting across 274 weather stations in the Mid-Atlantic United States."
tags:
  - Spatio-Temporal Analysis
  - Time Series Forecasting
  - Climate Data
  - GIS
  - Statistical Modeling
  - R
date: 2025-03-01
---

## Overview
This project evaluated the effectiveness of incorporating spatial dependence into time series forecasting of monthly temperature data using a Space–Time Autoregressive Integrated Moving Average (STARIMA) model, compared to traditional ARIMA models. Using observations from 274 NOAA weather stations across the Mid-Atlantic United States (2000–2015), the analysis examined whether spatial structure improves medium-term climate forecasting accuracy beyond seasonality alone :contentReference[oaicite:1]{index=1}.

The work was completed as part of UCL’s *Spatial-Temporal Data Analysis & Data Mining* coursework and focused on both methodological rigor and applied climate interpretation.

---

## Methods
The analysis followed a structured spatio-temporal modeling workflow:

- Preprocessed monthly average temperature data from NOAA’s Global Summary of the Month (GSOM) dataset
- Conducted exploratory temporal, spatial, and spatio-temporal analysis to identify seasonality, persistence, and spatial structure
- Evaluated temporal autocorrelation (ACF, PACF) and spatial autocorrelation (semivariograms)
- Defined spatial relationships using a k-nearest neighbors (KNN) spatial weight matrix
- Implemented:
  - **ARIMA** models independently at each weather station using automated parameter selection
  - A **seasonal naïve baseline** for benchmarking
  - A **STARIMA** model incorporating spatial and temporal dependence
- Assessed forecast performance using NRMSE, MAE, and sMAPE metrics

All models were trained on an 80% subset of the data and evaluated over a three-year forecast horizon.

---

## Key Results
- ARIMA models struggled to outperform a simple seasonal naïve benchmark, highlighting limitations of non-spatial approaches
- STARIMA consistently achieved **lower forecast errors** across NRMSE, MAE, and sMAPE metrics
- Incorporating spatial dependence reduced average forecast error from ~32% (ARIMA) to ~19.5% (STARIMA)
- Results demonstrated that spatial structure provides **measurable predictive improvement** beyond seasonality alone
- Residual diagnostics indicated remaining seasonal dependence, identifying opportunities for further model refinement

---

## Tools & Skills
R · Spatio-Temporal Statistics · Time Series Forecasting · Autocorrelation Analysis · KNN Spatial Weights · Climate Data Analysis · Data Visualization

---

## Project Output
{{< icon name="download" pack="fas" >}}
{{< staticref "uploads/final_proj_updated_cege0042.pdf" "newtab" >}}
View full project report (PDF)
{{< /staticref >}}
