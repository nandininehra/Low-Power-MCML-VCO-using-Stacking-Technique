# MCML-Based Low Power Ring VCO with Stacking Technique (90nm Cadence Design)

## Overview

This project presents the design and analysis of a **MOS Current Mode Logic (MCML) based Ring Voltage Controlled Oscillator (VCO)** implemented using **Cadence Virtuoso (GPDK 90nm technology)**.

A **stacking technique** is introduced to reduce static power consumption while maintaining high-frequency performance.

### Key Achievements

* Achieved **~23% reduction in power consumption** using stacking
* Operating frequency up to **~20 GHz**
* Improved stability with controlled **phase noise (~ -63 dBc/Hz)**
* Verified using **Transient, PSS, and PNOISE simulations**

---

## Key Concepts Used

* MCML (MOS Current Mode Logic)
* Differential Pair Design
* Ring Oscillator Architecture
* Voltage Controlled Oscillation
* Bias-controlled tuning (Vbias1, Vbias2)
* Stacking Technique for Low Power Design
* Phase Noise Analysis (PSS & PNOISE)

---

## Circuit Description

* Designed a **3-stage ring oscillator** using MCML inverters
* Each stage consists of:

  * NMOS differential pair
  * PMOS load transistors
  * Tail current source

### Control Parameters

* **Vbias1** → controls tail current
* **Vbias2** → controls load resistance
* **Vdc** → supply voltage (1.6V)

The output of the last stage is fed back to the first stage to sustain oscillations.

---

## Working Principle

* Oscillation satisfies **Barkhausen Criteria**:

  * Loop gain ≥ 1
  * Total phase shift = 360°

* Frequency of oscillation:

[
f = \frac{1}{2 N t_d}
]

where:

* N = number of stages
* td = delay per stage

---

## Stacking Technique (Proposed Work)

The major drawback of MCML circuits is **high static power consumption** due to constant bias current.

### Solution:

* Introduced an **additional NMOS transistor in series** with tail current source
* This increases effective resistance → reduces current → reduces power

[
P = V \cdot I
]

 Lower current directly reduces power consumption.

---

## 📊 Results Summary

### 🔹 Power Comparison

| Design                | Power (µW) at Vdc = 1.6V |
| --------------------- | ------------------------ |
| Conventional MCML VCO | ~527 µW                  |
| With Stacking         | ~407 µW                  |

✅ **~23% power reduction achieved**

---

### 🔹 Frequency Performance

* Maximum frequency: **~19.98 GHz**
* Frequency increases with **Vdc**
* Frequency decreases with **Vbias2** (due to increased load resistance)

---

### 🔹 Phase Noise Performance

* Best phase noise: **~ -63 dBc/Hz**
* At max frequency (~20 GHz): **~ -56 dBc/Hz**
* Improved stability at lower frequencies

---

##  Analysis Performed

### 🔸 Power Analysis

* Power vs Vbias1
* Power vs Vbias2
* Power vs Vdc
* Comparison: With vs Without Stacking

---
##  Simulation Details

* Technology: **GPDK 90nm**
* Tool: **Cadence Virtuoso**
* Supply Voltage: **1.6 V**

### Analyses Performed:

* Transient Analysis → Oscillation verification
* PSS (Periodic Steady State) → Stable oscillation
* PNOISE → Phase noise evaluation


##  Key Observations

* Power increases with **Vbias1** due to increased current
* Power decreases with **Vbias2** due to increased load resistance
* Power increases significantly with **Vdc**
* Stacking technique consistently reduces power across all conditions


## Future Work

* Layout design and post-layout simulation
* Further power optimization techniques


## Tools Used

* Cadence Virtuoso
* Analog Design Environment (ADE)
* GPDK 90nm Technology

---

##  Documentation

Detailed explanation available in:
📂 `docs/MCML_VCO_Paper.pdf`

---

## Author

**Nandini Nehra**
Electronics Engineering Student
Interest: Analog IC Design | VLSI | Semiconductor Devices

---

## ⭐ Project Highlight

**Designed and analyzed a high-frequency (~20 GHz) MCML VCO with reduced power consumption using stacking technique, validated through Cadence simulations (PSS & PNOISE).**

---

