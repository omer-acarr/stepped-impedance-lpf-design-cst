# 📡 Microstrip Stepped-Impedance LPF Design

![Software](https://img.shields.io/badge/Software-CST_Studio_Suite_2025-blue?style=flat-square&logo=dassaultsystemes)
![Material](https://img.shields.io/badge/Material-Rogers_RO4003C-orange?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-RF_/_Microwave-green?style=flat-square)
![Analysis](https://img.shields.io/badge/Analysis-EM_Simulation-red?style=flat-square)

This repository contains the design, simulation, and performance analysis of a **Microstrip Stepped-Impedance Low Pass Filter** developed in **CST Studio Suite 2025**.

## 📌 Project Overview
Stepped-impedance filters are essential components in RF/Microwave systems, providing a compact way to implement low-pass characteristics using alternating sections of high and low characteristic impedance.

This project focuses on a multi-section LPF designed on a high-performance **Rogers RO4003C** substrate, suitable for high-frequency applications requiring sharp roll-off and minimal insertion loss.

### Key Features:
* **Filter Topology:** Stepped-Impedance (Hi-Z / Low-Z sections)
* **Substrate Material:** Rogers RO4003C
* **Dielectric Constant ($\varepsilon_r$):** 3.55
* **Substrate Height ($h$):** 0.508 mm
* **Simulation Range:** 0 - 10 GHz
---
## 🛠 Design & Parameters

The filter geometry is fully parameterized, allowing for easy optimization and tuning of the cut-off frequency.

| Parameter | Value (mm) | Description |
| :--- | :--- | :--- |
| **W0** | 1.12 | 50 Ohm Feedline Width |
| **Wl** | 4.0 | Low-Impedance (Capacitive) Width |
| **Wh** | 0.2 | High-Impedance (Inductive) Width |
| **h** | 0.508 | Substrate Thickness |
| **t** | 0.018 | Copper Thickness |

---
## 🖥 Simulation & Mesh Settings

To ensure the accuracy of the electromagnetic fields, the following simulation settings were applied:

* **Solver:** Transient Solver
* **Mesh Type:** Hexahedral Mesh
* **Total Mesh Cells:** 178,848
* **Mesh Density:** Balanced for high-frequency accuracy at the discontinuities of the stepped sections.
---
## 📊 Simulation Results

The results demonstrate a clear low-pass response with a cut-off frequency near **8.5 - 9 GHz**.

* **Return Loss ($S_{11}$):** Stays below -15 dB throughout the passband, indicating excellent impedance matching.
* **Insertion Loss ($S_{21}$):** Minimal loss in the passband with a sharp transition at the stopband (~9 GHz).




