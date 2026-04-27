# Grid-Edge Analytics: VPP Capacity & Settlement Modeling
### Optimizing Distributed Energy Resources (DERs) for Grid Reliability

## Overview
This repository provides a technical framework for analyzing residential load profiles to support the development of **Virtual Power Plants (VPPs)**. Utilizing high-resolution end-use data from the **Open Energy Data Initiative (OEDI)**, this project demonstrates how to identify grid stress points, calculate flexibility ratios for controllable loads, and simulate industry-standard **Measurement & Verification (M&V)** protocols.

In a rapidly decarbonizing grid, managing "behind-the-meter" assets like Electric Vehicles (EVs) and smart HVAC systems is critical. This analysis bridges the gap between raw interval data and market-ready capacity.

## Key Analysis Workflows
The included Jupyter Notebook (`Energy_Market_Analysis_Samples.ipynb`) covers the three technical pillars of Solutions Engineering in the energy sector:

1.  **Marginal Hour Identification:** Analyzing 8,760 hourly load shapes to determine exactly when the local distribution grid is most reliant on expensive "Marginal Units." This identifies the highest-value windows for VPP dispatch.
2.  **M&V 2.0 Settlement (High 10-in-10):** A simulation of a Demand Response event. It calculates a counterfactual baseline to quantify the delivery of **Negawatts**, ensuring transparent financial settlement between the aggregator and the utility.
3.  **DER Flexibility Assessment:** Quantifying the "shaveable" load from HVAC and EV charging. This analysis determines the **Flexibility Ratio** to provide the utility with high-confidence **Firm Capacity** guarantees.

## Tech Stack
* **Language:** Python 3.x
* **Libraries:** Pandas (Data Wrangling), NumPy (Numerical Analysis), Matplotlib & Seaborn (Visualization)
* **Data Source:** [NREL/OEDI End-Use Load Profiles for US Building Stock](https://data.openei.org/)

## Business & Grid Impact
This methodology directly addresses the primary pain points of modern utilities:
* **Non-Wires Alternatives (NWAs):** Using software orchestration to avoid multi-million dollar physical substation upgrades (CapEx avoidance).
* **Peaker Plant Displacement:** Reducing the need for high-emission fossil fuel plants during the "Summer Peak."
* **Grid Resilience:** Providing a dispatchable, statistical resource that remains reliable even with high customer opt-out variability.

---
author: Allen Aguas
