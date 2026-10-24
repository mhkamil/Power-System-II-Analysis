# Solved Math Bank: all repeated numericals with full answers

> Every answer below was re-calculated and checked. Write the **given → formula → substitution → answer** steps in the exam exactly like this.
> r′ = 0.7788 r · k = ε₀ε<sub>r</sub> · ε₀ = 8.854×10⁻¹² F/m · ln = natural log · log = log₁₀

---

## PART 1: Inductance (Ch-2)

### M4 ⭐⭐⭐⭐⭐ Bundled ACSR Pheasant (F21, F22, F24a, Stevenson 4.5)
*Each conductor of the bundled line is ACSR 1,272,000-cmil Pheasant. d = 45 cm, phase spacing 8 m (a–b–c in a row). Find X<sub>L</sub> per km and per mile; also per-unit for 160 km, base 100 MVA, 345 kV (60 Hz).*

- From table A.3: D<sub>s</sub> (GMR) of Pheasant = 0.0466 ft = 0.0466 × 0.3048 = **0.0142 m**
- Bundle GMR: D<sub>s</sub><sup>b</sup> = √(D<sub>s</sub> · d) = √(0.0142 × 0.45) = **0.0799 m**
- D<sub>eq</sub> = ∛(8 × 8 × 16) = **10.08 m**
- X<sub>L</sub> = 2πf · 2×10⁻⁷ ln(D<sub>eq</sub>/D<sub>s</sub><sup>b</sup>) × 1000 = 2π(60)(2×10⁻⁴) ln(10.08/0.0799)
- **X<sub>L</sub> = 0.365 Ω/km = 0.587 Ω/mile**
- Z<sub>base</sub> = 345²/100 = 1190.25 Ω; X = 0.365 × 160 = 58.4 Ω → **X<sub>pu</sub> = 0.049 pu**
- (If the paper says 50 Hz: 0.304 Ω/km.)

### M9 ⭐⭐⭐⭐ 500 kV line, 2-conductor bundle (F22 1d, TT-1 21-22; Kothari Ex 2.9)
*Bundle spacing 0.5 m, conductor diameter 30 mm, phase spacing 15 m (a–b–c in a row), 50 Hz, each conductor carries 50 % current.*

- r = 15 mm → r′ = 0.7788 × 0.015 = 0.01168 m
- D<sub>s</sub> = √(r′ × 0.5) = **0.0764 m**
- D<sub>eq</sub> = ∛(15 × 15 × 30) = **18.9 m**
- L = 2×10⁻⁷ ln(18.9/0.0764) = **1.102×10⁻⁶ H/m**
- **X<sub>L</sub> = 2π·50·1.102×10⁻⁶ × 1000 = 0.346 Ω/km**

### M3 ⭐⭐⭐⭐⭐ Telephone line ("all-time favourite")
**General formula:** M = 2×10⁻⁷ ln[(D<sub>14</sub>·D<sub>23</sub>)/(D<sub>13</sub>·D<sub>24</sub>)] H/m (1, 2 = power; 3, 4 = telephone). Induced voltage V = ωMI.

**Version A (F24a 1d, TT-3 20-21): same horizontal plane**
*Power spacing 2.5 m, phone spacing 0.6 m, nearest distance 20 m, I = 150 A, 50 Hz.*
- Positions: A = 0, B = 2.5, C = 22.5, D = 23.1 m
- D<sub>AC</sub> = 22.5, D<sub>AD</sub> = 23.1, D<sub>BC</sub> = 20, D<sub>BD</sub> = 20.6 m
- M = 2×10⁻⁷ ln[(D<sub>AD</sub>·D<sub>BC</sub>)/(D<sub>AC</sub>·D<sub>BD</sub>)] = 2×10⁻⁷ ln[(23.1×20)/(22.5×20.6)] = 2×10⁻⁷ ln(462/463.5)
- |M| = 6.48×10⁻¹⁰ H/m = **0.648 µH/km**
- V = 2π(50)(6.48×10⁻⁷)(150) = **0.0306 V/km ≈ 30.6 mV/km**

