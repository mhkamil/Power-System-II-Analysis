# Derivations Guide: step skeletons you must reproduce

> Learn the **steps in order**. In the exam, draw the figure first, then write each numbered step. Steps follow your class notes (Lec 2–6, 8–10, 13–15).

---

## D1 ⭐⭐⭐⭐⭐ Capacitance of a 3-φ line with unsymmetrical spacing (asked 5 times)
**Figure:** triangle a(1), b(2), c(3) with sides D₁₂, D₂₃, D₃₁ + transposition diagram (Section 1: a-b-c, Section 2: c-a-b, Section 3: b-c-a).

1. Assume the line is **fully transposed**, all conductors have radius r, and the charge per unit length is the same in each section (q<sub>a</sub>, q<sub>b</sub>, q<sub>c</sub>).
2. Use V<sub>ab</sub> = (1/2πk)[q<sub>a</sub> ln(D<sub>ab</sub>/r) + q<sub>b</sub> ln(r/D<sub>ab</sub>) + q<sub>c</sub> ln(D<sub>cb</sub>/D<sub>ca</sub>)] for each section:
   - Sec 1: V<sub>ab1</sub> = (1/2πk)[q<sub>a</sub> ln(D₁₂/r) + q<sub>b</sub> ln(r/D₁₂) + q<sub>c</sub> ln(D₂₃/D₃₁)]
   - Sec 2: V<sub>ab2</sub> = (1/2πk)[q<sub>a</sub> ln(D₂₃/r) + q<sub>b</sub> ln(r/D₂₃) + q<sub>c</sub> ln(D₃₁/D₁₂)]
   - Sec 3: V<sub>ab3</sub> = (1/2πk)[q<sub>a</sub> ln(D₃₁/r) + q<sub>b</sub> ln(r/D₃₁) + q<sub>c</sub> ln(D₁₂/D₂₃)]
3. Average: V<sub>ab</sub> = (V<sub>ab1</sub> + V<sub>ab2</sub> + V<sub>ab3</sub>)/3. The q<sub>c</sub> term becomes ln(1) = 0:
   **V<sub>ab</sub> = (1/2πk)[q<sub>a</sub> ln(D<sub>eq</sub>/r) + q<sub>b</sub> ln(r/D<sub>eq</sub>)]**, where **D<sub>eq</sub> = ∛(D₁₂D₂₃D₃₁)**
4. Similarly **V<sub>ac</sub> = (1/2πk)[q<sub>a</sub> ln(D<sub>eq</sub>/r) + q<sub>c</sub> ln(r/D<sub>eq</sub>)]**
5. Add: V<sub>ab</sub> + V<sub>ac</sub> = (1/2πk)[2q<sub>a</sub> ln(D<sub>eq</sub>/r) + (q<sub>b</sub> + q<sub>c</sub>) ln(r/D<sub>eq</sub>)]
6. Balanced: q<sub>a</sub> + q<sub>b</sub> + q<sub>c</sub> = 0 → q<sub>b</sub> + q<sub>c</sub> = −q<sub>a</sub> → V<sub>ab</sub> + V<sub>ac</sub> = (3q<sub>a</sub>/2πk) ln(D<sub>eq</sub>/r)
7. Phasor diagram: V<sub>ab</sub> + V<sub>ac</sub> = 3V<sub>an</sub> (draw V<sub>an</sub>, V<sub>bn</sub>, V<sub>cn</sub> at 120°)
8. So V<sub>an</sub> = (q<sub>a</sub>/2πk) ln(D<sub>eq</sub>/r)
9. **C<sub>n</sub> = q<sub>a</sub>/V<sub>an</sub> = 2πk / ln(D<sub>eq</sub>/r) F/m to neutral**; for air: **C<sub>n</sub> = 0.0242 / log(D<sub>eq</sub>/r) µF/km**
10. Charging current: I<sub>a</sub> = jωC<sub>n</sub>V<sub>an</sub> A/km.

> For **equilateral spacing** (D<sub>eq</sub> = D) use steps 4–9 directly with D instead of D<sub>eq</sub>.

---

