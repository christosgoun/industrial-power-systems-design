# Industrial Power Systems Design & Engineering (Flour Mill Facility)

This repository contains the complete 5-phase electrical engineering study and design for a large-scale industrial flour mill facility. The project was developed as part of the advanced curriculum in **Electrical Power Engineering** at the **Aristotle University of Thessaloniki (AUTh)**.

The study delivers a comprehensive grid-connected industrial design, fully compliant with **ELOT HD 60364**, **IEC 60909**, **CENELEC HD384**, and Greek national regulations (FEK B 1222/2006).

---

## Project Structure & Deliverables

### 1. Load Estimation & Agreed Power Determination (Deliverable 1)
* **Scope:** Evaluation of total installed power for cage induction motors and auxiliary loads.
* **Key Methodology:** Applied coincidence/simultaneity factors ($k_s = 0.72$) and a 10% future expansion margin. Calculated the initial uncompensated power factor ($\cos\phi = 0.842$) to determine the total required apparent power of **1218.16 kVA** for utility contract negotiation with HEDNO (ΔΕΔΔΗΕ).

### 2. Grounding System Selection & Design (Deliverable 2)
* **Scope:** Grounding grid engineering for human safety, fault current mitigation, and equipment protection.
* **Key Methodology:** * Comparative analysis of earthing topologies (IT, TT, TN-C); selection of **TN-S** for optimal low-voltage protection.
  * Structural foundation grounding design according to FEK B 1222/2006.
  * Calculation of grounding resistance using equivalent circular electrode modeling ($R_A \approx 0.506\ \Omega$ for the main complex).
  * Equipotential bonding and touch voltage mitigation inside the MV/LV substation using floor meshes and dedicated ring busbars.

### 3. Cable Sizing & Routing Optimization (Deliverable 3)
* **Scope:** Ampacity sizing and voltage drop optimization for low-voltage (LV) distribution lines from the Main LV Switchboard (MLVS) to process sub-panels.
* **Key Methodology:**
  * Thermal current-carrying capacity sizing adjusted for $40^{\circ}\text{C}$ ambient conditions (CENELEC HD384).
  * Multi-variable iterative cross-section corrections ensuring total voltage drop ($\Delta u$) remains strictly $\le 4\%$ under full load conditions.
  * Cable containment design using perforated cable trays for indoor routing and rigid concrete conduits for underground runs.

### 4. Motor Control & Protection Coordination (Deliverable 4)
* **Scope:** Sizing of motor starting equipment and selective protection coordination.
* **Key Methodology:**
  * Starting methods evaluation: Direct-On-Line (DOL) for low-power auxiliary drives; **Soft Starters** for high-inertia process motors to limit inrush currents to $4 \times I_n$.
  * Protection scheme design featuring high-breaking-capacity fuses and Miniature Circuit Breakers (MCBs) calibrated against motor time-current curves to ensure selective coordination.
  * Implementation of Type B Residual Current Devices (RCDs) rated at $300\text{ mA}$ to handle power electronics harmonics without nuisance tripping.

### 5. Substation Engineering & Power Factor Correction (Deliverable 5)
* **Scope:** Design of the indoor 20/0.4 kV step-down distribution substation.
* **Key Methodology:**
  * Selection of a **1250 kVA cast-resin dry-type transformer** (6% short-circuit impedance $u_k$) suitable for hazardous dust environments.
  * Primary MV connections utilizing single-core $50\text{ mm}^2$ XLPE cables (2XSY 12/20kV) and main LV bus-ties using 18 single-core parallel $120\text{ mm}^2$ PVC copper cables per phase.
  * Integration of a two-tier Reactive Power Compensation system: **Fixed compensation** ($90\text{ kVAR}$) for transformer no-load losses and an **automatic central capacitor bank** ($8 \times 40\text{ kVAR}$) to maintain a utility-side $\cos\phi \ge 0.95$.
  * Specification of Air-Insulated Switchgear (AIS) with visible-break load break switches (LBS), earth switches, mechanical interlocks, and auxiliary UPS systems.

---

## Engineering Stack & Tools
* **CAD & Layouts:** AutoCAD (Single-Line Diagrams, Substation Layouts, Grounding Grids)
* **Computation:** MATLAB / Microsoft Excel (Iterative cable sizing, short-circuit current analysis, reactive power calculations)
* **Standards Compliance:** ELOT HD 60364, IEC 60909, CENELEC HD384, FEK B 1222/2006

---

## Team & Acknowledgments
Developed by **Team 7** (AUTh ECE - Electrical Power Engineering Section):
* **Christos Gounaris** 
* Georgios Xerogiannakis 
* Georgios Eftychiakos