**Version B (F24b 1d): telephone line symmetrically below**
*Power spacing 3 m; telephone 2 m below, symmetrical, spacing 0.8 m; I = 100 A, 50 Hz.*
- P₁ = (−1.5, 0), P₂ = (1.5, 0), T₁ = (−0.4, −2), T₂ = (0.4, −2)
- D<sub>P1T1</sub> = √(1.1² + 2²) = 2.2825 m = D<sub>P2T2</sub>; D<sub>P1T2</sub> = √(1.9² + 2²) = 2.7586 m = D<sub>P2T1</sub>
- Flux linking the phone loop: ψ = 2×10⁻⁷ I [ln(D<sub>P1T2</sub>/D<sub>P1T1</sub>) − ln(D<sub>P2T2</sub>/D<sub>P2T1</sub>)] = 2×10⁻⁷ I · 2 ln(2.7586/2.2825)
- **M = 4×10⁻⁷ ln(1.2086) = 7.58×10⁻⁸ H/m = 0.0758 mH/km**
- **V = 2π(50)(0.0758×10⁻³)(100) = 2.38 V/km**

### Composite conductor (Stevenson Ex 4.2, older TT-1)
*Side X: 3 solid wires r = 0.25 cm at a, b, c (vertical, 6 m apart). Side Y: 2 wires r = 0.5 cm at d (9 m from a, same level) and e (6 m below d).*
- D<sub>m</sub> = ⁶√(D<sub>ad</sub>D<sub>ae</sub>D<sub>bd</sub>D<sub>be</sub>D<sub>cd</sub>D<sub>ce</sub>) = ⁶√(9 · √117 · √117 · 9 · 15 · √117) = **10.743 m**
- D<sub>sX</sub> = ⁹√(r′³ · 6·12 · 6·6 · 12·6), r′ = 0.001947 m → **0.481 m**
- D<sub>sY</sub> = √(r′ × 6), r′ = 0.003894 m → **0.153 m**
- L<sub>X</sub> = 2×10⁻⁷ ln(10.743/0.481) = **6.212×10⁻⁷ H/m**; L<sub>Y</sub> = 2×10⁻⁷ ln(10.743/0.153) = **8.503×10⁻⁷ H/m**
- **L = L<sub>X</sub> + L<sub>Y</sub> = 14.715×10⁻⁷ H/m**

### Double-circuit line (your TT-1)
*a b c a′ b′ c′ in one horizontal row, 1 m spacing, r = 1.9 cm; a–a′, b–b′, c–c′ same phase (assume transposed).*
- r′ = 0.7788 × 0.019 = 0.0148 m. Each phase pair is 3 m apart: D<sub>s</sub> = √(r′ × 3) = **0.2107 m** (same for a, b, c)
- D<sub>ab</sub> = ⁴√(D<sub>ab</sub>D<sub>ab′</sub>D<sub>a′b</sub>D<sub>a′b′</sub>) = ⁴√(1·4·2·1) = 1.682 m
- D<sub>bc</sub> = ⁴√(1·4·2·1) = 1.682 m; D<sub>ca</sub> = ⁴√(2·1·5·2) = 2.115 m
- D<sub>eq</sub> = ∛(1.682 × 1.682 × 2.115) = **1.815 m**
- **L = 2×10⁻⁷ ln(1.815/0.2107) = 4.31×10⁻⁷ H/m = 0.431 mH/km/phase**

---

## PART 2: Capacitance (Ch-3)

### M12 ⭐⭐⭐⭐ Flat spacing (F22 2b, F24b 5b; Kothari Ex 3.2)
*3-φ, 50 Hz, flat horizontal spacing 3.5 m, No. 2/0 copper, outside diameter 1.05 cm, 110 kV.*
- r = 0.525 cm; D<sub>eq</sub> = ∛(3.5 × 3.5 × 7) = 3.5·∛2 = **4.41 m**
- C<sub>n</sub> = 2πε₀ / ln(D<sub>eq</sub>/r) = 55.63×10⁻¹² / ln(441/0.525) = **8.26×10⁻¹² F/m = 0.00826 µF/km**
- I<sub>c</sub> = ωC<sub>n</sub>V<sub>ph</sub> = 2π(50)(8.26×10⁻⁹)(110000/√3) = **0.165 A/km**

