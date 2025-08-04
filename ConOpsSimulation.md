# 🧠 Simulating Operational Concepts for Autonomous Space Robots: A Framework for Early Design Validation

**Authors:** Jasmine Rimani, Nicola Viola, Stéphanie Lizy-Destrez  
**Journal:** Aerospace 2023, 10(5), 408  
**DOI:** [10.3390/aerospace10050408](https://doi.org/10.3390/aerospace10050408)  
📅 *Published: May 2023*

🔗 [📄 Read the Full Paper](https://www.mdpi.com/2226-4310/10/5/408)

---

## 🚀 Summary

Autonomous systems are crucial for planetary exploration, yet their **operational behavior** is often hard to evaluate early in the design phase. Traditional Concept of Operations (ConOps) approaches often overlook **dynamic interactions** between system behavior, resources, and mission goals.

This study introduces a **simulation-backed framework** that helps **validate and refine operational scenarios** during the conceptual and preliminary design of autonomous robotic systems—*before hardware even exists*.

---

## 🧭 Motivation

Designing autonomous systems involves major systems engineering challenges:

- ✍️ Writing realistic and flexible **requirements** and **ConOps**
- 🔌 Managing **interfaces** between hardware, software, and human operators  
- ✅ Ensuring **verification & validation (V&V)** of system behavior  

Standard ConOps approaches are limited when autonomy increases. They often assume static behavior and ignore context-driven decision-making. This framework closes that gap by simulating how a system **reacts to its environment**, plans missions, and consumes resources from the very first steps of mission design.

---

## 🧱 Framework Architecture

### 1. **Model-Based Systems Engineering (MBSE)**
- Serves as the knowledge base for the system’s physical and functional architecture  
- Stores all mission scenarios, operations, constraints, and resources  

### 2. **Simulation Engine using MDP + MCTS**
- **Markov Decision Process (MDP)** defines decision space  
- **Monte Carlo Tree Search (MCTS)** solves for near-optimal operational timelines  
- Output: A feasible plan maximizing **scientific return** under **resource constraints**

### 3. **Scenario Execution & Visualization**
- Tracks **step-wise changes** in:
  - Power usage
  - Data storage
  - Mission time  
- Validates design against mission goals

---

## 🤖 Case Study: Lunar Surface Rover

- ⚖️ Mass: 30 kg  
- 🔋 Power: ~100 W (with recharging)  
- 🎯 Goal: Visit and sample high-value waypoints  
- 🧠 Decision-making is handled by the framework based on resource usage and mission utility

---

## 🧪 Key Contributions

- ✅ Simulates operational behavior **during early design**. 
- 🧩 Captures tight integration of autonomy, physical systems, and mission goals  
- 🧠 Provides traceable, explainable planning logic using **MBSE + MDP**  
- 🔁 Enables **reusability and modularity** across mission designs

---

## 🧩 Keywords

`MBSE` • `ConOps` • `MDP` • `MCTS` • `Space Robotics` • `Autonomy` • `System Simulation` • `Planetary Exploration`

---
## 🔍 Related Work

- 🔗[Integrated Conceptual Design and Parametric Control Assessment for a Hybrid Mobility Lunar Hopper](https://www.mdpi.com/2226-4310/10/8/669)
- 🔗[Application of a hierarchical task planner to a lunar lava tube analogue robotic mission](https://www.researchgate.net/publication/355873695_Application_of_a_hierarchical_task_planner_to_a_lunar_lava_tube_analogue_robotic_mission)
- 🔗[Sizing of a Propelled-Hopping System on the Moon](https://www.researchgate.net/publication/363743254_Sizing_of_a_Propelled-Hopping_System_on_the_Moon)
- 🔗[An Integrated Design Platform to Analyse and Size Planetary Exploration Systems Applied to Lunar Lava Tube Exploration](https://www.researchgate.net/publication/363742561_An_Integrated_Design_Platform_to_Analyse_and_Size_Planetary_Exploration_Systems_Applied_to_Lunar_Lava_Tube_Exploration)

---

## 📝 Citation

If this work supports your research, please cite:

```bibtex
@article{Rimani2023ConOps,
  author = {Rimani, Jasmine and Viola, Nicola and Lizy-Destrez, Stéphanie},
  title = {Simulating Operational Concepts for Autonomous Robotic Space Exploration Systems: A Framework for Early Design Validation},
  journal = {Aerospace},
  year = {2023},
  volume = {10},
  number = {5},
  pages = {408},
  doi = {10.3390/aerospace10050408}
}
