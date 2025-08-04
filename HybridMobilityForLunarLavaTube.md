# 🌑 Hybrid Mobility for Lunar Lava Tube Exploration: Conceptual Design & Control Assessment

**Authors:** Jasmine Rimani, Giacomo Bucchioni, Adam D. Ryals, Nicola Viola, Séverine Lizy-Destrez  
**Journal:** Aerospace 2023, 10(8), 669  
**DOI:** [10.3390/aerospace10080669](https://doi.org/10.3390/aerospace10080669)  

📅 *Published: August 2023*

🔗 [📄 Read the Full Paper](https://www.mdpi.com/2226-4310/10/8/669)

---

## 🧭 Mission Context

As space agencies plan sustained lunar presence, **lunar lava tubes**—natural underground tunnels formed by ancient volcanic activity—have emerged as prime candidates for future outposts. They offer:
- 🌡️ Thermal insulation  
- 🛡️ Protection from radiation, micrometeoroids, and regolith  
- 🔬 A pristine environment for scientific study  

But accessing and navigating these caves requires mobility systems capable of overcoming rugged terrain and communication blackouts.

---

## 🚀 Overview of the Study

This paper presents a **preliminary design** for a robotic *cave explorer* targeting lunar lava tubes, combining:
- **Conceptual systems engineering**
- **Parametric mass and power estimation**
- **Control performance analysis under design variations**

> The novelty lies in the **tight coupling of design feasibility and adaptive control capability**—assessing whether mobility and GNC systems can remain effective under mass/inertia fluctuations as the design evolves.

---

## 🤖 Key Features of the Lunar Hopper

### 🔁 Hybrid Mobility System
- **Wheels + Thrusters** for dual-mode terrain traversal:
  - Wheels for efficiency on flat basaltic terrain
  - Thrusters for semi-ballistic hops over large obstacles

### 🧠 Autonomy Level
- Targeting **ECSS E3-level autonomy** (adaptive onboard decision-making)
- Required due to limited Earth communication in subsurface environments

### ⚙️ Control Approach
- **Baseline PID controller** enhanced with:
  - **MRAC (Model Reference Adaptive Control)** to dynamically adjust to mass variations
- Enables GNC performance assessment *early in the design lifecycle*

---

## 📐 Contributions to Space Systems Design

### ✅ Mission Architecture & Stakeholder Mapping
- Identification of user needs, mission goals, and operational constraints

### 🧮 Preliminary Design Box
- Parametric estimation of:
  - Mass
  - Power consumption
  - System layout
- Provides an initial **feasibility boundary** for future iterations

### 🎯 Control-Driven Design Constraints
- GNC hardware (sensors & actuators) defines the **performance envelope** for mass variation
- PID+MRAC control helps estimate **safe mass growth margins** without redesign

---

## 🔁 Why This Matters

Most studies treat **guidance and control** as an optimization *after* design freeze.  
This work flips that logic:

> **What if we use GNC performance to *shape* the design itself from the start?**

This approach:
- Enables **earlier design validation**
- Reduces redesign risk
- Facilitates **in-flight certification**
- Prepares the system for autonomous adaptability in unknown environments

---

## 🔍 Future Work

- Extend MRAC controller with **robust or optimal control** strategies
- Broader **Multidisciplinary Design Optimization (MDO)** integration
- Explore **flexible GNC architectures** that evolve with system parameters
- Include full mission simulations in lunar cave analog environments

---

## 🧩 Keywords

`MBSE` • `GNC` • `MRAC` • `Lunar Hopper` • `Lava Tubes` • `Adaptive Control` • `Space Robotics` • `Systems Engineering`

---

## 📎 Citation

If this work contributes to your research, please cite:

```bibtex
@article{Rimani2023Hopper,
  author = {Rimani, Jasmine and Bucchioni, Giacomo and Ryals, Adam D. and Viola, Nicola and Lizy-Destrez, Séverine},
  title = {Integrated Conceptual Design and Parametric Control Assessment for a Hybrid Mobility Lunar Hopper},
  journal = {Aerospace},
  year = {2023},
  volume = {10},
  number = {8},
  pages = {669},
  doi = {10.3390/aerospace10080669}
}
