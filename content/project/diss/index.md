---
title: "Improving the Operational Resilience of Freight Transport Networks"
summary: "Multi-hazard (flood + landslip) exposure mapping and probabilistic disruption-cost modeling for freight on England’s Strategic Road Network."
tags:
  - Resilience
  - Climate Risk
  - Transport
  - GIS
  - Python
  - Risk Modeling
date: 2026-01-08
featured: true
---

## Overview

This project develops an integrated, national-scale framework to assess the **operational resilience of road freight transport under multi-hazard conditions**, focusing on **flooding** and **landslips** across England’s **Strategic Road Network (SRN)**. The aim is to connect **spatial hazard exposure** to **probabilistic disruption costs**, supporting risk-informed planning and resilience policy.

**Publication note:** A journal paper based on this research is in preparation for submission to Transportation Research Part D – Transport and Environment.

---

## Key Highlights

- Built a **GIS-based multi-hazard exposure framework** integrating surface-water flooding and landslip susceptibility on a uniform national grid.
- Identified **high-exposure segments and corridors** across the SRN, diversion routes, and freight-relevant assets (e.g., nodes and logistics hubs).
- Compared **baseline vs hazard-driven rerouting** under flood-only, landslip-only, and combined multi-hazard scenarios.
- Designed a **Python-based Monte Carlo cost model** to quantify uncertainty in HGV disruption costs (e.g., operational, environmental, and delay-related costs), identifying carbon pricing, unscheduled delays, fuel prices, and noise costs as dominant drivers of disruption cost uncertainty.
- Produced outputs designed for **decision support**, emphasizing transparency, defensible assumptions, and clear communication.

---

## Methods

**1) National-scale hazard exposure mapping (GIS)**  
- Harmonized hazard layers for flooding and landslips into a consistent spatial grid.
- Computed risk/exposure scores for SRN segments and diversion routes.

**2) Scenario-based rerouting**  
- Defined disruption “barriers” where risk clusters indicate likely closures or severe restrictions.
- Generated rerouted alternatives and extracted route distances for each scenario.

**3) Probabilistic disruption-cost modeling (Python / Monte Carlo)**  
- Built a simulation framework (NumPy/Pandas/SciPy/Matplotlib) to estimate cost distributions under uncertainty.
- Evaluated baseline and reroute cost outcomes across multiple scenarios.

---

## Figures

1. **Methodology diagram** (framework)
![Methodology diagram](fig1_methodology.png){ width=60% }
2. **Composite risk**
![Composite risk map](fig2_composite_risk.png){ width=60% }
3. **Disruption cost distribution: baseline vs hazard scenarios**
![Disruption cost distribution](fig3_cost_components_breakdown.png)

---

## Tools & Skills

- **GIS:** ArcGIS Pro / spatial data processing, raster & vector workflows, national-scale grid analysis  
- **Programming:** Python (NumPy, Pandas, SciPy, Matplotlib)  
- **Risk & resilience:** Multi-hazard screening, scenario design, uncertainty analysis (Monte Carlo)  
- **Communication:** Defensible methodology write-up, stakeholder-ready visualizations and summaries

---

## Access & Availability

To avoid pre-publishing the full dissertation while journal submission is in preparation, detailed methods, full results, and appendices are not posted publicly at this time.
