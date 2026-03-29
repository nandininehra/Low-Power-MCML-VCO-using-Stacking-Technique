# Low-Power MCML VCO using Stacking Technique

## 🚀 Key Highlights

* Achieved high-speed oscillation of **~19.98 GHz**
* Reduced power consumption by **~23% using stacking technique**
* Demonstrated stable oscillations with **phase noise up to ~ -63 dBc/Hz**
* Designed and simulated using **Cadence Virtuoso (GPDK 90 nm)**

---

## 📌 Overview

Designed a **high-speed, low-power Voltage Controlled Oscillator (VCO)** using **MOS Current Mode Logic (MCML)** with a stacking technique to improve power efficiency.

The project focuses on achieving **GHz-range oscillation with reduced power consumption**, making it suitable for applications such as **Phase Locked Loops (PLLs), RF systems, and high-speed communication circuits**.

---

## 🎯 Objectives

* Design a high-frequency VCO using MCML topology
* Reduce static power consumption using stacking (current reuse)
* Analyze performance using transient, power, frequency, and phase noise analysis
* Compare conventional and proposed designs

---

## ⚙️ Design Methodology

### 🔹 MCML Logic

MCML circuits operate using:

* Constant current biasing
* Differential signaling
* Low voltage swing

This enables **high-speed switching**, reduced delay, and improved noise immunity compared to CMOS logic.

---

### 🔹 Stacking Technique

To overcome high static power consumption in MCML:

* Transistors are connected in **series (stacking)**
* Enables **current reuse**
* Reduces overall current → reduces power consumption

Trade-off: Reduced voltage headroom, requiring careful biasing.

---

## 🧩 Circuit Description

The VCO is implemented using a **3-stage ring oscillator** built from MCML inverters.

Key components:

* Differential NMOS pair
* PMOS load transistors
* Tail current source
* Feedback loop for oscillation

Oscillation condition is satisfied by achieving **360° phase shift** across stages.

---

## 📊 Results and Analysis

### 🔸 Transient Analysis

* Stable periodic oscillations observed
* Confirms correct VCO operation
* Satisfies Barkhausen criteria

---

### 🔸 Power Analysis

* Power increases with **Vbias1** (higher tail current)
* Power decreases with **Vbias2** (load variation)
* Power increases significantly with **Vdc**

#### ✅ Key Result:

* At **Vdc = 1.6 V**:

  * Without stacking: **~527 µW**
  * With stacking: **~407 µW**

👉 **~23% power reduction achieved using stacking**

---

### 🔸 Frequency and Tuning Analysis

* Maximum frequency: **~19.98 GHz**
* Frequency increases with **Vdc** (reduced delay)
* Frequency decreases with **Vbias2** (increased load resistance)
* Minimal effect of **Vbias1** due to current vs swing trade-off

👉 Demonstrates **wide tuning range and high-speed operation**

---

### 🔸 Phase Noise Analysis

* Phase noise at max frequency (~19.98 GHz): **~ -56.65 dBc/Hz**
* Best phase noise: **~ -63.03 dBc/Hz (at lower supply voltage)**
* Improved stability observed at lower frequencies

---

## 🔄 Comparison with Conventional MCML VCO

| Parameter         | Conventional MCML VCO | Proposed MCML VCO (Stacking) |
| ----------------- | --------------------- | ---------------------------- |
| Power Consumption | Higher (~527 µW)      | Lower (~407 µW)              |
| Frequency         | ~20 GHz               | ~20 GHz                      |
| Efficiency        | Lower                 | Improved                     |
| Design Approach   | Standard              | Current Reuse (Stacking)     |

---

## 📈 Simulation Outputs

* Output oscillation waveform
* Frequency tuning characteristics
* Power vs Bias Voltage graphs

(Schematics and simulation plots included in repository)

---

## 🛠️ Tools Used

* Cadence Virtuoso
* Spectre Simulator
* GPDK 90 nm Technology

---

## 🚀 Key Learnings

* High-speed analog circuit design using MCML
* Power optimization using stacking (current reuse)
* Trade-offs between power, speed, and voltage headroom
* Importance of simulation-driven design validation

---

## 📌 Conclusion

A **low-power MCML-based VCO** using stacking technique was successfully designed and analyzed.

The proposed design achieves:

* **~20 GHz high-speed operation**
* **~23% reduction in power consumption**
* Stable oscillations with acceptable phase noise

This demonstrates that **MCML combined with stacking technique** is an effective approach for **low-power, high-frequency VLSI applications**.

---

---


---
