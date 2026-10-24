# Protocol: 4D-Printed Reversible Shape-Memory Polymers

*Prepared 2026-10-24*

## Overview

This protocol rebuilds the experimental workflow of Natali et al., *4D-printing of thermo- and photo-activated reversible stress-free shape-memory polymers*, European Polymer Journal 260 (2026) 115160 ([doi:10.1016/j.eurpolymj.2026.115160](https://doi.org/10.1016/j.eurpolymj.2026.115160)). All quantities and settings come from the paper's Experimental section; supporting-information details are not included.

**Aim:** make photo-crosslinkable PCL-PBS-PCL dimethacrylate blends, pick the blend with the best stress-free two-way shape-memory effect, add TiN nanoparticles for light activation, and print actuators by Fused Particle Fabrication (FPF).

**Workflow (paper's Scheme 2):**

1. Synthesize PBS diol (Mn ≈ 4 kDa).
2. Grow PCL blocks by ring-opening polymerization to make CPCL_3 (PCL blocks ≈ 3 kDa) and CPCL_9 (≈ 9 kDa).
3. End-cap both with methacrylate groups using 2-IEM.
4. Blend CPCL_9 and CPCL_3 (Mix_A, Mix_B, Mix_C) and make photo-crosslinked films.
5. Run stress-free shape-memory tests and select the best blend (Mix_A).
6. Load Mix_A with 0.4 wt% TiN nanoparticles.
7. 3D-print thermo- and photo-responsive specimens, grippers and stents, then characterize.

## Materials and equipment

All reagents were used as received unless noted.

| Reagent | Supplier | Use / note |
| --- | --- | --- |
| Dimethyl succinate | Sigma-Aldrich | PBS monomer |
| 1,4-Butanediol | Sigma-Aldrich | PBS monomer (15 % molar excess) |
| Titanium(IV) butoxide, 97 % | Sigma-Aldrich | PBS catalyst |
| ε-Caprolactone (CL), 97 % | Merck | Distill under reduced pressure over CaH2 and molecular sieves before use |
| Tin(II) 2-ethylhexanoate, Sn(Oct)2 | Sigma-Aldrich | ROP catalyst |
| Calcium hydride, CaH2 | Sigma-Aldrich | Drying agent for CL |
| 2-Isocyanatoethyl methacrylate (2-IEM), 98 % | Sigma-Aldrich | Methacrylation |
| Chloroform | Sigma-Aldrich | Solvent for casting |
| Additol HDMAP (2-hydroxy-2-methyl-1-phenyl propanone) | Cytec | Radical photoinitiator |
| TiN nanoparticles, cubic, 20 nm | Nanografi | Photothermal filler |
| Hexanoic acid | Not stated | NP dispersant |
| Ethanol | Not stated | Hot extraction of printed parts |

| Equipment | Model | Purpose |
| --- | --- | --- |
| 3D printer | EnvisionTEC BP3 3D-Bioplotter, high-temperature head + 365 nm UV module | FPF printing |
| CAD / slicer | Rhino 3D (.stl) → Prefactory Suite (.bpl) | Part design |
| FT-IR | PerkinElmer Spectrum Two, ATR | Isocyanate check |
| NMR | Bruker 700 MHz, CDCl3 | Mn and methacrylation degree |
| DSC | Netzsch DSC 204 | Thermal properties |
| Rheometer | Haake Mars, cone-plate 35 mm, 2° | Melt viscosity |
| SEM / EDX | Zeiss Supra 40VP; Oxford Ultim Extreme 100 | Morphology, NP dispersion |
| WAXD | Bruker D8 Discover, Hi-Star detector | Crystal orientation |
| Tensile tester | Zwick Roell Z005 with thermal chamber | Mechanics and shape memory |
| Solar simulator | LOT-Oriel LS0306, 322 W xenon arc, AM1.5G filter | Photo-activation |
| Thermal camera | InfraTec VarioCAM | Surface temperature |
| Spectrometer | Ocean Insight RS2000XR with CC-3-DA cosine corrector | Irradiance calibration |
| Image analysis | ImageJ 1.53t | Elongation and bending angles |

## Synthesis

### Step 1: PBS diol (Mn ≈ 4 kDa), two-step bulk polymerization

1. Add 58.5 g dimethyl succinate (0.40 mol) and 41.5 g 1,4-butanediol (0.46 mol, 15 % excess) to a 250 mL three-neck round-bottom flask.
2. Stir magnetically under nitrogen and heat to 160 °C.
3. Add 0.068 g titanium(IV) butoxide (0.20 mmol). Run transesterification for 2 h at 160 °C.
4. Raise to 240 °C, add another 0.068 g titanium(IV) butoxide (0.20 mmol), and apply vacuum.
5. Polycondense for 1 h under vacuum. Do not purify.
6. Confirm Mn by 1H NMR (Equation 1).

### Step 2: PCL-PBS-PCL triblocks by ring-opening polymerization

CL monomer is initiated by the PBS diol hydroxyl ends. Vary the CL amount to set the PCL block length: about 3 kDa (CPCL_3) or 9 kDa (CPCL_9).

1. Dry PBS diol at 60 °C under vacuum overnight.
2. Example (CPCL_9): place 3.40 g PBS diol (0.86 mmol) in a three-neck flask with a mechanical stirrer and melt at 130 °C.
3. Add 16.4 g freshly distilled CL (144 mmol) and 0.020 g Sn(Oct)2 (0.1 wt%).
4. React at 130 °C under nitrogen overnight.
5. Confirm PCL block Mn by 1H NMR (Equation 2).

### Step 3: Methacrylation with 2-IEM (one pot, bulk)

1. Keep the hydroxy-terminated triblock at 115 °C under nitrogen with mechanical stirring.
2. Add 2-IEM dropwise at 20 % molar excess over the hydroxyl groups.
3. React for 3 h at 115 °C.
4. Remove unreacted 2-IEM under dynamic vacuum.
5. Check by FT-IR that the isocyanate band at 2275 cm⁻¹ is gone.
6. Confirm degree of methacrylation by 1H NMR (Equation 3). The paper reports DM ≥ 97–98 % for all materials.

## Formulations and photo-crosslinked films

### Blend compositions (paper's Table 1)

| Sample | CPCL_9 (wt%) | CPCL_3 (wt%) | CL:BS (w/w) |
| --- | --- | --- | --- |
| CPCL_9 | 100 | 0 | 82:18 |
| Mix_A | 75 | 25 | 76:24 |
| Mix_B | 50 | 50 | 71:29 |
| Mix_C | 25 | 75 | 65:35 |
| CPCL_3 | 0 | 100 | 60:40 |

### Step 4: Neat crosslinked films

1. Dissolve the dimethacrylated CPCL_9 and CPCL_3 in chloroform in the Table 1 ratio.
2. Add Additol HDMAP at 0.5 wt%.
3. Cast into a Petri dish. Evaporate overnight at room temperature in a fume hood, in the dark.
4. Melt the dried film at 130 °C and pour into a hot mold: two glass plates (25 × 75 mm) with PTFE spacers 0.2–0.3 mm thick.
5. Photo-crosslink on a hot plate at 130 °C under a 365 nm UV lamp (≈ 2 mW cm⁻²) held 2 cm from the sample.
6. Irradiate each side for 5 min.

**For printing feedstock:** prepare the uncrosslinked film the same way but with 1 wt% photoinitiator. Shred it and store in the dark at −20 °C.

### Step 5: TiN-loaded photo-responsive formulation (Mix_A_TiN)

Targets: TiN 0.4 wt% of the formulation; hexanoic acid : TiN = 45 : 1 (w/w); photoinitiator 3 wt%.

1. Put 25 mg TiN nanoparticles in a flask with 50 mL chloroform and 1.125 g hexanoic acid.
2. Sonicate for 5 min until the dispersion is homogeneous.
3. Add 1.25 g CPCL_3 and 3.75 g CPCL_9 (the Mix_A ratio) and 0.2 g Additol HDMAP. Stir until dissolved.
4. Solvent-cast in a Petri dish and evaporate overnight in a fume hood, in the dark.
5. For films: photo-crosslink exactly as in Step 4.
6. For printing: shred the uncrosslinked film and store in the dark at −20 °C.
7. Before printing, remove the hexanoic acid by heating the uncrosslinked formulation at 80 °C for 4 h. Confirm by 1H NMR. This restores the melt viscosity to near that of neat Mix_A (product called Mix_A_TiN_Treatment).

## 3D printing by Fused Particle Fabrication

### Step 6: Prepare and load

1. Design parts in Rhino 3D, export as .stl, and convert to .bpl in Prefactory Suite.
2. Load the shredded photo-crosslinkable feedstock into the high-temperature cartridge of the BP3 Bioplotter.

### Step 7: Print and crosslink layer by layer

Print at 100 °C (chosen from DSC and rheology) on a bed at room temperature. Crosslink each layer immediately after it is extruded.

| Setting | Neat Mix_A (thermo-responsive) | Mix_A_TiN (photo-responsive) |
| --- | --- | --- |
| Head temperature | 100 °C | 100 °C |
| Bed temperature | Room temperature | Room temperature |
| Pressure | 3.5 bar | 3.5–4.0 bar |
| Speed | 4 mm s⁻¹ | 3–7 mm s⁻¹ |
| Offset and line spacing | 0.5 mm | 0.5–0.7 mm |

**UV module (all prints):** 96 mW cm⁻², 15 mm above the last layer, moving at 1 mm s⁻¹, 6.9 mm light spot.

**TiN print variants (paper's Table 7):**

| Sample | Pressure (bar) | Speed (mm s⁻¹) | Offset (mm) | Thickness (mm) | Gel content (%) |
| --- | --- | --- | --- | --- | --- |
| 3D_TiN_1 | 3.5 | 7 | 0.5 | 0.12–0.14 | 76.0 ± 0.4 |
| 3D_TiN_2 | 3.5 | 5 | 0.7 | 0.25–0.28 | 71.0 ± 0.3 |
| 3D_TiN_3 | 4.0 | 3 | 0.5 | 0.50–0.60 | 20.0 ± 0.6 |

Thinner prints crosslink better because TiN absorbs UV, so 3D_TiN_1 was used for testing.

### Step 8: Specimens and demonstrators

- **Dog-bones, monolayer:** raster angles 0° (3D_0), 45° (3D_45) and 90° (3D_90) relative to the load direction.
- **Dog-bones, multilayer:** bilayer (3D_0_2) and trilayer (3D_0_3) at 0°.
- **Four-arm gripper:** thermo-activated open–close demonstrator.
- **Stents:** printed on a rotating mandrel. The built-in UV module could not be used here, so crosslink in a separate step afterwards. Program in a compressed shape to show self-expansion above Tm,PBS.

## Characterization methods

| Method | Conditions |
| --- | --- |
| FT-IR (ATR) | 32 scans, 4 cm⁻¹ resolution |
| 1H NMR | 700 MHz, CDCl3, referenced to TMS at 0 ppm |
| Gel content | Films 20 × 20 × 0.4 mm and dog-bones (35 mm long, 5 mm wide, 0.3–1 mm thick); soak in chloroform overnight at room temperature; dry to constant weight |
| DSC | Under N2: heat −100 → 160 °C, cool to −100 °C, reheat to 160 °C, all at 10 °C min⁻¹; crystallinity from the second heating |
| Rheology | Frequency sweep 0.1–20 Hz at 1.0 Pa shear stress, 0.2 mm gap, at 100, 110 and 120 °C |
| SEM / EDX | 3 kV; iridium or carbon sputter coat; ETD, BSED and EDX detectors |
| WAXD | Cu anode, 40 kV / 40 mA, λ = 0.15418 nm, 0.8 mm collimator, 150 mm sample–detector distance, detector at 2θ = 25° (range 7.2–43.5°), 300 s exposure; fit peaks with Pearson VII in TOPAS |
| WAXD sample states | Pristine; programmed and fixed at 200 % strain; equilibrated stress-free at Tact then cooled to room temperature |
| Photothermal | Xenon solar simulator with AM1.5G filter (≈ 200–2500 nm); irradiance 1463 W m⁻² (200–1020 nm) at 40 mm working distance; temperature tracked with a thermal camera |

### Equations

**Eq. 1, PBS molecular weight** (90 Da = butanediol end unit, 172 Da = BS repeat unit):

$$M_n(\mathrm{PBS}) = 90 + \frac{A_{4.10}}{A_{3.66}} \times 172$$

**Eq. 2, PCL block molecular weight** (114 Da = CL repeat unit):

$$M_n(\mathrm{PCL\ block}) = \frac{A_{2.35}}{A_{2.62}} \times DP_{\mathrm{PBS}} \times 114$$

**Eq. 3, degree of methacrylation** (3.50 ppm = urethane CH2 next to N; 3.64 ppm = CH2 next to unreacted OH):

$$DM\,(\%) = \frac{A_{3.50}}{A_{3.50} + A_{3.64}} \times 100$$

**Eq. 4, gel content** (m_d = dried mass after extraction, m_0 = initial mass):

$$G = \frac{m_d}{m_0} \times 100$$

**Eq. 5, crystallinity** from the second DSC heating (ΔH⁰ = 200 J g⁻¹ for PBS, 134.9 J g⁻¹ for PCL):

$$\chi_c = \frac{\Delta H_{m,i}}{\Delta H^{0}_{m,i}} \times 100$$

## Mechanical and shape-memory testing

### Step 9: Tensile tests

1. Test printed dog-bones (30 mm long, 5 mm wide, 0.3–1 mm thick) at room temperature on the Zwick Z005.
2. Use 0.02 N preload and 5 mm min⁻¹ until failure.
3. Take Young's modulus from the slope at 0.5–2 % strain.
4. Test at least 4 replicates. Report mean ± SD and compare groups with Welch's t-test (two-tailed, α = 0.05).

### Step 10: Thermally activated two-way stress-free shape memory

Run on the Zwick Z005 with its thermal chamber.

1. Heat the sample to 110 °C and hold 5 min.
2. Stretch to 100 % strain at 5 mm min⁻¹.
3. Cool to −20 °C at 2 °C min⁻¹ while holding the strain.
4. Release the strain and keep the sample quasi-stress-free (0.05 N preload).
5. Cycle between Tact = 55 °C and −20 °C at 2 °C min⁻¹. Run at least 4 cycles (the paper shows 5).
6. Calculate εrev, ε′rev and Qef as the average of cycles 2–5. Report mean ± SD; compare with Welch's t-test.
7. Heating above Tm,PBS recovers the original permanent shape.

Tact = 55 °C fully melts the PCL (actuating) crystals while leaving most PBS (skeleton) crystals intact.

**Eq. 6, reversible elongation:**

$$\varepsilon_{rev} = \frac{l_{max} - l_{min}}{l_0} \times 100$$

**Eq. 7, relative reversible elongation:**

$$\varepsilon'_{rev} = \frac{l_{max} - l_{min}}{l_{min}} \times 100$$

**Eq. 8, deformation fixation efficiency:**

$$Q_{ef} = \frac{\varepsilon_{min}}{\varepsilon_{pr}} \times 100$$

Here l_max and l_min are the longest and shortest sample lengths in the stress-free cycles, l_0 is the initial length, ε_pr is the programmed strain (100 %), and ε_min is the lowest strain reached on heating to Tact. Measure lengths and gripper bending angles with ImageJ.

### Step 11: Photo-activated shape memory

1. Thermally program a crosslinked Mix_A_TiN film to 100 % strain (Step 10, steps 1–4).
2. Irradiate with the solar simulator; record surface temperature with the thermal camera.
3. Switch the light off and let the sample cool to room temperature.
4. Repeat on/off cycles and measure the reversible elongation.

Expected: the film reaches 55 °C in about 20 s and plateaus near 65 °C after 1 min. With the light off it drops to about 40 °C in 15 s and reaches room temperature within the next 45 s. A neat Mix_A control shows no significant heating.

## Post-treatment, key results and notes

### Step 12: Extraction of uncrosslinked chains (TiN samples)

TiN absorbs UV and lowers the gel content, which weakens actuation. Removing the soluble fraction restores it.

- **Films (Mix_A_TiN):** soak overnight in a chlorinated solvent.
- **Printed parts (3D_TiN_1):** soak in ethanol at 75 °C for 4 h. Ethanol is a marginal solvent for polyesters, so it extracts without the swelling damage chloroform causes.
- Photothermal response is unchanged after extraction.

### Key results to expect

| Sample | εrev (%) | ε′rev (%) | Qef (%) | Gel content (%) |
| --- | --- | --- | --- | --- |
| Mix_A film | 22.8 ± 0.3 | 14.5 ± 0.2 | 45.5 ± 1.1 | 88 ± 1 |
| Mix_B film | 19.5 ± 0.5 | 11.6 ± 0.4 | 67.8 ± 1.4 | 91 ± 1 |
| CPCL_9 film | 12.6 ± 1.2 | 9.7 ± 1.0 | 29 ± 1.5 | 88 ± 3 |
| Mix_C film | 4.3 ± 0.1 | 2.3 ± 0.1 | 84.2 ± 0.3 | 90 ± 2 |
| CPCL_3 film (single test) | 2.5 | 1.2 | 79 | 95.0 ± 0.5 |
| Mix_A_TiN film | 11.4 ± 0.5 | 6.0 ± 0.3 | 88.3 ± 2.5 | 74 ± 3 |
| Mix_A_TiN film, extracted | 19.7 ± 0.2 | 12.4 ± 0.1 | 59.3 ± 0.2 | — |
| 3D_0 print (Mix_A) | 6.6 ± 0.9 | 3.6 ± 0.8 | 81 ± 1 | 82 ± 1 |
| 3D_TiN_1 print | 3.9 ± 0.5 | 2.0 ± 0.3 | 92.8 ± 1.3 | 76.0 ± 0.4 |
| 3D_TiN_1 print, extracted | 15.5 ± 0.5 | 8.5 ± 0.3 | 81.9 ± 0.9 | — |

Mix_A was chosen because it gives the highest reversible elongation. Photo-activated cycling of a Mix_A_TiN film gave εrev ≈ 10 %, close to thermal activation. The printed gripper reversibly moved about 13°.

### Notes

- Printed parts actuate less than films because they are crosslinked at room temperature, not in the melt at 130 °C. That is needed for shape fidelity but gives lower gel content and more PBS crystallinity.
- Raster angle and layer number had no significant effect on εrev (p ≥ 0.05).
- Only 5 cycles were tested. The paper notes long-term cycling and aging were not evaluated.
- Exact printing optimization (paper's Figs. S5–S6) and other supporting-information details are not covered here.
