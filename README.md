# Low-Power MCML VCO using Stacking Technique

## 📌 Overview

This project presents the design and simulation of a low-power Voltage Controlled Oscillator (VCO) using MOS Current Mode Logic (MCML) with a stacking technique. The design focuses on achieving high-speed operation with reduced power consumption, making it suitable for high-frequency analog and mixed-signal applications such as PLLs and communication systems.

---

## 🎯 Objectives

* Design a high-speed VCO using MCML topology
* Reduce power consumption using stacking (current reuse) technique
* Analyze oscillation behavior through simulation
* Study trade-offs between power, speed, and voltage headroom

---

## ⚙️ Design Methodology

### 🔹 MCML Logic

MCML (MOS Current Mode Logic) operates using constant current biasing and differential signaling. It offers:

* Low voltage swing
* Faster switching speed
* Reduced noise sensitivity

These properties make MCML suitable for high-speed circuit design compared to conventional CMOS logic.

---

### 🔹 Stacking Technique

The stacking technique is used to improve power efficiency by enabling current reuse across multiple transistors. This reduces overall power consumption while maintaining high-speed performance. However, stacking introduces reduced voltage headroom, requiring careful biasing and design considerations.

---

## 🧩 Circuit Description

The designed VCO consists of differential MCML stages forming a feedback loop to sustain oscillations. The circuit includes:

* Differential pair transistors
* Constant current source for biasing
* Load resistors / active loads
* Feedback path for oscillation generation

The oscillation frequency depends on circuit parameters such as bias current and effective capacitance.

---

## 📊 Results and Analysis

The circuit was simulated to observe oscillatory behavior and evaluate performance.

* Stable oscillations were obtained at the output
* MCML topology enabled high-speed switching due to reduced voltage swing
* Stacking technique helped in lowering power consumption through current reuse
* The design demonstrates improved efficiency compared to conventional approaches

---

## 📈 Simulation Results

### Output Waveform

The output waveform shows sustained oscillations, confirming correct VCO operation.

### Frequency Behavior

The oscillation frequency is controlled by biasing conditions and circuit parameters, demonstrating tunable behavior.

---

## 🔄 Comparison with Conventional Design

| Parameter         | Conventional CMOS VCO | MCML VCO (Proposed) |
| ----------------- | --------------------- | ------------------- |
| Power Consumption | Higher                | Lower               |
| Speed             | Moderate              | High                |
| Voltage Swing     | High                  | Low                 |
| Efficiency        | Lower                 | Improved            |

---

## 🛠️ Tools Used

* Cadence Virtuoso
* Spectre Simulator
* Analog Circuit Design Techniques

---

## 🚀 Key Learnings

* Understanding of high-speed analog circuit design
* Implementation of MCML logic in oscillator design
* Importance of current reuse techniques for power optimization
* Trade-offs between power, speed, and voltage headroom

---

## 📌 Conclusion

A low-power MCML-based VCO using stacking technique was successfully designed and simulated. The circuit demonstrates high-speed operation with improved power efficiency, making it suitable for modern high-frequency integrated circuit applications.

---