## D5 ⭐⭐⭐⭐ Inductance of a 3-φ line with unsymmetrical spacing (+ transposition)
1. Without transposition: λ<sub>a</sub> = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + I<sub>b</sub> ln(1/D<sub>ab</sub>) + I<sub>c</sub> ln(1/D<sub>ca</sub>)], and similarly for λ<sub>b</sub>, λ<sub>c</sub> (write the 3×3 matrix).
2. With I<sub>b</sub> = α²I<sub>a</sub>, I<sub>c</sub> = αI<sub>a</sub>: L<sub>a</sub>, L<sub>b</sub>, L<sub>c</sub> come out **unequal and complex**, so the line is unbalanced. **Therefore we transpose.**
3. Transposed, positions 1, 2, 3:
   - λ<sub>a1</sub> = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + I<sub>b</sub> ln(1/D₁₂) + I<sub>c</sub> ln(1/D₁₃)]
   - λ<sub>a2</sub> = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + I<sub>b</sub> ln(1/D₂₃) + I<sub>c</sub> ln(1/D₁₂)]
   - λ<sub>a3</sub> = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + I<sub>b</sub> ln(1/D₁₃) + I<sub>c</sub> ln(1/D₂₃)]
4. λ<sub>a</sub> = (λ<sub>a1</sub> + λ<sub>a2</sub> + λ<sub>a3</sub>)/3 = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + (I<sub>b</sub> + I<sub>c</sub>) ln(1/∛(D₁₂D₂₃D₁₃))]
5. I<sub>b</sub> + I<sub>c</sub> = −I<sub>a</sub> → λ<sub>a</sub> = 2×10⁻⁷ I<sub>a</sub> ln(D<sub>eq</sub>/r′)
6. **L<sub>a</sub> = L<sub>b</sub> = L<sub>c</sub> = 2×10⁻⁷ ln(D<sub>eq</sub>/r′) H/m = 0.4605 log(D<sub>eq</sub>/r′) mH/km**, D<sub>eq</sub> = ∛(D₁₂D₂₃D₃₁)

**Equilateral (prove L equal):** λ<sub>a</sub> = 2×10⁻⁷[I<sub>a</sub> ln(1/r′) + (I<sub>b</sub> + I<sub>c</sub>) ln(1/D)] = 2×10⁻⁷ I<sub>a</sub> ln(D/r′), so by symmetry L<sub>a</sub> = L<sub>b</sub> = L<sub>c</sub> = 2×10⁻⁷ ln(D/r′).

---

## D2 ⭐⭐⭐⭐⭐ Inductance of composite-conductor lines (teacher: "derivation very important")
**Figure:** conductor A = n identical strands (1, 2, …, n) carrying I/n each; conductor B = m strands (1′, …, m′) carrying −I/m each.

1. From "flux linkage of one conductor in a group": λ<sub>i</sub> = 2×10⁻⁷ Σ I<sub>j</sub> ln(1/D<sub>ij</sub>)
2. For filament 1 of A:
   λ₁ = 2×10⁻⁷ (I/n)[ln(1/r₁′) + ln(1/D₁₂) + … + ln(1/D₁ₙ)] − 2×10⁻⁷ (I/m)[ln(1/D₁₁′) + ln(1/D₁₂′) + … + ln(1/D₁ₘ)]
3. Combine: λ₁ = 2×10⁻⁷ I ln[ ᵐ√(D₁₁′D₁₂′…D₁ₘ) / ⁿ√(r₁′D₁₂…D₁ₙ) ]
4. Filament inductance: L₁ = λ₁/(I/n) = 2n×10⁻⁷ ln[ ᵐ√(D₁₁′…D₁ₘ) / ⁿ√(r₁′D₁₂…D₁ₙ) ]. Write similarly for L₂ … Lₙ.
5. Average filament inductance L<sub>av</sub> = (L₁ + … + Lₙ)/n. The n filaments are in parallel, so **L<sub>A</sub> = L<sub>av</sub>/n = (L₁ + … + Lₙ)/n²**
6. L<sub>A</sub> = 2×10⁻⁷ ln[ ᵐⁿ√((D₁₁′…D₁ₘ)…(Dₙ₁′…Dₙₘ)) / ⁿ²√((D₁₁…D₁ₙ)…(Dₙ₁…Dₙₙ)) ], with D<sub>ii</sub> = r<sub>i</sub>′
7. **L<sub>A</sub> = 2×10⁻⁷ ln(D<sub>m</sub>/D<sub>sA</sub>) H/m = 0.461 log(D<sub>m</sub>/D<sub>s</sub>) mH/km**
   - D<sub>m</sub> = mutual GMD (mn-th root of mn distances)
   - D<sub>s</sub> = self GMD/GMR (n²-th root of n² distances)
