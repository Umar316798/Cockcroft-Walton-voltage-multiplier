
A compact, multi-stage hardware voltage multiplier circuit designed in **KiCad 9.0**. This design utilizes a cascading diode-capacitor ladder network to progressively clamp, rectify, and elevate an input AC or pulsed waveform into a high-voltage DC output.

<p align="center">
  <img src="3d_view.png" alt="PCB 3D Render View" width="550"/>
  <br>
  <i>Figure 1: Completed 3D Assembly Render showing SMD Component Array</i>


---

## 🛠️ System Overview & Design Layout

The hardware features an elegant symmetrical placement engineered to reduce current loop inductance while maximizing trace space distance between high potential differences.

<p align="center">
  <img src="schematic.png" alt="Circuit Schematic Diagram" width="48%"/>
  <img src="pcb_layout.png" alt="2D Copper Layout Database" width="48%"/>
  <br>
  <i>Figure 2: Complete Design Walkthrough — Electrical Schematic (Left) vs. Dual-Layer Track Layout Routing (Right)</i>
</p>

### 🔧 Component Specifications
* **EDA Tool Version:** KiCad v9.0.0+
* **Layer Count:** 2-Layer Board (Integrated Ground Shielding Pour)
* **Diodes (D1–D6):** 6x 1N4148 High-Speed Switching Diodes (SOD-123 Package)
* **Capacitors (C1–C6):** 6x 10µF Multi-layer Ceramic Capacitors (1206 Package)
* **Resistors (R1, R2):** 2x 1kΩ High-Power Energy Dampening Resistors (2010 Package)

---

## 🚀 How It Works

1. **The Ladder Cascade:** Input voltage pulses shuffle charges along the capacitor ladder. Diodes act as electrical check-valves, locking charge peak values stage-by-stage.
2. **SMD Footprint Optimization:** By replacing classic through-hole parts with low-profile **SOD-123** and **1206** footprints, parasitical inductance is nearly eliminated.
3. **Safety Isolation:** **R1** and **R2** function as surge limitin
