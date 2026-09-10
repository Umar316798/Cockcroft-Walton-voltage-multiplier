# 6-Stage Cockcroft-Walton Voltage Multiplier PCB

A voltage multiplier circuit designed in **KiCad 9.0**. This design uses a cascading diode-capacitor ladder network to rectify an input AC or pulsed waveform into a high-voltage DC output.

<p align="center">
<img width="1084" height="684" alt="image" src="https://github.com/user-attachments/assets/a7b00c96-05ee-44db-a729-c71a9234d203" />
  <br>
  <i>Figure 1: Completed 3D Assembly Render showing SMD Component Array</i>
</p>

---

## 🛠️ System Overview & Design Layout

The hardware features symmetrical placement to reduce current inductance while maximizing trace space distance between high potential differences.

<p align="center">
  <img width="829" height="420" alt="image" src="https://github.com/user-attachments/assets/f3a59ac9-fb6e-4184-a79c-76e5bc0562db" />
  <img width="923" height="726" alt="image" src="https://github.com/user-attachments/assets/655227f5-a7de-42f2-9af6-31e088254fcd" />
  <br>
  <i>Figure 2: Complete Design Walkthrough — Electrical Schematic and Track Layout Routing </i>
</p>

### 🔧 Component Specifications
* **EDA Tool Version:** KiCad v9.0.0+
* **Layer Count:** 2-Layer Board 
* **Diodes (D1–D6):** 6x 1N4148 High-Speed Switching Diodes (SOD-123 Package)
* **Capacitors (C1–C6):** 6x 10µF Ceramic Capacitors (1206 Package)
* **Resistors (R1, R2):** 2x 1kΩ High-Power Resistors (2010 Package)

---

## 🚀 How It Works

1. **The Ladder Cascade:** Input voltage pulses charges along the capacitor ladder. Diodes act as electrical charge peak values stage-by-stage.
2. **SMD Footprint Optimization:** By replacing classic through-hole parts with low-profile **SOD-123** and **1206** footprints, parasitical inductance is nearly eliminated.
3. **Safety Isolation:** **R1** and **R2** function as surge limiting protection variables, isolating input nodes from downstream high-voltage storage banks.

