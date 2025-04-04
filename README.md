# 🌡️ SPR PCF Biosensor – Design 1

This repository presents the design and simulation of a **highly sensitive dual-core Surface Plasmon Resonance (SPR) based Photonic Crystal Fiber (PCF) biosensor** for detecting small refractive index variations. The biosensor utilizes **Silver (Ag)** as a plasmonic material, enhanced by a thin **Titanium Dioxide (TiO₂)** layer to improve chemical stability and performance.

## 🔍 Project Summary

- **Purpose**: To develop a dual-core PCF-based SPR biosensor capable of detecting minor changes in refractive index with high sensitivity.
- **Plasmonic Materials**: Silver + TiO₂ (anti-oxidation layer)
- **Simulation Method**: Finite Element Method (FEM)
- **Application Areas**: Biomedical diagnostics, chemical sensing, environmental monitoring.


## 🧪 Working Principle

The sensor operates by exciting **surface plasmons** at the metal–dielectric interface. When the **core-guided mode** and **SPP mode** intersect, **resonance occurs**, leading to a spike in **confinement loss** — this is the detection mechanism.

Key Features:
- Phase matching condition achieved at **λ = 1.65 μm**
- Strong evanescent field interaction enhances sensitivity


## 📐 Design Parameters

| Parameter | Symbol | Value |
|----------|--------|-------|
| Circle 1 diameter | d₁ | 1.8 μm |
| Circle 2 diameter | d₂ | 1.0 μm |
| Circle 3 diameter | d₃ | 1.65 μm |
| Pitch (hole spacing) | A | 3.3 μm |
| Silver thickness | Ts | 65 nm |
| TiO₂ thickness | ti | 10 nm |
| Microchannel width | mc | 1.75 μm |
| Analyte RI | na | 1.36 |
| Operating Wavelength | opw | 1.72 μm |


## 🧮 Sellmeier & Dielectric Equations

- **Silica Refractive Index**:
nsilica = sqrt(1 + (b1λ²)/(λ²−c1) + (b2λ²)/(λ²−c2) + (b3λ²)/(λ²−c3))
- **TiO₂ Dielectric Constant**:
nti = sqrt(5.913 + (2.441×10⁷)/(λ² − 0.803×10⁷))

## 📊 Simulation Highlights

### 📌 1. Phase Matching

- Resonance occurs at **λ = 1.65 μm** where:
- Core mode index ≈ SPP mode index
- Confinement loss peaks at **263 dB/cm**



### 📌 2. Refractive Index Sensing

- Analyte RI varied from **1.36 to 1.39**
- Loss curve shifts to higher wavelength with increased RI
- Demonstrates high sensitivity



### 📌 3. Amplitude Sensitivity

- Calculated using confinement loss difference
- Amplitude sensitivity peaks at **1.36–1.39 RI**



## 🔧 Parameter Variation Results

This study explores how key structural parameters impact performance:

| Parameter | Insight |
|----------|---------|
| **d₁ (Circle 1 diameter)** | Affects confinement loss significantly |
| **d₂ (Circle 2 diameter)** | Controls x-polarized core mode loss |
| **d₃ (Circle 3 diameter)** | Adjusts mode interaction strength |
| **Pitch (A)** | Alters field distribution and phase matching |
| **Silver Thickness** | Impacts peak loss location |
| **TiO₂ Layer Thickness** | Modifies resonance sharpness and stability |

Each of these was simulated and plotted in the report.


## 📁 Files in This Repo

| File | Description |
|------|-------------|
| `Sensor_Design1_Report.docx` | Full report with theory, modeling, results |
| `README.md` | Project summary and GitHub documentation |
| `images/` | Extracted graphs and figures for README display |

## 🧠 Conclusion

This dual-core PCF SPR biosensor demonstrates:
- High confinement loss at resonance
- Excellent tunability through structural parameters
- Sensitivity to small RI changes — suitable for medical and biochemical sensin

## 🛠 Tools Used

- **COMSOL Multiphysics** (FEM Simulation)
- **Microsoft Word**
- **Excel**

