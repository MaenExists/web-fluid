# Standardized Testing Protocol: Web Strand Characterization

To systematically compare formulations and quantify performance across iterations (V1 through V5+), all tests must follow this reproducible benchtop evaluation standard.

---

## 1. Test Setup & Equipment

### 1.1 The Gap-Bridging Test Rig
- **Rig Specifications:** Two vertical wooden dowels, metal rods, or notched cardboard uprights mounted to a flat base.
- **Fixed Spans:** 
  - Standard Gap: **15 cm (6 in)**
  - Extended Gap: **30 cm (12 in)**
- **Target Distance:** The atomizer nozzle is positioned at a fixed distance of **50 cm (20 in)** from the plane of the gap, spraying horizontally.

```
       [ Atomizer Nozzle ]
              │
              │  ◄──── Fixed Distance: 50 cm ────►
              ▼
         ═══════════════════════════════════════════
               │                             │
               │◄────── Fixed Gap: 15 cm ───►│
            [ Post A ]                    [ Post B ]
```

---

## 2. Quantitative & Qualitative Metrics

### Metric 1: Fiber Cohesion & Morphology (Visual Rating)
Inspect the sprayed material immediately after flight under direct lighting:

| Grade | Morphology Class | Description | Physical Meaning |
|---|---|---|---|
| **M0** | **Discrete Droplets** | Wet mist/splatter, zero fibers. | Polymer concentration too dilute ($c < c^*$). No chain overlap. |
| **M1** | **Beads-on-String** | Droplets connected by thin, fragile threads. | Semi-dilute unentangled ($c^* < c < c_e$). High capillary pinching. |
| **M2** | **Continuous Web** | Multi-fibrillar interconnected web network bridging posts. | Entangled regime ($c > c_e$). Extensional viscosity arresting breakup. |
| **M3** | **Single Monofilament** | Cohesive, rope-like central strand with minimal stray mist. | High-entanglement, optimized nozzle shear. |

### Metric 2: Flash-Off Speed (Tack-Free Time)
- Using a dry wooden toothpick or silicone probe, gently touch the center of the bridged strand at $1\text{s}$, $3\text{s}$, $5\text{s}$, and $10\text{s}$ post-spray.
- **Record:** Time (seconds) until the probe pulls away cleanly with zero liquid transfer or tack.
  - Target: **$< 2 \text{ seconds}$** for true in-flight phase inversion.

### Metric 3: Tensile Ductility & Snap Test (Hand-Pull)
Gently pinch the center of the span between thumb and forefinger and pull axially until fracture:

| Rating | Classification | Elongation at Break | Tactile Sensation |
|---|---|---|---|
| **D1** | **Glassy / Crumbly** | $< 5\%$ | Shatters like dried styrofoam / glass dust. Zero yield. (V1 Polystyrene Baseline) |
| **D2** | **Leathery / Yielding** | $10\text{–}30\%$ | Stretches slightly, then shears cleanly. Minimal snapback. |
| **D3** | **Ductile / Elastic** | $50\text{–}150\%$ | Distinct rubbery tension, notable elastic recovery before breaking. |
| **D4** | **High-Toughness / Fiction-Like** | $> 150\%$ | Significant resistance to pull; requires two-hand force or blade to sever. |

### Metric 4: Static Mass-Hold Test (Payload Capacity)
For strands that successfully bridge the 15 cm gap:
1. Place a light wire hook onto the center of the suspended strand.
2. Incrementally add standard test masses until tensile failure:
   - **Tier 1:** Standard paperclip ($~1.0\text{ g}$)
   - **Tier 2:** Plastic bottle cap ($~5.0\text{ g}$)
   - **Tier 3:** AA Battery ($~23.0\text{ g}$)
   - **Tier 4:** $50\text{ g}$ lab weight or small screwdriver
3. **Record:** Maximum sustained load (grams) before strand snaps or peels off anchor posts.

---

## 3. Standardized Test Log Template

When executing tests, copy and complete this entry block in the corresponding log file:

```markdown
### Batch Run: [e.g., V2-A (10 wt% PVAc in Acetone)]
- **Date / Ambient Temp / Humidity:** [e.g., 2026-09-11 / 22°C / 45% RH]
- **Polymer:** [e.g., Dry PVAc confetti from Elmer's Glue-All]
- **Solvent:** [e.g., Pure Acetone]
- **Polymer Mass / Solvent Mass:** [e.g., 3.0 g PVAc in 27.0 g Acetone = 10% w/w]
- **Delivery System:** [e.g., Fine mist perfume atomizer, 0.4 mm orifice]
- **Spray Distance:** [50 cm]
- **Visual Morphology (M0-M3):** [ ]
- **Tack-Free Time:** [ s]
- **Ductility Rating (D1-D4):** [ ]
- **Max Mass Held:** [ g]
- **Failure Mode / Observations:** [e.g., Droplets formed; nozzle clogged after 2 pumps; strands snapped under 1g load]
```