8. Similarly L<sub>B</sub>; total **L = L<sub>A</sub> + L<sub>B</sub>**.

## Flux linkages of one conductor in a group (pre-step of D2)
n conductors carrying I₁ … Iₙ with ΣI = 0; point P far away at distances D₁ₚ … Dₙₚ.
λ<sub>i</sub> = 2×10⁻⁷[I₁ ln(D₁ₚ/D<sub>i1</sub>) + … + I<sub>i</sub> ln(D<sub>ip</sub>/r<sub>i</sub>′) + … + Iₙ ln(Dₙₚ/D<sub>in</sub>)]. Split the logs and substitute Iₙ = −(I₁ + … + Iₙ₋₁). As P → ∞, every ln(D<sub>kp</sub>/Dₙₚ) → 0, so
**λ<sub>i</sub> = 2×10⁻⁷[I₁ ln(1/D<sub>i1</sub>) + … + I<sub>i</sub> ln(1/r<sub>i</sub>′) + … + Iₙ ln(1/D<sub>in</sub>)] Wb-T/m**

## Single-phase two-wire line (L = 4×10⁻⁷ ln D/r′)
1. Internal flux linkage: λ<sub>int</sub> = I/2 × 10⁻⁷ (Ampère's law, H<sub>x</sub> = I x/2πr²; partial linkage x²/r²; integrate 0 → r)
2. External between D₁ and D₂: λ = 2×10⁻⁷ I ln(D₂/D₁)
3. Conductor 1 up to D: λ = 2×10⁻⁷ I[¼ + ln(D/r)] = 2×10⁻⁷ I ln(D/(re<sup>−¼</sup>)) = 2×10⁻⁷ I ln(D/r′), with r′ = 0.7788 r
4. L₁ = 2×10⁻⁷ ln(D/r₁′), L₂ = 2×10⁻⁷ ln(D/r₂′)
5. **L = L₁ + L₂ = 4×10⁻⁷ ln(D/√(r₁′r₂′)) = 4×10⁻⁷ ln(D/r′) H/m** (if r₁ = r₂) = 0.921 log(D/r′) mH/km

---

## D4 ⭐⭐⭐⭐ Dielectric stress in a single-core cable (+ proof g<sub>max</sub> is at the conductor)
**Figure:** core diameter d, sheath inner diameter D, a cylinder of radius x.

1. Charge Q C/m. Electric flux density at radius x: D<sub>x</sub> = Q/(2πx) C/m²
2. Field (stress): **g = E<sub>x</sub> = Q/(2πε₀ε<sub>r</sub>x)** V/m
3. V between core and sheath: V = ∫<sub>d/2</sub><sup>D/2</sup> g dx = (Q/2πε₀ε<sub>r</sub>) ln(D/d)
4. Eliminate Q: **g = V / (x ln(D/d))**
5. Since g ∝ 1/x, **g is maximum at the smallest x = d/2 (conductor surface)** and decreases outwards, minimum at x = D/2 (sheath):
   - **g<sub>max</sub> = 2V/(d ln(D/d))**, **g<sub>min</sub> = 2V/(D ln(D/d))**, **g<sub>max</sub>/g<sub>min</sub> = D/d**
6. (Capacitance comes from step 3: C = Q/V = 2πε₀ε<sub>r</sub>/ln(D/d) F/m = ε<sub>r</sub>/(41.4 log(D/d)) × 10⁻⁹ F/m.)

### Most economical conductor size (follow-on)
g<sub>max</sub> = 2V/(d ln(D/d)). For fixed V and D, g<sub>max</sub> is minimum when d ln(D/d) is maximum: d/dd[d ln(D/d)] = ln(D/d) − 1 = 0 → **D = e·d = 2.718 d** → **g<sub>max</sub> = 2V/d → d = 2V/g<sub>max</sub>**.

### Capacitance grading (F24b 2d)
Why non-uniform stress is undesirable: (i) a thicker insulation is needed, which increases the cable size; (ii) it can lead to breakdown of insulation.
1. Three layers ε₁ > ε₂ > ε₃ with boundaries d, d₁, d₂, D. Same Q: g<sub>1max</sub> = Q/(πε₀ε₁d), g<sub>2max</sub> = Q/(πε₀ε₂d₁), g<sub>3max</sub> = Q/(πε₀ε₃d₂)
2. For equal maximum stress: **ε₁d = ε₂d₁ = ε₃d₂**
3. V₁ = (g<sub>max</sub>d/2) ln(d₁/d), V₂ = (g<sub>max</sub>d₁/2) ln(d₂/d₁), V₃ = (g<sub>max</sub>d₂/2) ln(D/d₂)
4. **V = (g<sub>max</sub>/2)[d ln(d₁/d) + d₁ ln(d₂/d₁) + d₂ ln(D/d₂)]** > V′ = (g<sub>max</sub>d/2) ln(D/d) for an ungraded cable, so a graded cable works at a higher voltage or uses a smaller size.
5. Intersheath grading: g<sub>1max</sub> = 2V₁/(d ln(d₁/d)), g<sub>2max</sub> = 2V₂/(d₁ ln(d₂/d₁)), g<sub>3max</sub> = 2V₃/(d₂ ln(D/d₂)), set equal.

### Insulation resistance of a single-core cable
Elemental layer dx at radius x: dR = ρ dx/(2πxl) → **R = (ρ/2πl) ln(r₂/r₁)**

### Capacitance of a 3-core cable
C<sub>c</sub> between cores (delta) → star: 3C<sub>c</sub>. **C<sub>N</sub> = C<sub>e</sub> + 3C<sub>c</sub>; I<sub>c</sub> = 2πfC<sub>N</sub>V<sub>ph</sub>**. Measurement: (i) bunch the 3 cores and measure against the sheath → C₁ = 3C<sub>e</sub>; (ii) connect 2 cores to the sheath and measure against the 3rd → C₂ = C<sub>e</sub> + 2C<sub>c</sub>.

---

## D6 ⭐⭐⭐⭐ String efficiency: potential distribution (3 discs)
**Figure:** 3 discs in series (self capacitance C), shunt capacitance mC from each pin to the tower; currents I₁, I₂, I₃ and i₁, i₂.

1. Kirchhoff at junction A: I₂ = I₁ + i₁ → V₂ωC = V₁ωC + V₁ωmC → **V₂ = V₁(1 + m)**
2. At junction B: I₃ = I₂ + i₂ → V₃ωC = V₂ωC + (V₁ + V₂)ωmC → **V₃ = V₁(1 + 3m + m²)**
3. V = V₁ + V₂ + V₃ = V₁(3 + 4m + m²)
4. **η = V/(3V₃) × 100 %**
5. Effects: **K = m = 0.2**: V₂ = 1.2V₁, V₃ = 1.64V₁, η = 3.84/(3 × 1.64) ≈ 78 %. **K = 0.8**: V₂ = 1.8V₁, V₃ = 4.04V₁, η = 6.84/(3 × 4.04) ≈ 56 %, so a larger K gives worse efficiency (more unequal voltage). **More discs** → efficiency decreases (distribution becomes more uneven).

**Methods of improving string efficiency** (10 marks):
1. **Longer cross-arm**: reduces m (shunt capacitance). Limited by tower cost.
2. **Grading the units**: discs of different capacitance, with the largest capacitance nearest the line, so V × C is equal across all units.
3. **Static shielding (guard ring)**: a metal ring around the bottom unit, connected to the line. Its capacitance to each pin cancels the shunt charging current, which equalises the voltages.

---

## D3 ⭐⭐⭐⭐⭐ Swing equation (teacher: "derivation in exam")
1. Two torques act on the rotor: mechanical T<sub>m</sub> (from the turbine) and electrical T<sub>e</sub> (opposing). T<sub>m</sub> = T<sub>e</sub> → steady speed; T<sub>m</sub> > T<sub>e</sub> → speeds up; T<sub>m</sub> < T<sub>e</sub> → slows down.
2. Newton: **J d²θ<sub>m</sub>/dt² = T<sub>m</sub> − T<sub>e</sub>**
3. Rotor angle measured from a synchronously rotating frame: θ<sub>m</sub> = ω<sub>sm</sub>t + δ<sub>m</sub> → d²θ<sub>m</sub>/dt² = d²δ<sub>m</sub>/dt²
4. Multiply by ω<sub>sm</sub> (P = Tω): J ω<sub>sm</sub> d²δ<sub>m</sub>/dt² = P<sub>m</sub> − P<sub>e</sub>; M = Jω<sub>sm</sub> = angular momentum
5. **M d²δ/dt² = P<sub>m</sub> − P<sub>e</sub> = P<sub>a</sub>** (swing equation, power form)
6. Inertia constant H = stored KE/rating = ½Jω<sub>sm</sub>²/G (MJ/MVA) → M = 2GH/ω<sub>s</sub> = GH/(πf)
7. Per unit: **(2H/ω<sub>s</sub>) d²δ/dt² = P<sub>m</sub> − P<sub>e</sub>** or **(H/πf) d²δ/dt² = P<sub>m</sub> − P<sub>max</sub> sin δ** (pu), where P<sub>e</sub> = (|E||V|/X) sin δ
8. Plot the power-angle curve: stable region 0 < δ < 90°, P<sub>max</sub> at 90°.

**Multi-machine (coherent machines, δ₁ = δ₂):** add the two swing equations → M<sub>eq</sub> d²δ/dt² = P<sub>m,eq</sub> − P<sub>e,eq</sub>, with **H<sub>eq</sub> = (G₁H₁ + G₂H₂)/G<sub>sys</sub>**.
**Non-coherent:** M<sub>eq</sub> = M₁M₂/(M₁ + M₂), δ₁₂ = δ₁ − δ₂, P<sub>m</sub> = (M₂P<sub>m1</sub> − M₁P<sub>m2</sub>)/(M₁ + M₂).

## Equal-area criterion (derivation + sudden increase in input) ⭐⭐⭐⭐
1. M d²δ/dt² = P<sub>a</sub>. Multiply by 2dδ/dt: d/dt (dδ/dt)² = (2P<sub>a</sub>/M) dδ/dt
2. Integrate: (dδ/dt)² = (2/M) ∫<sub>δ₀</sub><sup>δ</sup> P<sub>a</sub> dδ
3. Stable when the swing stops (dδ/dt = 0) → **∫<sub>δ₀</sub><sup>δ</sup> (P<sub>m</sub> − P<sub>e</sub>) dδ = 0 → A₁ = A₂**

**Sudden increase in P<sub>m</sub> (P<sub>m0</sub> → P<sub>m1</sub>), on the P–δ diagram** (draw the sine curve with points a, b, c):
- **At a** (δ₀): P<sub>m0</sub> = P<sub>e0</sub>, P<sub>a</sub> = 0, ω = ω<sub>s</sub>.
- **a → b**: P<sub>m1</sub> > P<sub>e</sub> → P<sub>a</sub> positive → rotor accelerates, δ rises from δ₀ to δ₁. The KE stored is **A₁ = ∫<sub>δ₀</sub><sup>δ₁</sup> (P<sub>m1</sub> − P<sub>e</sub>) dδ** (accelerating area).
- **At b** (δ₁): P<sub>e</sub> = P<sub>m1</sub>, but ω > ω<sub>s</sub>, so δ keeps increasing because of rotor inertia.
- **b → c**: P<sub>e</sub> > P<sub>m1</sub> → P<sub>a</sub> negative → rotor decelerates. **A₂ = ∫<sub>δ₁</sub><sup>δ₂</sup> (P<sub>e</sub> − P<sub>m1</sub>) dδ**
- **At c** (δ₂): ω = ω<sub>s</sub> and **A₁ = A₂** → δ swings back and oscillates about b, and damping settles it at δ₁. **Stable** if A₂ (available up to δ<sub>max</sub> = 180° − δ₁) ≥ A₁.
- Advantage: no swing-curve solution needed for one machine vs infinite bus or any 2-machine system. Disadvantage: not applicable to a multi-machine system.
