# 🪂 Preliminary Sizing & Performance Assessment of Spaceplanes’ Landing Parafoils

**Authors:** Jasmine Rimani, Nicola Viola, Andrea Saluzzi  
**Journal:** *Aerospace*, 2022, 9(12), 823  
**DOI:** [10.3390/aerospace9120823](https://doi.org/10.3390/aerospace9120823)  
📅 *Published: December 2022*  
🔗 [Read the full article](https://www.mdpi.com/2226-4310/9/12/823)

---

## 📌 Summary

This paper introduces a **fast and modular framework** for the **preliminary design of parafoil-based landing systems** for spaceplanes, with a focus on **Space Rider**, ESA's reusable orbital return vehicle.

The tool, called **PIMENTO (ParafoIl ModElliNg ToOl)**, integrates:
- Parafoil sizing using historical analogs,
- Six-DOF dynamics,
- Inflation modeling,
- Aerodynamic modeling based on similarity laws,
- A GNC algorithm to simulate terminal landing phases.

The goal is to support **early-stage system design** by providing performance feedback (e.g., touchdown velocity, dispersion) without requiring high-fidelity simulations.

---

## 🔍 Core Contributions

- 📐 **Parafoil Sizing Module**: Parametric estimation of canopy geometry and control surfaces based on mission mass.
- 🌬️ **Aerodynamics Module**: Uses reference data (e.g., from X-38) with corrections from test campaigns.
- 📉 **Inflation Model**: Captures dynamic effects during initial deployment to estimate operational envelope.
- 🌀 **Six-DOF Dynamics**: Includes gravity, drag, lift, and rigging angle effects for realistic motion simulation.
- 🎮 **GNC Model**: Guidance based on kino-dynamic loiter-to-final-approach strategy; control using proportional logic and flare detection.

---

## 🎯 Key Insights

- **Rapid design iteration** is possible with a fully integrated, low-fidelity model.
- The **trade-off between mass, parafoil size, and control efficiency** is critical to ensure safe landings.
- GNC logic at this fidelity can already reveal **failure scenarios** and guide design choices.

---

## 🛠 Use Cases

- Early design of reusable vehicles like **Space Rider** or **X-38-derived concepts**.
- Parametric trade studies for landing dispersion, descent time, or touchdown energy.
- Risk assessment of control failures (e.g., winch underperformance, actuator lag).

---

## 🧩 Keywords

`parafoil design` · `reentry vehicles` · `spaceplane recovery` · `six DOF dynamics` · `low-fidelity simulation` · `GNC` · `reusability`

---

## 📚 Citation (APA)

Rimani, J., Viola, N., & Saluzzi, A. (2022). An approach to the preliminary sizing and performance assessment of spaceplanes’ landing parafoils. *Aerospace, 9*(12), 823. https://doi.org/10.3390/aerospace9120823

---

## 📂 Related Work

- ✅ [Simulating Operational Concepts for Autonomous Robotic Space Exploration Systems (2023)](https://www.mdpi.com/2226-4310/10/5/408)
-🔗 [iDREAM: A Multidisciplinary Methodology and Integrated Toolset for Flight Vehicle Engineering (2022)](https://www.researchgate.net/publication/363742956_iDREAM_a_multidisciplinary_methodology_and_integrated_toolset_for_flight_vehicle_engineering)

---

## 🧠 TL;DR

**PIMENTO** gives designers a **fast, flexible** way to explore parafoil landings in the conceptual design phase, enabling validation of key performance thresholds (like vertical velocity <3 m/s) and early identification of control-related risks—**before** committing to costly high-fidelity modeling.

---