### Partridge, single-phase susceptance (older TT-1, Stevenson)
*60 Hz, Partridge (outside diameter 0.642 in), spacing 20 ft.*
- r = 0.321 in = 0.02675 ft; C<sub>ab</sub> = πε₀ / ln(D/r) = 27.8×10⁻¹²/ln(747.7) = 4.20×10⁻¹² F/m
- **B = ωC<sub>ab</sub> × 1609 = 2.55×10⁻⁶ S/mile** (line-to-line)

---

## PART 3: Underground cables (Ch-11)

Key formulas: C = 2πε₀ε<sub>r</sub>/ln(D/d) F/m = ε<sub>r</sub>/(41.4 log(D/d)) × 10⁻⁹ F/m · g<sub>max</sub> = 2V/(d ln(D/d)) · g<sub>min</sub> = 2V/(D ln(D/d)) · R<sub>ins</sub> = (ρ/2πl) ln(r₂/r₁)

### M11 ⭐⭐⭐⭐ 11 kV, conductor area 0.645 cm² (F24b 2c, TT-2 21-22)
*Sheath internal diameter 2.18 cm, ε<sub>r</sub> = 3.5, 50 Hz.*
- d = √(4 × 0.645/π) = **0.906 cm**; ln(D/d) = ln(2.18/0.906) = 0.878
- **g<sub>max</sub> = 2 × 11/(0.906 × 0.878) = 27.66 kV/cm (rms)**
- **g<sub>min</sub> = 2 × 11/(2.18 × 0.878) = 11.5 kV/cm (rms)**
- **C = 3.5/(41.4 log 2.406) × 10⁻⁹ = 0.222 µF/km**
- **I<sub>c</sub> = 2π(50)(0.222×10⁻⁶)(11000) = 0.766 A**

### 33 kV, d = 1 cm, D = 4 cm (F24a 2d; Mehta 11.7)
- **g<sub>max</sub> = 2 × 33/(1 × ln 4) = 47.6 kV/cm rms**; **g<sub>min</sub> = 2 × 33/(4 × ln 4) = 11.9 kV/cm rms**

### g<sub>max</sub> = 40, g<sub>min</sub> = 10 kV/cm, d = 2 cm (F24a 4c; Mehta 11.8)
- g<sub>max</sub>/g<sub>min</sub> = D/d → D = 4 × 2 = 8 cm → **insulation thickness = (8 − 2)/2 = 3 cm**
- V = g<sub>max</sub> · (d/2) · ln(D/d) = 40 × 1 × ln 4 = **55.45 kV (rms)**

### M8 ⭐⭐⭐⭐ Most economical conductor size (F21, F22 theory; F24b 6a maths; Mehta 11.10)
*Single-core cable, 132 kV 3-φ, permissible g<sub>max</sub> = 60 kV/cm.*
- Theory: d/dd [d ln(D/d)] = 0 → ln(D/d) = 1 → **D = 2.718 d** and g<sub>max</sub> = 2V/d
- V (peak, phase) = 132 × √2/√3 = 107.8 kV
- **d = 2V/g<sub>max</sub> = 2 × 107.8/60 = 3.59 cm**; **D = 2.718 × 3.59 = 9.77 cm**

### M10 ⭐⭐⭐⭐ Insulation thickness (F22 3c, F24b 4b; Mehta 11.2)
*R = 495 MΩ/km, core diameter 2.5 cm, ρ = 4.5×10¹⁴ Ω-cm.*
- R = (ρ/2πl) ln(r₂/r₁) → 495×10⁶ = (4.5×10¹⁴ / 2π×10⁵) ln(r₂/1.25)
- ln(r₂/1.25) = 0.691 → r₂ = 2.495 cm → **thickness = 2.495 − 1.25 ≈ 1.25 cm**

### Insulation resistance, 3 km (F21 3a; Tutorial 11.3)
*r = 12.5 mm, insulation 10 mm, ρ = 5×10¹² Ω-m.*
- **R = (5×10¹²/2π·3000) ln(22.5/12.5) = 155.9 MΩ**

