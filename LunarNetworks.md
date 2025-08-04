# 📡 Parametric Data Handling for Autonomous Lunar Networks

**Authors:** Jasmine Rimani · Luigi Mascolo · Juan A. Fraire  
**Journal:** CEAS Space Journal, Vol 14, pp. 365–376 (2022)  
**DOI:** [10.1007/s12567-021-00390-4](https://doi.org/10.1007/s12567-021-00390-4)  
📅 *Published: 22 September 2021 (Issue date: April 2022)*  
🔗 [Read the full article ↗︎](https://link.springer.com/article/10.1007/s12567-021-00390-4)

---

## 🧠 Summary

As upcoming lunar missions generate massive volumes of scientific data (e.g. 3D mapping of lava tube skylights), reliable and efficient communication becomes mission‑critical. This work introduces a **parametric framework** to evaluate communication and data‑handling architectures—**bent‑pipe (BP), store‑and‑forward (S&F), store‑carry‑and‑forward (SC&F)**—against configurable networks, data volumes, and mission sites. A case study using **six lunar relay satellites** and multiple ground stations servicing the **Marius Hills lava tube** demonstrates how the framework identifies thresholds where one architecture outperforms another, enabling rapid trade-off analysis in early mission design.

---

## ✅ Core Contributions

- A **hardware-agnostic evaluation algorithm** that inputs satellite orbits, ground stations, point-of-interest location, data volumes—and outputs the optimal data‑handling architecture.
- Detection of **inflection points** (e.g. ~1.5 Tbit/day) where SC&F becomes preferable over simpler architectures in the lava-tube use case.
- A **generalizable tool** keyed to modular configurability (e.g. add ground stations, vary antenna gains, orbital parameters), reusable across lunar mission concepts.

---

## 🧪 Methodology

1. **Orbit & GS configuration**: Six satellites in two RAAN clusters (0° and 90° inclination), plus DSN Earth ground stations (Goldstone, Canberra, Madrid); site-of-interest at Marius Hills.  
2. **Communication modelling**: X‑band data links (150 Mbit/s), compressed payload volumes (e.g. 160 Gbit, 2–4 Tbit), device telemetry protocols (S‑band) considered.  
3. **Data-handling modes**:  
   - **BP** (real-time relay)  
   - **S&F** (upload then download)  
   - **SC&F** (multi-step store-and-forward, implements DTN logic)  
4. **Evaluation algorithm**: Post-processes STK-generated access windows; simulates upload/download sequences; handles partial transfers; outputs number of successful transmissions and mode usage per architecture.

---

## 📊 Validation & Results

- **Low data rates (e.g. ≤ 0.16 Tbit/day)**: S&F overwhelmingly used (> 80% of transfers) as windows are large enough. SC&F rarely required.  
- **High data rates (> ~1.5 Tbit/day)**: SC&F becomes necessary, and eventually dominant for throughput. Inflection point shifts with additional ground stations (≈ 2 Tbit for two GSs, ≈2.5 Tbit for three).  
- **BP architecture covers <10%** of communication opportunities and only in short windows—inefficient for typical lunar payload profiles.  
- Satellites with RAAN = 0° outperform those at 90°, and data throughput increases predictably as GS count rises.

---

## 🔍 Key Insights

- SC&F (DTN‑style) is essential for **high-volume mission support**, especially in degraded or stretched networks.  
- BP strategy is **highly sensitive to LOS availability**, and impractical for continuous daily data demands.  
- Evaluation thresholds (e.g. ~1.5 Tbit) provide **design guards** for constellation sizing and GS placement.  
- The algorithm is **lightweight and adaptable**, facilitating rapid architecture feasibility checks.

---

## 🛠️ Use Cases

- **Early-phase mission concept trade‑studies**: choose number of relays vs. GSs vs. architecture.  
- **Lava tube/ISRU missions**: guarantee required downlink bandwidth per site (e.g. drones or robots exploring sub-surface).  
- **Delay‑tolerant design evaluation**: simulate combinations of SC&F vs. S&F under partial contacts or relay loss.  
- **Strategic planning**: assess coverage redundancy, network resilience, or mission extension scenarios.

---

## 🧩 Keywords

Communication · Moon · Lava tubes · Space networking · Access analysis · Delay-/Disruption‑Tolerant Networking · Lunar relay constellation

---

## 📚 APA Citation

Rimani, J., Mascolo, L., & Fraire, J. A. (2021). *A parametric data handling evaluation framework for autonomous lunar networks*. CEAS Space Journal, 14, 365–376. https://doi.org/10.1007/s12567-021-00390-4

---

## Related Work in This Series

## 🔍 Related Work

- 🔗 [Simulating Operational Concepts for Autonomous Robotic Space Exploration Systems (2023)](https://www.mdpi.com/2226-4310/10/5/408)
- 🔗 [Application of a Hierarchical Task Planner to a Lunar Lava Tube Analogue Robotic Mission (2021)](https://www.researchgate.net/publication/355873695_Application_of_a_hierarchical_task_planner_to_a_lunar_lava_tube_analogue_robotic_mission)
- 🔗 [Sizing of a Propelled-Hopping System on the Moon (2022)](https://www.researchgate.net/publication/363743254_Sizing_of_a_Propelled-Hopping_System_on_the_Moon)
- 🔗 [An Integrated Design Platform to Analyse and Size Planetary Exploration Systems Applied to Lunar Lava Tube Exploration (2022)](https://www.researchgate.net/publication/363742561_An_Integrated_Design_Platform_to_Analyse_and_Size_Planetary_Exploration_Systems_Applied_to_Lunar_Lava_Tube_Exploration)
- 🔗 [A Novel Approach to Planetary Rover Guidance, Navigation and Control Based on the Estimation of the Remaining Useful Life (2020)](https://www.researchgate.net/publication/355873613_A_novel_approach_to_planetary_rover_guidance_navigation_and_control_based_on_the_estimation_of_the_remaining_useful_life)

---

## TL;DR

A flexible parametric tool—tested on Marius Hills lava tube networks—quickly shows *when* and *why* to adopt SC&F (DTN) vs. S&F, identifies critical thresholds (~1.5 Tbit/day), and helps shape next-gen lunar comms architectures before landing pad designs ever begin.

---
