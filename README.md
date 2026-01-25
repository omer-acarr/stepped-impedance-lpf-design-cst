# 📡 Microstrip Stepped-Impedance LPF Designer

![Software](https://img.shields.io/badge/Software-CST_Studio_Suite_2025-blue?style=flat-square&logo=dassaultsystemes)
![Material](https://img.shields.io/badge/Material-Rogers_RO4003C-orange?style=flat-square)
![Domain](https://img.shields.io/badge/Domain-RF_/_Microwave-green?style=flat-square)
![Analysis](https://img.shields.io/badge/Analysis-EM_Simulation-red?style=flat-square)

An electromagnetic design and high-fidelity simulation of a **Microstrip Stepped-Impedance Low-Pass Filter (LPF)**, optimized for high-frequency defense and communication systems. This project represents the transition from theoretical microwave synthesis to 3D electromagnetic verification using industrial-grade materials.

## 🎯 Project Motivation

At microwave frequencies (GHz range), traditional lumped elements (SMD inductors and capacitors) fail due to parasitic effects. This project addresses these physical constraints by:
* **Distributed Element Design**: Utilizing alternating high-impedance (inductive) and low-impedance (capacitive) microstrip lines to implement the filter transfer function.
* **RO4003C Optimization**: Selecting Rogers RO4003C, a defense-standard low-loss dielectric, to ensure thermal stability and high performance.
* **High Precision Analysis**: Accounting for fringing fields and step-discontinuity parasitics through full 3D electromagnetic analysis, unlike basic circuit simulators.

## 🚀 Technical Highlights

* **Frequency Domain Solver**: Employed for high-precision matrix inversion, achieving a solver accuracy of **$2.22 \times 10^{-09}$**.
* **Wide-Band Mode Analysis**: Verified **Quasi-TEM** mode propagation across the **$4-6\ GHz$** band at the excitation ports.
* **Impedance Matching**: Optimized feed lines to a characteristic impedance of **$48.51\ \Omega$** to ensure maximum power transfer.

## 📊 Design Parameters

The filter geometry is defined by the following optimized parameters:

* 📏 **W0 (Feed Line)**: $1.12\ mm$ for $50\ \Omega$ matching.
* 📏 **WI (Capacitive Section)**: $4.0\ mm$ (Low-impedance section).
* 📏 **Wh (Inductive Section)**: $0.2\ mm$ (High-impedance section).
* 📏 **Stage Lengths**: $1.58\ mm$, $1.47\ mm$, and $2.73\ mm$ for optimized rejection.
* 📏 **Total Length (x1)**: $13.83\ mm$.



## 🛠️ Simulation Setup

* **Software Platform**: CST Studio Suite 2025.
* **Substrate Material**: Rogers **RO4003C (lossy)**, $\epsilon_r = 3.38$.
* **Dielectric Height ($h$)**: $1.588\ mm$.
* **Metallization**: Annealed Copper with thickness **$t = 0.018\ mm$**.
* **Port Analysis**: Quasi-TEM mode analysis performed across the **$4-6\ GHz$** frequency range.


