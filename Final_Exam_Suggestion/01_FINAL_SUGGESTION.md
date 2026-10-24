# EEE 337 – Power System II: Final Exam Suggestion

> Built from **every file in this repo**: 4 previous finals (Dec-2021, 2022, 2024 [2020-21], 2024 [2021-22]), all term tests (your batch + older batches), all 17 lectures (including the teacher's own *"For Exam"*, *"Overview"*, *"Must"* and *"Not necessary"* notes), the syllabus and the course outcomes.
>
> ⭐ rating = how often it was asked + whether the teacher flagged it in class.
> 🔁 = number of times it appeared in finals/TTs.

---

## How the paper is set (pattern across all 4 finals)

| | Part A (answer any 2 of Q1–Q3) | Part B (answer any 2 of Q4–Q6) |
|---|---|---|
| Mostly from | Ch-2 Inductance, Ch-3 Capacitance, Ch-11 Cables | Ch-8 Overhead line, Ch-11 Cables (faults/loop tests), Ch-12 Stability, HVDC |
| Each question | 25 marks = 1 definition (1–4) + 1 derivation (8–10) + 1–2 maths (5–10) | same |

**Most important point:** the teacher repeats questions, often word-for-word with the same numbers. About **70 % of each final is a repeat** of an older final or a term test. If you learn the list below, you can answer 4 full questions.

---

## 🔴 TIER 1: Learn these first (asked 3 to 5 times, guaranteed)

### Derivations (each worth 8–10 marks)
| # | Question | 🔁 | Where asked |
|---|---|---|---|
| D1 ⭐⭐⭐⭐⭐ | **Derive the capacitance of a 3-phase line with unsymmetrical spacing** (transposed line, C<sub>n</sub> = 2πk / ln(D<sub>eq</sub>/r)) | **5** | F-2022, F-2024(20-21), F-2024(21-22), **your TT-1**, TT-1(21-22) |
| D2 ⭐⭐⭐⭐⭐ | **Derive the inductance of composite-conductor lines** (D<sub>m</sub>, D<sub>s</sub>, GMD/GMR) | 2 + teacher wrote *"Derivation very important for exam"* | F-2024(20-21), F-2024(21-22), Lec-4 |
| D3 ⭐⭐⭐⭐⭐ | **Derive the swing equation** (M d²δ/dt² = P<sub>m</sub> − P<sub>e</sub>, and the per-unit form with H) | 2 + teacher boxed *"Swing eqn derivation in exam"* | F-Dec2021, F-2022, Lec-13 |
| D4 ⭐⭐⭐⭐ | **Dielectric stress in a single-core cable**: derive it and prove it is maximum at the conductor surface (g<sub>max</sub>/g<sub>min</sub> = D/d) | 3 | F-Dec2021, F-2022, F-2024(20-21) |
| D5 ⭐⭐⭐⭐ | **Inductance of a 3-phase line with unsymmetrical spacing + transposition** (D<sub>eq</sub> = ∛(D<sub>12</sub>D<sub>23</sub>D<sub>31</sub>)) | 2 | F-2024(21-22), your TT notes |
| D6 ⭐⭐⭐⭐ | **String efficiency**: potential distribution over a suspension string with equivalent circuit; effect of K = 0.2, K = 0.8, more discs | 1 + TT-3 maths | F-2024(21-22) |

### Maths (repeated with the same numbers; solutions are in `03_Solved_Math_Bank.md`)
| # | Problem | 🔁 | Answer |
|---|---|---|---|
| M1 ⭐⭐⭐⭐⭐ | **String of insulators**: (a) 3 discs, top 8 kV, middle 11 kV; (b) 3 units, 33 kV, m = 11 %; (c) 3 discs, line unit 17.5 kV, m = 1/8; (d) 5 discs, 100 kV, m = 0.1 | **5** | (a) K = 0.375, V<sub>L</sub> = 64.3 kV, η = 68.3 % |
| M2 ⭐⭐⭐⭐⭐ | **Generator–infinite bus (x'<sub>d</sub> = 0.25, j0.1, two lines j0.5)**: find E′ and P<sub>max</sub> (healthy / 3-φ fault at middle / one line open) | **3** | E′ = 1.075∠33.9°, P<sub>max</sub> = 1.79 / 0.693 / 1.264 pu |
| M3 ⭐⭐⭐⭐⭐ | **Telephone-line mutual inductance** (teacher's "all-time favourite") | **3** | see bank (2 versions) |
| M4 ⭐⭐⭐⭐⭐ | **Bundled ACSR Pheasant, d = 45 cm, 8 m spacing**: X per km/mile + per-unit | **3** | 0.365 Ω/km, 0.587 Ω/mi, 0.049 pu |
| M5 ⭐⭐⭐⭐ | **Murray loop**: 500 m, 1 Ω/1000 m, sound 2.25 Ω/1000 m, ratio 2.75 : 1 | **3** | 433.3 m |
| M6 ⭐⭐⭐⭐ | **Varley loop**: 20 km, 20 Ω/km, S = 200 Ω (and your TT: 40 km, 40 Ω/km) | **3** | 15 km (37.5 km) |
| M7 ⭐⭐⭐⭐ | **Sag**: unequal towers at a river crossing (30/90 m, 500 m, 1600 kg, 1.5 kg/m) and (40/90 m, 400 m, 2000 kg, 1 kg/m); 132 kV support height; wind-loaded sag | **4** | 23.0 m & 30.7 m; 13.71 m; 20.08 m / 12.0 m |
| M8 ⭐⭐⭐⭐ | **Most economical conductor size** (132 kV, g<sub>max</sub> = 60 kV/cm) | **3** | d = 3.59 cm, D = 9.77 cm |
| M9 ⭐⭐⭐⭐ | **500 kV, 2-conductor bundle, 0.5 m, 15 m spacing**: X per phase | 2 | 0.346 Ω/km |
| M10 ⭐⭐⭐⭐ | **Insulation thickness** (495 MΩ/km, 2.5 cm core, ρ = 4.5×10¹⁴ Ω-cm) | 2 | 1.25 cm |
| M11 ⭐⭐⭐⭐ | **11 kV cable, 0.645 cm², sheath 2.18 cm, ε<sub>r</sub> = 3.5**: g<sub>max</sub>, g<sub>min</sub>, C, I<sub>c</sub> | 2 | 27.66 / 11.5 kV/cm, 0.222 µF/km, 0.766 A |
| M12 ⭐⭐⭐⭐ | **3-φ flat spacing 3.5 m, 110 kV, No. 2/0 Cu (1.05 cm)**: C<sub>n</sub> and charging current | 2 | 0.00826 µF/km, 0.165 A/km |

### Short questions (1 to 5 marks, very easy marks)
| # | Question | 🔁 |
|---|---|---|
| S1 ⭐⭐⭐⭐⭐ | **Transposition**: what it is and why it is used (+ figure of a–b–c sections) | **5** |
| S2 ⭐⭐⭐⭐⭐ | **String efficiency**: definition + methods of improving it (10-mark theory) | **4** |
| S3 ⭐⭐⭐⭐ | **Critical disruptive voltage**: definition + significance | **3** |
| S4 ⭐⭐⭐⭐ | **Corona**: definition, theory, advantages/disadvantages, methods of reducing | **3** |
| S5 ⭐⭐⭐⭐ | **Sudden increase in mechanical input, explained with the P–δ curve** (equal-area criterion) | **3** (incl. your TT-3) |
| S6 ⭐⭐⭐ | **HVDC**: definition, economics (break-even distance), types of links (monopolar/bipolar/homopolar) | **3** |

---

## 🟠 TIER 2: Study next (asked once or twice, or flagged by the teacher)

**Maths**
- 3-core belted cable: 12.6 µF and 7.4 µF at 66 kV → **I<sub>c</sub> = 107.7 A** (Mehta 11.18)
- 33 kV single-core, d = 1 cm, D = 4 cm → **g<sub>max</sub> = 47.6, g<sub>min</sub> = 11.9 kV/cm** (Mehta 11.7)
- g<sub>max</sub> = 40, g<sub>min</sub> = 10 kV/cm, d = 2 cm → **thickness 3 cm, V = 55.45 kV** (Mehta 11.8)
- Graded cable, 66 kV, ε 5 and 3, 1 cm each, core 2 cm → **48.2 and 40.2 kV/cm**
- 33 kV, 4 km, 3 single-core cables (2.5 cm, 0.5 cm, ε<sub>r</sub> 3) → **1.98 µF, 11.87 A, 678 kVAR** (Mehta 11.6)
- 11 kV single-phase cable, 2.5 km → **0.823 µF, 2.84 A, 31.3 kVAR**
- Insulation resistance, 3 km, r = 12.5 mm, t = 10 mm → **155.9 MΩ**
- Permissible current loading (your TT-2): **I ≈ 580 A**
- Corona: 132 kV line, 1.956 cm, corona at 210 kV → **spacing ≈ 3.38 m** (Mehta 8.14)
- Power-angle equation (x'<sub>d</sub> = 0.2, j0.1, lines j0.4) → **P<sub>e</sub> = 2.10 sin δ**
- Composite conductor (Stevenson 4.2): 3 wires of 0.25 cm vs 2 wires of 0.5 cm → **L = 14.7×10⁻⁷ H/m**
- **Double-circuit line** (your TT-1): a b c a′ b′ c′, 1 m spacing, r = 1.9 cm → **0.431 mH/km/phase**
- Capacitive susceptance, Partridge, 1-φ, 20 ft → **2.55 µS/mile**

**Derivations and theory**
- Inductance of a single-phase two-wire line, L = 4×10⁻⁷ ln(D/r′)
- Flux linkages of one conductor in a group
- Inductance of a 3-φ line with equilateral spacing (prove L<sub>a</sub> = L<sub>b</sub> = L<sub>c</sub>)
- Capacitance of a 3-φ line with equilateral spacing
- **Effect of earth on line capacitance** (method of images; earth modifies r to r(1 + D²/4h²)<sup>½</sup>)
- **Capacitance grading** (why unequal stress is bad + derivation with 3 dielectrics); intersheath grading
- Capacitance of a 3-core cable, C<sub>N</sub> = C<sub>e</sub> + 3C<sub>c</sub>, and measuring C<sub>e</sub> and C<sub>c</sub>
- Equal-area criterion: derivation (∫(P<sub>m</sub> − P<sub>e</sub>)dδ = 0), advantages and limits
- Multi-machine swing equation (coherent machines → H<sub>eq</sub>)
- Sag calculation, equal supports (S = wl²/8T) and unequal supports (x<sub>1</sub> = l/2 − Th/wl)

**Short**
- Bundled conductor: what it is and why it is used · composite vs bundled · Al vs Cu (which is better and why)
- Skin effect and proximity effect · define inductance · power angle
- Underground cable: definition, requirements, advantages and drawbacks, **construction of a 3-core cable with figure** (teacher: *"11.1 figure important"*)
- Thermal resistance · sag · stringing chart · main components of an overhead line
- Types of insulators (pin < 33 kV, suspension > 33 kV, strain, shackle), desirable properties, **causes of insulation failure** (asked twice), how breakdown happens in a pin-type insulator
- Types of cable faults (open-circuit / short-circuit / earth fault tables) · Megger
- FACTS devices and applications · series and shunt compensation (X′ = X − X<sub>c</sub> and its 4 benefits)

---

## 🟢 TIER 3: Only if you have time left
- Classification of cables by voltage; laying methods (direct burial, draw-in, solid system)
- Line supports: wooden, RCC, steel poles, towers; conductor materials
- Steady-state stability · factors affecting stability · numerical solution of the swing equation
- Power quality (sags, swells, harmonics, flicker): it is in the syllabus but **never asked**
- Travelling-wave pulse question (Dec-2021 6c): **out of current syllabus, skip it**
- Kothari Example 3.3: teacher said *"Not necessary"*

---

## Chapter-wise article lists the teacher gave in class

| Chapter | Teacher's instruction (from lecture notes) |
|---|---|
| **Ch-2 Inductance** (Kothari) | Art 2.2 define inductance · Art 2.5 description · **Art 2.7 derivation + examples** · Art 2.10 bundled · Art 2.12 skin/proximity · *"Find D<sub>m</sub>, D<sub>s</sub> type math from Example, Exercise"* |
| **Ch-3 Capacitance** (Kothari) | Art 3.1 – 3.7 · **Examples 3.1, 3.2 → MUST** · Example 3.3 → not necessary · *"avoid extremely complex"* |
| **Ch-11 Cables** (Mehta) | **11.1 (figure important)**, 11.3, 11.6, 11.7, 11.8, 11.9, 11.10, 11.12, 11.13, 11.17, 11.20, 11.21, 11.22 · maths from Examples + Exercises |
| **Ch-8 Overhead line** (Mehta) | Art 8.1 – 8.15 (pin & suspension insulators marked ★★) · maths from Examples + Exercises |
| **Ch-12 Stability** (Kothari) | Swing equation **derivation (in exam)**, power-angle curve, multi-machine, equal-area criterion, sudden increase in input |

---

## If you only have ONE day

| Time | Do this |
|---|---|
| 1.5 h | D1 + D5 (capacitance & inductance, unsymmetrical, with transposition): they share the same steps, so learn them together |
| 1 h | D2 composite conductor + M4 Pheasant + M9 500 kV bundle + M3 telephone line |
| 1.5 h | Cables: D4 stress, M8 economical size, M10, M11, belted cable, M5 Murray, M6 Varley |
| 1.5 h | Overhead: S2 + M1 (all 4 string maths, one formula), M7 sag (3 types), S3 + S4 corona/CDV |
| 1.5 h | Stability: D3 swing equation, S5 P–δ sudden increase, M2 (E′, P<sub>max</sub>), HVDC economics + types |
| 1 h | Read `05_Short_Questions_and_Definitions.md` + `06_Formula_Sheet.md` twice |

**Exam-hall strategy:** In Part A pick the question that contains the **unsymmetrical-spacing derivation** and/or the **telephone/bundled maths**. In Part B pick the **string-efficiency / sag** question and the **stability** question. All four types appear in every paper.
