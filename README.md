# Ball Screw Linear Actuator System
### DFM-Optimised Vertical Linear Actuator — 1000 mm Travel

> Designed by **Jubin Agrawal** | March 2026

---

## 📋 Project Overview

This project presents the complete engineering design and Design for Manufacturability (DFM) analysis of a Ball Screw Linear Actuator system. The system drives a **55 kg vertical load** over a **1000 mm stroke** at **0.4 m/s**, achieving zero backlash and a service life of **75,956 hours** — 3.8× the design requirement.

An interactive **3D model viewer** is included to visualise the complete assembly.

🔗 **[View Live Demo](https://agarwaljubin.github.io/Ball-screw-leniar-actuator/)**

---

## ⚙️ System Specifications

| Parameter | Requirement | Achieved |
|---|---|---|
| Axial Load | 55 kg (570 N) | Static: 570 N / Dynamic: 680 N |
| Travel Distance | 1000 mm | 1000 mm |
| Linear Speed | 0.4 m/s | 0.4 m/s → 2400 RPM |
| Positional Accuracy | ±0.5 mm / 1000 mm | C7 Grade (±0.05 mm/300 mm) |
| Backlash | ≤ 0.1 mm | Zero (preloaded nut + clamp coupling) |
| Service Life | 20,000 hours | **75,956 hours (3.8×)** |
| Acceleration | 0.2 s (a = 2 m/s²) | Inertial force = 110 N ✓ |

---

## 🔩 Selected Components

| Component | Model | Key Metric |
|---|---|---|
| Ball Screw | 32-10T4 (Ø32 mm, 10 mm lead, C7) | Life: 75,956 hr / Safety: 3.8× |
| Motor | YASKAWA SGM7J-08A (750 W) | Peak torque: 8.36 N·m / 2400 RPM |
| Coupling | C-SCPW46-19-19 Disc Clamp | Rating: 10 N·m / Zero Backlash |
| Bearings | Angular Contact DB pair + Radial float | Span: 1200 mm / Thermal: ±2 mm |
| Shaft | Stepped Ø32→Ø25→M25→Ø19 mm | Single setup machining |
| Base Plate | S235 Steel, 25 mm × 1400×300 mm | No secondary stiffeners required |

---

## 🏭 DFM Highlights

**9 DFM interventions** were implemented across the design:

- **Single-bar shaft machining** — Entire Ø32→Ø25→M25→Ø19 mm shaft profile machined from one Ø32 bar in a single CNC lathe setup (reduces 3–4 setups to 1)
- **Fixed + Floating bearing arrangement** — Eliminates pre-tensioning hardware; accommodates ±2 mm thermal expansion
- **Clamp-type disc coupling** — 2-bolt assembly, zero shaft marring, tool-free removal
- **Circlip groove + undercut at float end** — Fool-proof axial retention, no shimming required
- **C0.5 chamfers on all shaft edges** — Eliminates deburring step, ensures smooth bearing press-in
- **Catalogue-only components** (THK / NSK / YASKAWA) — No custom fabrication, shorter lead time
- **25 mm base plate** — Eliminates need for secondary stiffening ribs or gussets
- **C7 accuracy grade** — Meets ±0.5 mm system requirement at lower cost than C5/C3
- **Keyway for anti-rotation** — Prevents screw rotation during nut tightening

---

## 📐 Engineering Analysis Summary

### Load Analysis
- Total static weight: **570 N**
- Total dynamic axial load (incl. inertia): **680 N**
- Load safety factor: **102.5×** (Co/Fa)

### Speed & Critical Speed
- Max operating speed: **2400 RPM**
- Critical speed (fixed-fixed): **4023 RPM**
- Max permissible speed: **3218 RPM**
- Safety margin: **0.745 → SAFE ✓**

### Service Life
- Dynamic load rating C: **3252 kgf**
- Calculated life: **75,956 hours**
- Life safety factor: **3.80×**

---

## 📁 Repository Contents

```
├── index.html               # Interactive 3D model viewer
├── Ball_Screw_DFM_Report.pdf  # Full engineering DFM report
└── README.md
```

---

## 📄 Documentation

The full DFM report covers:
1. Executive Summary & Project Overview
2. Load Analysis & Ball Screw Selection
3. Speed Analysis & Critical Speed Verification
4. Service Life Calculation & Stiffness Analysis
5. Bearing Arrangement Design
6. Ball Screw Shaft — DFM Feature Design
7. Coupling Selection & Performance Analysis
8. DFM Principles Matrix
9. Structural Design, Base Plate & Conclusions

---

## 👤 Author

**Jubin Agrawal**  
March 30, 2026
