# 🛰️ Securing Satellite Operations: A Novel Approach for Space Assets On-Board Safety

**Authors:** Jasmine Rimani, Lorenzo Buizza, Aurélie Baker  
**Conference:** IAF Space Systems Symposium, 75th International Astronautical Congress (IAC 2024)  
**DOI:** [10.52202/078372-0013](https://doi.org/10.52202/078372-0013)  
📅 *Published: January 2024*

---

## 🚀 Overview

With the proliferation of autonomous satellites and mega-constellations, space systems are now more exposed to cybersecurity threats than ever before. Traditional ground-segment defenses often react *after* an intrusion has occurred—leaving spacecraft vulnerable to command hijacking, GNSS spoofing, and mission degradation.

This research introduces **SafetySat**: a novel onboard safety framework that enables satellites to **detect anomalous commands or signals and protect themselves in real time**, significantly enhancing mission resilience.

---

## 🔐 Key Challenges Addressed

- **Telecommand Hijacking:** Unauthorized commands can be trusted blindly by spacecraft once decoded.
- **GNSS Spoofing & Jamming:** Can mislead navigation, timing, and orbit control systems.
- **Operator Burden:** Current cyberattack detection methods rely heavily on human ground support post-incident.
- **Standardization Vulnerabilities:** Uniform software/hardware opens doors for repeatable attacks across constellations.

---

## 🧠 Our Approach: SafetySat

**Two complementary detection axes** were designed to run *directly onboard* satellites:

### 1. Model-Driven Telecommand Validation
- ✅ Uses **ontology-based reasoning** to validate command sequences.
- 🚫 Detects harmful or anomalous sequences *before execution*.
- 🛰️ Suitable for autonomous spacecraft or ground support planning.

### 2. Data-Driven GNSS Spoofing Detection
- 📈 Leverages telemetry data to detect abnormal signal behavior.
- 🧪 Initial tests with **DBSCAN** and **KMeans** show promise, but future work explores:
  - **Agglomerative Clustering**
  - **LSTM-based AutoEncoders**
- 🌍 Expanding datasets from multiple LEO missions will improve detection accuracy.

---

## 🔬 Results & Use Cases

SafetySat was evaluated in two real-world use cases:

1. **Onboard Telecommand Verification:** Prevents execution of unexpected or hazardous commands.
2. **GNSS Spoofing Detection:** Especially relevant for LEO satellites with autonomous maneuvering capabilities.

Early testing confirms the potential of SafetySat to **proactively detect** and **report anomalous commands** without waiting for operator intervention.

---

## 📚 Keywords

`Knowledge Systems` • `Autonomous Systems` • `On-board Safety` • `GNSS Spoofing` • `Cyberattack Detection` • `Clustering Algorithms`

---

## 📈 Future Work

- Improve temporal GNSS anomalous signals detection with **deep learning models** (e.g., LSTM AutoEncoders).
- Integrate richer datasets across varied satellite missions.
- Build generalized onboard cybersecurity modules for next-gen satellite platforms.

---

## 🧩 Why This Matters

As space missions become more autonomous and complex, cybersecurity must evolve **beyond Earth**. SafetySat represents a critical shift—**bringing AI-powered defense directly onboard**, ensuring space assets are equipped to safeguard themselves in real-time.

---

## 📎 Citation

If you use or reference this work, please cite:

```bibtex
@inproceedings{Rimani2024Securing,
  author = {Rimani, Jasmine and Buizza, Lorenzo and Baker, Aurélie},
  title = {Securing Satellite Operations: A Novel Approach for Space Assets On-Board Safety},
  booktitle = {IAF Space Systems Symposium, 75th International Astronautical Congress (IAC)},
  year = {2024},
  doi = {10.52202/078372-0013}
}
