# Parametric CMM (CMM4) – Offline Programming Helper

A SOLIDWORKS® parametric **CMM head + probe library** with two sample parts to help de-risk Aberlink® offline programs.  
Aberlink’s offline view only shows a stylus shaft + ball; it doesn’t visualize the head, module, or adjacent probes.  
This assembly lets you check **access**, **clearance**, and **collisions** before you go to the machine.

> **Goal**: Get it right the first time when bringing an offline program online — fewer surprises, fewer collisions, faster prove-out.

---

## Features

- Full **CMM head** assembly with **TP20 module** and interchangeable probe library  
- **Two inspection sample parts** for realistic access checks  
- **Global variables** for parametric positioning:
  - `AngleA` (tilt): `0° → 105°`
  - `AngleB` (spin): `0° → 360°`
- **Mate setup** for stylus ball-to-feature alignment  
- Built-in **interference detection** workflow

---

## Screenshots

| Description | Preview |
|-------------|---------|
| Stylus ball coincident-mated to measured face | ![Probe–face mate](images/01_probe_face_mate.png) |
| Top view to confirm head clearance | ![Top view clearance](images/02_top_view_clearance.png) |
| Global variables for head orientation | ![Equations](images/03_equations_angles.png) |
| Probe rack simulation | ![Probe rack](images/04_probe_rack.png) |
| Interference detection in action | ![Interference](images/05_interference_detection.png) |

*(Upload your screenshots into an `images/` folder and update paths if needed.)*

---

## How to Use

1. **Open the assembly**  
   `CMM Arm Full Assembly.SLDASM`

2. **Choose a probe**  
   Suppress/unsuppress or replace:
   - `Probe 1 Dia 6.SLDPRT`
   - `Probe 2 Dia 1.SLDPRT`
   - `Probe 2 Dia 0.7.SLDPRT`
   - `Probe 3 Dia 2.SLDPRT`
   - `Probe 4 Dia 4.SLDPRT`  
   Plus `TP20 Module.SLDPRT`, `Probe Head Housing.SLDPRT`, `Probe Shaft.SLDPRT`.

3. **Insert part to inspect**  
   Use included samples (`Inspection Sample 1/2.SLDPRT`) or your own.

4. **Align probe**  
   Mate stylus ball to the target face/edge.

5. **Set head orientation**  
   In Equations:
   - `AngleA` = tilt (0–105°)  
   - `AngleB` = spin (0–360°)

6. **Check interference**  
   Use `Evaluate → Interference Detection` to detect head/part collisions.

---

## Folder Structure
