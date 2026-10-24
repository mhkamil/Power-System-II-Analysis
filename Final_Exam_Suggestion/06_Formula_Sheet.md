# One-Page Formula Sheet (read this in the last 30 minutes)

## Inductance (Ch-2)
| Item | Formula |
|---|---|
| Internal inductance | L<sub>int</sub> = ½ × 10⁻⁷ H/m |
| Between D₁, D₂ | L₁₂ = 2×10⁻⁷ ln(D₂/D₁) H/m |
| GMR solid conductor | r′ = 0.7788 r = r e<sup>−¼</sup> |
| 1-φ two-wire | L = 4×10⁻⁷ ln(D/r′) H/m = 0.921 log(D/r′) mH/km (loop) |
| Composite | L = 2×10⁻⁷ ln(D<sub>m</sub>/D<sub>s</sub>); D<sub>m</sub> = ᵐⁿ√(∏D<sub>ij′</sub>), D<sub>s</sub> = ⁿ²√(∏D<sub>ij</sub>) |
| 3-φ equilateral | L = 2×10⁻⁷ ln(D/r′) H/m/phase = 0.4605 log(D/r′) mH/km |
| 3-φ unsymmetrical (transposed) | L = 2×10⁻⁷ ln(D<sub>eq</sub>/r′), D<sub>eq</sub> = ∛(D₁₂D₂₃D₃₁) |
| Flat spacing D, D, 2D | D<sub>eq</sub> = D·∛2 = 1.26D |
| Bundle, 2 conductors | D<sub>s</sub><sup>b</sup> = √(D<sub>s</sub>d) |
| Bundle, 3 conductors | D<sub>s</sub><sup>b</sup> = ∛(D<sub>s</sub>d²) |
| Bundle, 4 conductors | D<sub>s</sub><sup>b</sup> = 1.09 ⁴√(D<sub>s</sub>d³) |
| Mutual (telephone) | M = 2×10⁻⁷ ln[(D₁₄D₂₃)/(D₁₃D₂₄)] H/m; V = ωMI |
| Reactance | X<sub>L</sub> = 2πfL; X<sub>pu</sub> = X/(kV²/MVA) |

## Capacitance (Ch-3); k = ε₀ε<sub>r</sub>, ε₀ = 8.854×10⁻¹²
| Item | Formula |
|---|---|
| Field of a line charge | E = q/(2πkx); V₁₂ = (q/2πk) ln(D₂/D₁) |
| 1-φ line-to-line | C<sub>ab</sub> = πk/ln(D/r) F/m = 0.0121/log(D/r) µF/km |
| 1-φ to neutral | C<sub>n</sub> = 2C<sub>ab</sub> = 0.0242/log(D/r) µF/km |
| 3-φ (equilateral / transposed) | C<sub>n</sub> = 2πk/ln(D<sub>eq</sub>/r) = 0.0242/log(D<sub>eq</sub>/r) µF/km (use r, NOT r′) |
| Charging current | I<sub>c</sub> = ωC<sub>n</sub>V<sub>ph</sub> A/km; Q = 3V<sub>ph</sub>I<sub>c</sub> |
| Effect of earth (1-φ) | C<sub>ab</sub> = πk/ln[D/(r√(1 + D²/4h²))] |

