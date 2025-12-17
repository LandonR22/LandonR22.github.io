---
title: "Identifying Sea Level Change and Vulnerable Infrastructure in Liverpool"
summary: "GIS-based assessment of national sea level change across England and building-level flood vulnerability in Liverpool using tide gauge data and elevation modeling."
tags:
  - GIS
  - Flood Risk
  - Sea Level Rise
  - Infrastructure Vulnerability
  - Spatial Analysis
date: 2024-03-01
---

## Overview
This project investigated historical sea level change around England’s coastline and assessed flood vulnerability for low-lying urban infrastructure in Liverpool. Using tide gauge records, elevation data, and building footprints, the analysis identified areas experiencing the greatest sea level rise and quantified infrastructure exposure within flood-prone elevation zones.

The work was completed as part of UCL’s *Geospatial Science* coursework and culminated in a research poster integrating national-scale trends with a detailed local case study :contentReference[oaicite:0]{index=0}.

---

## Methods
The analysis combined national-scale sea level trend mapping with a localized flood vulnerability assessment:

- Processed historical and recent tide gauge data from the Permanent Service for Mean Sea Level (PSMSL)
- Calculated sea level change between baseline (~2000) and recent (~2023) observations
- Applied Inverse Distance Weighted (IDW) interpolation to generate a continuous coastal sea level change surface
- Integrated high-resolution elevation data (OS Terrain 50) to identify areas between 0–10 meters above sea level
- Converted raster flood-prone zones to vector format and intersected them with building footprints to identify vulnerable structures

---

## Key Results
- Identified Liverpool and Heysham as experiencing some of the largest observed sea level increases along England’s coast
- Mapped national spatial variability in sea level change using interpolated tide gauge data
- Identified 14,249 buildings within the 0–10 meter elevation range in Liverpool and surrounding areas, highlighting concentrated flood exposure
- Demonstrated how combining national climate trends with local elevation and land-use data can support infrastructure risk screening

---

## Tools & Skills
QGIS · Raster & Vector Analysis · Spatial Interpolation (IDW) · Flood Risk Mapping · Cartographic Design · Spatial Data Integration

---

## Project Output
- 📄 **View Poster (PDF)**  
  [View poster](uploads/LLR_cege0094_poster.pdf)