### Graded cable, two dielectrics (F24b 4d)
*66 kV single-core, ε₁ = 5 (inner), ε₂ = 3, each 1 cm thick, core diameter 2 cm → d = 2, d₁ = 4, D = 6 cm.*
- Same charge: ε₁ d g<sub>1max</sub> = ε₂ d₁ g<sub>2max</sub> → g<sub>2max</sub> = (5×2)/(3×4) g<sub>1max</sub> = 0.833 g<sub>1max</sub>
- V = g<sub>1max</sub>(d/2) ln(d₁/d) + g<sub>2max</sub>(d₁/2) ln(D/d₁) = g<sub>1max</sub>[1·ln2 + 0.833·2·ln1.5] = 1.369 g<sub>1max</sub>
- **g<sub>1max</sub> = 66/1.369 = 48.2 kV/cm; g<sub>2max</sub> = 40.2 kV/cm** (rms)

### 3-core belted cable (F24a 3d; Mehta 11.18)
*C(three cores bunched ↔ sheath) = 12.6 µF; C(one core ↔ other two + sheath) = 7.4 µF; 66 kV, 50 Hz.*
- 3C<sub>e</sub> = 12.6 → **C<sub>e</sub> = 4.2 µF**
- C<sub>e</sub> + 2C<sub>c</sub> = 7.4 → **C<sub>c</sub> = 1.6 µF**
- C<sub>N</sub> = C<sub>e</sub> + 3C<sub>c</sub> = **9 µF**
- **I<sub>c</sub> = 2π(50)(9×10⁻⁶)(66000/√3) = 107.7 A**

### 33 kV, 4 km, three single-core cables (F21 3c; Mehta 11.6)
*d = 2.5 cm, radial thickness 0.5 cm → D = 3.5 cm, ε<sub>r</sub> = 3.*
- C/km = 3/(41.4 log 1.4) = 0.496 µF → **C/phase (4 km) = 1.98 µF**
- **I<sub>c</sub> = 2π(50)(1.98×10⁻⁶)(33000/√3) = 11.87 A**
- **kVAR = √3 × 33 × 11.87 = 678 kVAR**

### 66 kV, 1 km, core 10 cm, insulation 7 cm, ε<sub>r</sub> = 4 (F21 2d; Mehta 11.5)
- D = 24 cm; **C = 4/(41.4 log 2.4) = 0.254 µF**; **I<sub>c</sub> = 2π(50)(0.254×10⁻⁶)(66000/√3) = 3.04 A**

### 11 kV single-phase, 2.5 km (older TT-2)
*d = 20 mm, sheath radius 15 mm → D = 30 mm, ε<sub>r</sub> = 2.4.*
- **C = 2.4/(41.4 log 1.5) × 2.5 = 0.823 µF**; **I<sub>c</sub> = 2π(50)(0.823×10⁻⁶)(11000) = 2.84 A**; **kVAR = 11 × 2.84 = 31.3**

### Permissible current loading (your TT-2)
*Core 30 mm (r₁ = 15 mm), dielectric 40 mm (r₂ = 55 mm), thermal resistivity k = 5 thermal-Ω-m, sheath-to-ground S = 0.45, Δt = 55 °C, R = 110 µΩ/m, n = 1.*
- S<sub>dielectric</sub> = (k/2π) ln(r₂/r₁) = (5/2π) ln(55/15) = 1.034 thermal Ω/m
- S = 1.034 + 0.45 = 1.484
- **I = √(t / (nRS)) = √(55 / (110×10⁻⁶ × 1.484)) ≈ 580 A**

### M5 ⭐⭐⭐⭐ Murray loop (F22 4c, F24b 1b, TT-3 21-22)
*500 m faulty cable 1 Ω/1000 m; looped with a sound cable of same length 2.25 Ω/1000 m; ratio arms 2.75 : 1.*
- Faulty R = 0.5 Ω, sound R = 1.125 Ω → loop (R + X) = 1.625 Ω
- P/Q = R/X → (P + Q)/Q = (R + X)/X → X = [Q/(P + Q)] × loop = (1/3.75) × 1.625 = 0.4333 Ω
- **Distance = 0.4333 Ω ÷ (1 Ω/1000 m) = 433.3 m**

### M6 ⭐⭐⭐⭐ Varley loop (F24a 5b; your TT-2; Mehta 11.24)
*Formula (P = Q): S + X = (loop − X) → **X = (loop − S)/2**.*
- F24a: 20 km, 20 Ω/km: loop = 2 × 20 × 20 = 800 Ω; X = (800 − 200)/2 = 300 Ω → **fault at 300/20 = 15 km**
- Your TT-2: 40 km, 40 Ω/km: loop = 3200 Ω; X = (3200 − 200)/2 = 1500 Ω → **fault at 37.5 km**

