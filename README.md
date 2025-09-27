## 📌 Project Overview
This project simulates the **efficiency of a solar panel** using **digital logic components** in **LogicWorks 5**.  
The system models the effect of **light intensity** and **panel angle** on power output. It provides both **Binary (manual)** and **Decimal (step-based)** input modes, with real-time output indicators and display.

---

## 🎯 Features
- **Hybrid Input Modes**
  - Binary input via DIP switches
  - Decimal input via counters (increment/decrement)
  - Selection via multiplexer
- **PROM-based Calculations**
  - PROM lookup table for cos(angle) × 15
  - PROM multiplier (light × cos)
  - PROM BCD converter (8-bit → two digits)
- **Condition LEDs**
  - 🖤 Night Mode: Light intensity = 0
  - 💜 Weak Light: Intensity = 1–3
  - 🟩 Green: Angle = 0°–60° (Ideal)
  - 🟨 Yellow: Angle = 60°–90° (Moderate)
  - 🟥 Red: Angle > 90° (Invalid)
- **Output Display**
  - Two-digit decimal output displayed on **seven-segment LEDs**

---

## 🛠️ Tools & Components
- **LogicWorks 5** (circuit simulation)
- **PROMs** (for lookup tables, multiplication, BCD conversion)
- **DIP switches** and **Counters** (for inputs)
- **MUX** (Binary/Decimal mode selection)
- **7-Segment Displays** (output power result)
- **LEDs** (status indicators)

---

## 📐 System Flow
1. Input (Binary or Decimal) → MUX → PROM (cosine calculator)
2. Light Intensity → PROM (cosine) → PROM (multiplier)
3. Multiplier PROM output (8-bit power) → PROM (BCD converter)
4. BCD digits → 7-Segment decoders → Display
5. Parallel LED indicators for night mode, weak light, and angle validity

---

## 🚀 Expected Outcome
- Simulation of real-world solar panel behavior under varying conditions.
- Condition LEDs for intuitive feedback.
- Accurate 2-digit decimal display of power output.
- Demonstrates **lookup tables, counters, multiplexers, PROM usage, and decoders**.

---
## Circuit Image:
<img width="4712" height="2624" alt="Solar-Panel-Efficiency-Simulaor" src="https://github.com/user-attachments/assets/ad188b19-be62-44d4-aff4-2db859357fb2" />

---

## 📖 Course Context
- **Course:** Digital Logic Design (DLD)  
- **Semester:** 2nd Semester, Spring 2025  
- **University:** FAST NUCES, Karachi Campus  

---

## 📌 Skills Learned
- PROM-based lookup table design
- Multiplexing inputs and counters
- Digital multiplication using memory
- Displaying numeric outputs with BCD & seven-segment decoders
- Teamwork and circuit debugging