## Cables (Ch-11)
| Item | Formula |
|---|---|
| Insulation resistance | R = (ρ/2πl) ln(r₂/r₁) = (ρ/2πl) ln(D/d) |
| Capacitance | C = 2πε₀ε<sub>r</sub>/ln(D/d) F/m = ε<sub>r</sub>l/(41.4 log(D/d)) × 10⁻⁹ F |
| Stress at x | g = V/(x ln(D/d)) (g ∝ 1/x) |
| g<sub>max</sub> / g<sub>min</sub> | g<sub>max</sub> = 2V/(d ln(D/d)); g<sub>min</sub> = 2V/(D ln(D/d)); g<sub>max</sub>/g<sub>min</sub> = D/d |
| Economical size | D = 2.718 d; d = 2V/g<sub>max</sub> (V = peak phase voltage) |
| Capacitance grading | ε₁d = ε₂d₁ = ε₃d₂; V = (g<sub>max</sub>/2)[d ln(d₁/d) + d₁ ln(d₂/d₁) + d₂ ln(D/d₂)] |
| Intersheath grading | g<sub>1max</sub> = 2V₁/(d ln(d₁/d)), g<sub>2max</sub> = 2V₂/(d₁ ln(d₂/d₁)), … |
| 3-core cable | C₁ (bunched) = 3C<sub>e</sub>; C₂ = C<sub>e</sub> + 2C<sub>c</sub>; C<sub>N</sub> = C<sub>e</sub> + 3C<sub>c</sub>; I<sub>c</sub> = ωC<sub>N</sub>V<sub>ph</sub> |
| Thermal resistance | S = kl/A; dielectric S = (k/2π) ln(r₂/r₁); I = √(t/(nRS)) |
| Murray loop | X = [Q/(P + Q)] × loop resistance; distance = X/(Ω per m) |
| Varley loop (P = Q) | X = (loop − S)/2; general balance: (S + X)/(loop − X) = ratio of the fixed arms on those sides |

## Overhead lines (Ch-8)
| Item | Formula |
|---|---|
| String (3 discs) | V₂ = V₁(1 + m); V₃ = V₁(1 + 3m + m²); general V<sub>n+1</sub> = V<sub>n</sub> + m(V₁ + … + V<sub>n</sub>) |
| String efficiency | η = V<sub>ph</sub>/(n·V<sub>bottom</sub>) × 100 % |
| Sag, equal supports | S = wl²/(8T), T = breaking load/SF |
| Sag, unequal supports | x₁ = l/2 − Th/(wl); x₂ = l/2 + Th/(wl); S<sub>i</sub> = wx<sub>i</sub>²/(2T) |
| Wind / ice | w<sub>ice</sub> = density × π t(d + t); w<sub>wind</sub> = p × (d + 2t); w<sub>t</sub> = √((w + w<sub>ice</sub>)² + w<sub>wind</sub>²); vertical sag = S·(w + w<sub>ice</sub>)/w<sub>t</sub> |
| Critical disruptive voltage | V<sub>c</sub> = m₀g₀δr ln(d/r) kV/phase, g₀ = 21.1 kV/cm rms, δ = 3.92b/(273 + t) |
| Visual critical voltage | V<sub>v</sub> = m<sub>v</sub>g₀δr(1 + 0.3/√(δr)) ln(d/r) |
| Corona loss (Peek) | P = 242.2 (f + 25)/δ · √(r/d) (V<sub>ph</sub> − V<sub>c</sub>)² × 10⁻⁵ kW/km/phase |

## Stability (Ch-12)
| Item | Formula |
|---|---|
| Swing equation | M d²δ/dt² = P<sub>m</sub> − P<sub>e</sub> = P<sub>a</sub>; M = GH/(πf) |
| Per unit | (H/πf) d²δ/dt² = P<sub>m</sub> − P<sub>max</sub> sin δ |
| Power transfer | P<sub>e</sub> = (|E||V|/X) sin δ; P<sub>max</sub> = |E||V|/X |
| E′ behind x′<sub>d</sub> | find θ from P = V<sub>t</sub>V sin θ/X<sub>t→bus</sub>; I = (V<sub>t</sub> − V)/jX; E′ = V<sub>t</sub> + jx′<sub>d</sub>I |
| Fault at the middle of a line | star–delta: X<sub>transfer</sub> = (ab + bc + ca)/(arm to ground) |
| Equal area | ∫<sub>δ₀</sub><sup>δ</sup>(P<sub>m</sub> − P<sub>e</sub>)dδ = 0 → A₁ = A₂ |
| Coherent machines | H<sub>eq</sub> = (G₁H₁ + G₂H₂)/G<sub>sys</sub> |

## Unit traps
- 1 mile = 1.609 km · 1 ft = 0.3048 m · 1 inch = 2.54 cm
- Use **r′ for inductance** and **r for capacitance**
- Cable g<sub>max</sub> with an rms voltage gives an rms stress. For the "economical size" problem use the **peak phase voltage** (V<sub>L</sub>√2/√3)
- Line voltage → phase voltage: ÷√3
