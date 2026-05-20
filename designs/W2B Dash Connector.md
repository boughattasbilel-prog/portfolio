### W2B Dash Connector Project 

Design and develop a compact **Wire-to-Board (W2B) high-density automotive connector** for dashboard integration — from concept phase through pre-series, meeting automotive qualification requirements.

---

### Objective

**Key targets:**
- Achieve high pin density within a constrained PCB footprint
- Ensure reliable mating/unmating force and secondary locking robustness under automotive conditions
- Optimize housing geometry for plastic injection moldability (DFM)
- Support integration in a complex dashboard harness environment
- Validate the design through simulation, analysis, and cross-functional review

---

## My Ownership & Contributions

> The following reflects my **direct personal contributions** to this project. This is not a team summary — it is what I personally owned, drove, and delivered.

### 🔩 3D Design — NX Siemens (Full Ownership)
- Owned the full 3D connector housing geometry from blank sketch to pre-series model
- Designed the **primary and secondary locking features** — geometry, draft angles, and interference fit
- Modeled complex multi-body assemblies (housing, TPA, CPA, pin interfaces) and managed all mating constraints
- Produced **2D drawings with GD&T** callouts — directly used in manufacturing reviews

### 📐 Tolerance Analysis (Direct Contribution)
- Performed dimensional tolerance stack-ups on the mating interface to verify assemblability
- Identified critical clearance conditions between pin and housing that risked mis-mating
- Coordinated with metrology team to align drawing callouts with control plan requirements

### 🧪 FEA — Structural Simulation (Active Participation)
- Built analytical models to estimate stress and deflection on the locking arm geometry
- Reviewed FEA results and used simulation output to drive geometry iterations
- Identified stress concentration zones in the secondary lock that led to a geometry change

### 🏭 Moldflow & DFM (Direct Analysis)
- Interpreted Moldflow analyses on the housing — validated injection assumptions
- Identified weld line risk zones near the locking features and recommended gate relocation
- Recommended DFM improvements: rib thickness adjustments, corner radii, wall uniformity
- Coordinated with tooling supplier to implement DFM feedback before mold cut

### ⚙️ Material Selection (Contributed Decision)
- Evaluated material candidates for the housing — assessed structural behavior vs. moldability trade-off
- Supported the decision between **LCP** and **PBT GF30** based on stiffness, shrinkage, and cost
- *(Safe to disclose: material names are not proprietary on their own)*

### 📋 DFMEA & Quality (Support Role)
- Participated in DFMEA sessions — contributed failure mode identification for locking and pin interface
- Proposed corrective actions on 2 critical risk items (locking breakage, pin back-out)
- Interfaced directly with manufacturing and quality teams to resolve non-conformities during pre-series

---

## Tools & Methods

| Tool / Method | My Usage |
|---|---|
| **NX Siemens** | Primary 3D CAD tool — housing, assembly, 2D drawings |
| **FEA (structural)** | Locking feature stress and deflection validation |
| **Moldflow** | Injection analysis, weld line mapping, DFM recommendations |
| **ISO GPS / GD&T** | Functional dimensioning on all 2D manufacturing drawings |
| **DFMEA** | Failure mode identification and risk reduction |
| **Siemens Teamcenter (PDM)** | Data management, revision control, release workflow |
| **PPAP support** | Pre-series documentation and supplier coordination |

---

## Engineering Challenge

The central challenge was **packaging a high pin count into a minimal PCB footprint** while keeping the secondary locking system mechanically robust under automotive vibration, thermal cycling, and repeated mating/unmating.

The locking arm geometry was too thin in the initial concept — FEA confirmed high stress concentration at the base of the latch. Resolving this required a design iteration that:
1. Increased the latch root radius without violating the housing envelope
2. Changed wall thickness locally to improve stiffness-to-weight
3. Adjusted draft angles to remain compatible with the injection mold direction

Simultaneously, Moldflow showed a weld line forming directly across the locking feature — a critical risk for brittle fracture. Gate position was relocated to push the weld line to a non-critical zone.

---

## Results

- ✅ Delivered a robust connector concept — validated by FEA and design review before pre-series
- ✅ Eliminated locking fracture risk through geometry iteration driven by simulation
- ✅ Moldflow-driven DFM changes adopted in final tooling — weld line repositioned successfully
- ✅ GD&T drawings released and used in manufacturing control plan
- ✅ DFMEA risk items reduced from critical to acceptable through design action

---

## Project Media

![W2B Dash Connector](https://user-gen-media-assets.s3.amazonaws.com/gpt4o_images/288332ea-5e98-497a-ac1a-8e76eeaed9c3.png)
