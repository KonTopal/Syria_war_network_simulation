# Network-Based Simulation of the Syrian Civil War (2011–2024)

---

## Overview

This notebook presents a **network-based simulation** of the **later stages of the Syrian Civil War**, focusing on the **evolution of territorial control** between 2019 and 2024.

The model treats **Syrian cities and towns as nodes** in a **geographical network**, each associated with demographic, geographic, and strategic attributes.  
Through iterative battle simulations and decision-making algorithms, it models how control shifts between the **state forces**, **rebel groups**, and other factions, ultimately reproducing the **December 2024 collapse of the regime**.
The analysis aims to explore how geography, demography, and resource distribution influence connectivity and centrality in Syria’s complex network structure. The simulation notebook integrates **stochastic dynamics**, **reinforcement mechanisms**, and **network-theoretic centrality metrics** to explore how **local interactions** can lead to **macro-level geopolitical outcomes**.

---

## Calibration and Goals
The model is calibrated to reproduce the **December 2024 rebel advance**, tuning the influence of:
- Population and resource distribution  
- Network centrality  
- Troop inertia and stochasticity  
- Collapse thresholds  

---

## Notebook Structure

| Section | Description |
|:--------|:-------------|
| **1. Setup & Data Import** | Load network, city data, and initialize factions |
| **2. Network Analysis** | Compute centrality measures and visualize the Syrian conflict network |
| **3. Decision-Making Algorithm** | Define the probabilistic rules for attacks and defenses |
| **4. Simulation Loop** | Run the iterative territorial evolution |
| **5. Visualization** | Display conflict maps, time series, and key metrics |
| **6. Sensitivity Analysis** | Explore how model parameters affect final outcomes |

---

## Input Data

All data are stored or loaded from the `data/` directory:

- `cities.csv` — City names, coordinates, populations, ethnoreligious majorities  
- `connections.csv` — Adjacency data or distances between cities  
- `resources.csv` — Oil/gas field coordinates and infrastructure nodes  

---

## Key Features

- **Dual role of centrality:** guides both troop distribution and target selection  
- **Stochastic realism:** includes probabilistic combat and random decision shifts  
- **Reinforcement dynamics:** success increases local combat potential  
- **Collapse modeling:** simulates overextension and regime breakdown  
- **Data-driven initialization:** built on real Syrian geographic and demographic data (2019)

---

## Expected Outcomes

- Reconstruction of the **territorial collapse** of the Assad regime in late 2024  
- Quantitative assessment of which factors most influenced the outcome  
- Insight into how **node-level dynamics** shape **macro-level geopolitical shifts**  
- A framework adaptable to other modern or historical conflicts

---

## Dependencies

To run the notebook, install:

```bash
pip install numpy pandas networkx geopandas matplotlib seaborn shapely scipy
