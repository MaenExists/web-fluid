# DIY "Web Shooter" Fluid Development

A methodical, engineering-driven project to develop a sprayable polymer fluid that forms cohesive, rapid-solidifying web-like strands in mid-air via flash-evaporative solution blow spinning.

---

## 🕷️ Project Vision & Goal
The objective is to synthesize and atomize a polymer-solvent fluid inspired by fiction (Spider-Man web fluid) that achieves:
1. **In-Flight Phase Change:** High-volatility solvent flashes off during aerodynamic transit.
2. **Strand Cohesion:** Elastic, continuous micro-fibers form instead of discrete droplet mist (suppressing Rayleigh-Plateau instability).
3. **Mechanical Utility:** Fibers strong and ductile enough to bridge gaps and support lightweight loads, improving incrementally across iterations.

---

## 🔬 Core Physical & Chemical Mechanism
The fluid operates on the principles of **Solution Blow Spinning / Flash Evaporation Spinning**:
```
[Polymer in High-Vapor-Pressure Solvent] 
                  │
                  ▼ (Pressure Discharge through Orifice)
[Viscoelastic Liquid Jet / Filament] 
                  │
                  ├── Extensional strain pulls polymer chains into alignment
                  └── Solvent flashes rapidly into the surrounding air
                  │
                  ▼
[Solidified Tensile Polymer Strand / Web Network]
```

To form a continuous fiber rather than a cloud of droplets:
- **Chain Entanglement ($c > c_e$):** Polymer concentration must exceed the entanglement threshold so molecular chains interlock and resist capillary breakup.
- **Extensional Viscosity:** The fluid must exhibit strong resistance to stretching (strain hardening), allowing aerodynamic drag to pull it into a filament.
- **Flash-Off Kinetics:** The solvent's vapor pressure must be high enough to drop the jet below the gel/glass transition point within milliseconds of flight.

---

## 🗺️ Iteration Roadmap

| Iteration | Polymer System | Solvent System | Additives | Key Focus / Milestone |
|---|---|---|---|---|
| **V1** | Polystyrene (EPS) | Acetone | None | *Proof of Concept:* Proved strand formation; brittle crumbly fibers due to glassy $T_g \approx 100^\circ\text{C}$. |
| **V2** *(Current)* | Polyvinyl Acetate (PVAc) | Acetone / Ethyl Acetate | None | *Ductility & Extraction:* Extract clean PVAc from emulsion glue; establish concentration curve; benchmark toughness vs V1. |
| **V3** | PVAc | Acetone | Plasticizer (Glycerin / Triacetin) | *Elongation & Adhesion:* Tune $T_g$ downward to prevent snap brittleness and improve surface grab. |
| **V4** | PVAc + Polystyrene Alloy | Acetone / Co-solvent | Plasticizer | *Tensile Reinforcement:* Polymer blend balancing PVAc elasticity with PS rigid backbone. |
| **V5+** | Hybrid Polymer Matrix | Optimized Fast-Flash | Micro-reinforcements / Tackifiers | *Advanced Performance:* Explore crosslinkers, cellulose microfibers, delivery mechanics (pressurized coaxial gas nozzles). |

---

## ⚠️ Safety Protocols
Working with volatile organic solvents (acetone, ethyl acetate, thinners) poses distinct chemical hazards:
1. **Flammability:** Acetone flash point is $-20^\circ\text{C}$ ($-4^\circ\text{F}$); ethyl acetate flash point is $-4^\circ\text{C}$ ($25^\circ\text{F}$). **Never operate near open flames, sparks, heaters, or unrated electrical switches.**
2. **Vapor Inhalation:** Work exclusively in well-ventilated outdoor areas or under an active fume extraction hood. Use a half-face respirator with **organic vapor (OV) cartridges** (e.g., 3M 6001/6003). Dust masks do NOT block solvent vapors.
3. **Eye & Skin Protection:** Always wear chemical splash goggles and solvent-compatible gloves (Butyl rubber or heavy Nitrile; note that thin disposable nitrile degrades quickly in acetone).
4. **Pressure Safety:** Never pressurize glass vessels. Use only solvent-rated metal or HDPE/PP plastic spray reservoirs.

---

## 📁 Repository Structure
```
web-fluid/
├── README.md                      # Project overview, core physics, roadmap, safety
├── docs/
│   ├── RESEARCH.md                # Polymer physics, rheology, thermodynamics, extraction chemistry
│   ├── EXTRACTION_PROTOCOLS.md    # Practical bench guide: extracting dry PVAc from white glue
│   ├── FORMULATIONS.md            # Recipe book and batch composition matrix
│   ├── TESTING_PROTOCOL.md        # Standardized tensile, hang, and airborne flight metrics
│   └── LOGS/
│       ├── V1_POLYSTYRENE.md      # V1 test run, observation data, and failure analysis
│       └── V2_PVAC.md             # V2 test execution plan, concentration series, and bench log
```