---

## PART 4: Overhead lines (Ch-8)

### M1 ⭐⭐⭐⭐⭐ String of insulators
**One rule does all the maths:** V<sub>n+1</sub> = V<sub>n</sub> + m(V₁ + V₂ + … + V<sub>n</sub>), with V₁ at the top (tower side) and m = C<sub>shunt</sub>/C<sub>self</sub> = K.
For 3 discs: V₂ = V₁(1 + m), V₃ = V₁(1 + 3m + m²). String efficiency η = V<sub>ph</sub>/(n × V<sub>bottom</sub>).

**(a) Your TT-3 / F24b 5c: top 8 kV, middle 11 kV**
- 11 = 8(1 + K) → **K = 0.375**
- V₃ = V₂ + K(V₁ + V₂) = 11 + 0.375 × 19 = **18.125 kV**
- V<sub>ph</sub> = 8 + 11 + 18.125 = 37.125 kV → **V<sub>line</sub> = √3 × 37.125 = 64.3 kV**
- **η = 37.125/(3 × 18.125) = 68.3 %**
- Equivalent circuit: 3 self capacitances C in series (pin to cap), with a shunt capacitance KC from each cap/pin junction to the tower.

**(b) F24b 3c: 33 kV, 3 units, m = 0.11**
- V<sub>ph</sub> = 19.05 kV = V₁(1 + 1.11 + 1.3421) = 3.4521 V₁
- **V₁ = 5.52, V₂ = 6.13, V₃ = 7.41 kV; η = 19.05/(3 × 7.41) = 85.7 %**

**(c) F21 4b: line unit 17.5 kV, m = 1/8**
- 17.5 = V₁(1 + 3/8 + 1/64) = 1.3906 V₁ → **V₁ = 12.58, V₂ = 14.16 kV**
- V<sub>ph</sub> = 44.24 kV → **V<sub>line</sub> = 76.6 kV; η = 44.24/(3 × 17.5) = 84.3 %**

**(d) TT-2 (21-22): 5 discs, 100 kV, m = 0.1**
- V<sub>ph</sub> = 57.74 kV. Ratios 1 : 1.1 : 1.31 : 1.651 : 2.157
- **V₁ … V₅ = 8.00, 8.80, 10.48, 13.21, 17.25 kV; η = 57.74/(5 × 17.25) = 66.9 %**

### M7 ⭐⭐⭐⭐ Sag
**Equal supports:** S = wl²/(8T), T = breaking load/SF.
**Unequal supports (h = difference in heights):** x₁ = l/2 − Th/(wl), x₂ = l/2 + Th/(wl), S₁ = wx₁²/(2T), S₂ = wx₂²/(2T).

**(a) F22 5c (Mehta 8.23): towers 30 m and 90 m, span 500 m, T = 1600 kg, w = 1.5 kg/m**
- h = 60 m; x₁ = 250 − (1600 × 60)/(1.5 × 500) = **122 m** (from the lower tower)
- S₁ = 1.5 × 122²/(2 × 1600) = 6.98 m → **minimum clearance = 30 − 6.98 = 23.02 m**
- Midway point is 250 − 122 = 128 m from the lowest point → sag = 1.5 × 128²/3200 = 7.68 m
- **Clearance at midway = 23.02 + 7.68 = 30.70 m**

**(b) F21 5c (Mehta 8.25): towers 40 m and 90 m, span 400 m, T = 2000 kg, w = 1 kg/m**
- x₁ = 200 − (2000 × 50)/(1 × 400) = −50 m → the lowest point lies **50 m outside** the span, beyond the lower tower
- Midway point is 200 + 50 = 250 m from the lowest point. Height of lowest point = 40 − (1 × 50²/4000) = 39.375 m
- **Clearance at midway = 39.375 + 1 × 250²/4000 = 39.375 + 15.625 = 55 m**

