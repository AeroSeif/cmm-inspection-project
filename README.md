# Parametric CMM (PH10T) – Offline Programming Helper

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

**Coincident mate between probe tip and inspection face**
![Coincident Mate](PH10T/screenshots/Screenshot%202025-09-05%20065708.png)

**Top view to check probe clearance**
![Top View](PH10T/screenshots/Screenshot%202025-09-05%20065812.png)

**Probe head orientation with variable angles**
![Angles Applied](PH10T/screenshots/Screenshot%202025-09-05%20065918.png)

**Exploded view showing probes and head at A=0°, B=0°**
![Exploded View](PH10T/screenshots/Screenshot%202025-09-05%20071349.png)

**Interference detection results**
![Interference Detection](PH10T/screenshots/Screenshot%202025-09-05%20072559.png)




---

## How to Use

1. **Open the assembly**  
   `CMM Arm Full Assembly.SLDASM`

2. **Choose a probe**  
   Suppress/unsuppress or replace:
   - `Probe 1 Dia 6.SLDPRT`
   - `Probe 2 Dia 1.SLDPRT`
   - `Probe 3 Dia 2.SLDPRT`
   - `Probe 4 Dia 4.SLDPRT`  
  

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

## Note
This is a **geometric clearance check**. Dynamics and probe triggering not included.  


---

## License

Released under the **MIT License**.  
Forks, adaptations, and improvements are welcome.

---

## Credits

Modeling, probe library, and example parts by **Seif Adly**.  
Not affiliated with Renishaw®, Aberlink®, or SOLIDWORKS®. Trademarks belong to their respective owners.