**(c) F24a 5c (Mehta 8.17): 132 kV, w = 680 kg/km, span 260 m, ultimate strength 3100 kg, SF = 2, clearance 10 m**
- T = 3100/2 = 1550 kg; S = 0.68 × 260²/(8 × 1550) = **3.71 m**
- **Height of support = 10 + 3.71 = 13.71 m**

**(d) Your TT-2: span 300 m, area 1.3 cm², 1170 kg/km, breaking stress 4218 kg/cm², SF = 5, wind 122 kg/m²**
- d = √(4 × 1.3/π) = 1.287 cm; w<sub>wind</sub> = 122 × 0.01287 = 1.570 kg/m; w = 1.17 kg/m
- w<sub>t</sub> = √(1.17² + 1.570²) = 1.958 kg/m; T = 4218 × 1.3/5 = 1096.7 kg
- **Slant sag S = 1.958 × 300²/(8 × 1096.7) = 20.08 m**
- **Vertical sag = S × (w/w<sub>t</sub>) = 20.08 × 1.17/1.958 = 12.0 m**

### Corona: spacing (F21 5b; Mehta 8.14)
*132 kV line, conductor diameter 1.956 cm, corona if line voltage > 210 kV (rms), g₀ = 30 kV/cm (peak), m = δ = 1.*
- V<sub>c</sub> (phase) = g₀ r ln(d/r), with g₀ = 30/√2 = 21.21 kV/cm rms
- 210/√3 = 121.24 = 21.21 × 0.978 × ln(d/0.978) → ln(d/r) = 5.845
- **d = 0.978 × e<sup>5.845</sup> ≈ 338 cm ≈ 3.38 m**

---

## PART 5: Stability (Ch-12)

### M2 ⭐⭐⭐⭐⭐ Generator → infinite bus (F24a 6c, F24b 6d, TT-3 20-21)
*x′<sub>d</sub> = 0.25, transformer j0.1, two parallel lines j0.5 each, P = 1.0 pu, |V<sub>t</sub>| = 1.0, |V| = 1.0∠0°.*
1. X between V<sub>t</sub> and the bus = 0.1 + 0.5‖0.5 = 0.35. P = V<sub>t</sub>V sin θ / 0.35 = 1 → sin θ = 0.35 → **θ = 20.49°**
2. V<sub>t</sub> = 1∠20.49° = 0.9367 + j0.35
3. I = (V<sub>t</sub> − V)/j0.35 = (−0.0633 + j0.35)/j0.35 = **1 + j0.181 pu**
4. E′ = V<sub>t</sub> + j0.25 I = 0.9367 + j0.35 + j0.25 − 0.0452 = 0.8915 + j0.60 → **E′ = 1.075∠33.94° pu**
- **(i) Healthy:** X = 0.25 + 0.1 + 0.25 = 0.6 → **P<sub>max</sub> = 1.075/0.6 = 1.79 pu**
- **(ii) 3-φ fault at the middle of one line:** star (0.35, 0.5, 0.25 to ground) → transfer X = (0.35×0.5 + 0.5×0.25 + 0.25×0.35)/0.25 = **1.55** → **P<sub>max</sub> = 0.693 pu**
- **(iii) One line open:** X = 0.25 + 0.1 + 0.5 = 0.85 → **P<sub>max</sub> = 1.264 pu**
- Plot: three sine curves P = P<sub>max</sub> sin δ with peaks 1.79 > 1.264 > 0.693; draw the P<sub>m</sub> = 1 line; δ₀ = sin⁻¹(1/1.79) = 33.9°.

### Power-angle equation (F22 6c, Stevenson)
*x′<sub>d</sub> = 0.2, j0.1, lines j0.4 ‖ j0.4, P = 1, V<sub>t</sub> = V = 1.*
- X(V<sub>t</sub> → bus) = 0.1 + 0.2 = 0.3 → sin θ = 0.3, θ = 17.46°; V<sub>t</sub> = 0.954 + j0.3
- I = (V<sub>t</sub> − 1)/j0.3 = 1 + j0.154; E′ = V<sub>t</sub> + j0.2 I = 0.923 + j0.5 = **1.05∠28.44°**
- X<sub>total</sub> = 0.2 + 0.1 + 0.2 = 0.5 → **P<sub>e</sub> = (1.05 × 1/0.5) sin δ = 2.10 sin δ pu**
