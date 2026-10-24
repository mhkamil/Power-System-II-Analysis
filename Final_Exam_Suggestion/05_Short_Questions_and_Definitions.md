# Short Questions & Definitions (1 to 5 marks each, ready-to-write answers)

Ordered by how often they were asked. ⭐ = repeat count.

---

## Ch-2 / Ch-3: Line parameters

**Transposition: what it is and why it is used** ⭐⭐⭐⭐⭐
Transposition means exchanging the positions of the three phase conductors at regular intervals (every one-third of the length) so that each conductor occupies each position for an equal distance (Section 1: a-b-c → Section 2: c-a-b → Section 3: b-c-a; draw this).
*Why:* with unsymmetrical spacing the flux linkages, and so the inductance and capacitance, of each phase are different (the middle conductor links more flux). The result is unequal voltage drops, an unbalanced receiving-end voltage, extra losses, and interference with nearby telephone lines. Transposition makes **L<sub>a</sub> = L<sub>b</sub> = L<sub>c</sub>** and **C<sub>a</sub> = C<sub>b</sub> = C<sub>c</sub>**, so the line becomes balanced (D<sub>eq</sub> = ∛(D₁₂D₂₃D₃₁)).

**Define inductance**
Inductance is the flux linkage per ampere: **L = λ/I** (H). From e = dλ/dt = (dλ/di)(di/dt) = L di/dt, so L = dλ/di. A transmission line carries AC, which produces a varying flux and therefore self and mutual inductance.

**Skin effect**
In AC the current is not distributed uniformly over the conductor cross-section. It tends to concentrate near the surface, so the effective area falls and the **AC resistance is higher than the DC resistance**. It increases with frequency, conductor size and permeability. DC has no skin effect (f = 0).
**Proximity effect**: a non-uniform current distribution caused by the alternating flux of nearby conductors. It also raises the resistance.

**Bundled conductor: what it is and why it is used**
Two or more sub-conductors per phase, spaced apart (e.g. 0.3–0.5 m) and held by spacers. Why: increases the effective GMR → **reduces the inductance (reactance) → more power transfer**; increases the effective radius → **reduces the surface gradient → less corona loss, radio interference and audible noise**; increases capacitance → higher surge-impedance loading.

**Composite vs bundled conductor**
Composite: the strands are in contact and twisted together, often of two metals (e.g. ACSR = Al + steel), acting as one conductor. Bundled: separate conductors of the **same phase, spaced apart** (not in contact) by spacers, used at EHV mainly to cut corona and reactance.

**Aluminium vs copper: which is superior?**
Copper has higher conductivity and strength. **Aluminium is preferred for overhead lines** because it is cheaper and much lighter (about ½ the weight for the same resistance). Its larger diameter for the same resistance also **reduces corona**, and steel reinforcement (ACSR) gives the strength. Drawbacks of Al: lower tensile strength, higher expansion coefficient, larger sag and swing.

**Effect of earth on capacitance**
The earth is treated as an equipotential plane and replaced by **image conductors** at the same depth below the surface with opposite charge (method of images). The earth increases the line capacitance: in the formula r is replaced by r(1 + D²/4h²)<sup>½</sup>. **C<sub>ab</sub> = πk / ln[D/(r(1 + D²/4h²)<sup>½</sup>)]**. For h ≫ D the effect is negligible.

**GMD and GMR**: D<sub>m</sub> = mutual geometric mean distance (between conductors); D<sub>s</sub> = self GMD = GMR = r′ = 0.7788r for a solid conductor.

---

## Ch-8: Overhead lines

**String efficiency: definition** ⭐⭐⭐⭐⭐
The ratio of the voltage across the whole string to the product of the number of discs and the voltage across the disc nearest the conductor: **η = V/(n × V<sub>n</sub>) × 100 %**. The voltage is unequal because of the **shunt capacitance** between each disc's metal cap/pin and the earthed tower. (For improvement methods see `04_Derivations_Guide.md` D6: longer cross-arm, capacitance grading, guard ring.)

**Critical disruptive voltage: definition and significance** ⭐⭐⭐⭐
The minimum phase-neutral voltage at which corona starts, i.e. the potential gradient at the conductor surface equals the breakdown strength of air (g₀ = 30 kV/cm peak = 21.1 kV/cm rms).
**V<sub>c</sub> = m₀ g₀ δ r ln(d/r) kV/phase** (m₀ = irregularity factor, δ = air density factor = 3.92b/(273 + t)).
*Significance:* the line's operating voltage must stay below V<sub>c</sub> to avoid corona loss. It is used to choose the conductor size and spacing. The **visual critical voltage** V<sub>v</sub> = m<sub>v</sub> g₀ δ r(1 + 0.3/√(δr)) ln(d/r) is where the glow becomes visible.

**Corona: definition, theory, advantages/disadvantages, reducing it** ⭐⭐⭐⭐
*Definition:* a violet glow, hissing sound and ozone production around a conductor when the surface gradient exceeds the breakdown strength of air.
*Theory:* air always has some free ions (from UV and cosmic rays). At high gradient these electrons gain enough speed to knock more electrons off neutral molecules by collision. This ionisation spreads (an avalanche) around the conductor, making the air conducting and luminous.
*Advantages:* the air around the conductor becomes conducting, so the virtual diameter increases and the stress falls; it reduces the effect of transients and surges (acts like a safety valve).
*Disadvantages:* power loss; ozone, which corrodes the conductor; non-sinusoidal current and third harmonics → interference with communication lines.
*Reducing it:* increase the conductor size/diameter (ACSR, hollow conductors); increase the spacing between conductors; use bundled conductors.
*Factors affecting it:* atmosphere, conductor size and surface condition, spacing, line voltage.

**Sag** ⭐⭐: the difference in level between the points of support and the lowest point of the conductor. Sag is necessary so that the tension stays safe and temperature changes do not over-stress the conductor. S = wl²/8T.

**Stringing chart**: a graph of **sag and tension against temperature** for a given span. It is used during erection so the conductor is strung with the correct sag/tension for the ambient temperature.

**Main components of an overhead line**: conductors, supports (poles/towers), insulators, cross-arms, plus earth wire, lightning arresters, fuses/isolators, guard wires, vibration dampers, danger plates.

**Types of insulators**: Pin type (up to 33 kV) · Suspension type (above 33 kV, discs in a string; cheaper at high voltage, flexible, a failed disc is easy to replace, can add discs) · Strain type (at dead ends, sharp curves, river crossings) · Shackle type (LV distribution).

**Desirable properties of insulators**: high mechanical strength; high electrical resistance (low leakage); high relative permittivity (high dielectric strength); non-porous, free from impurities and cracks; high ratio of puncture strength to flashover voltage; unaffected by temperature changes.

**Causes of insulation failure** ⭐⭐: cracking of the insulator (temperature stress, unequal expansion); defective/porous material; improper glazing (absorbs moisture); flash-over (arc heating); mechanical stresses (bad workmanship); short circuit by birds/branches; dust and pollution.

**How breakdown happens in a pin-type insulator**: two ways. (i) **Flash-over**: an arc between the line conductor and the earthed pin through the surrounding air (the insulator survives). (ii) **Puncture**: the discharge goes through the body of the insulator, which is permanently damaged. Safety factor = puncture strength/flash-over voltage (kept high, about 10).

**Supports used for distribution (up to 11 kV)**: wooden poles (cheap, rural, up to about 20 kV, 50 m span), RCC poles (stronger, little maintenance, costly to transport), steel tubular poles (higher strength, longer span). Steel towers are used for long-distance HV transmission.

**Line support requirements**: high mechanical strength, light weight, low cost, long life, easy access to conductors.

---

## Ch-11: Cables

**Underground cable: definition and requirements**
A cable is one or more insulated conductors with a protective covering, laid underground.
*Requirements:* conductor of standard annealed Cu/Al with high conductivity and the right size (carries the load without overheating or excessive voltage drop); proper insulation thickness for safety and reliability; suitable mechanical protection; chemically and physically stable materials.
*Advantages:* safer (not exposed to storms or lightning), lower maintenance, fewer faults, smaller voltage drop, better appearance. *Drawbacks:* much higher installation cost, insulation problems at high voltage. *Used in* thickly populated areas, near power stations and substations.

**Construction of a 3-core cable (with figure)** ⭐ teacher: "figure important"
From inside out: **cores/conductors → insulation (impregnated paper, varnished cambric, rubber) → metallic sheath (lead/Al; keeps out moisture, gases, acids) → bedding (jute/fibrous; protects the sheath from corrosion and mechanical injury) → armouring (steel wires/tape; mechanical protection) → serving (jute; protects the armour from the atmosphere)**. Draw concentric layers labelled (i) to (vi).

**Classification of cables by voltage**: low-tension (LT) up to 1 kV · high-tension (HT) up to 11 kV · super-tension (ST) 22–33 kV · extra-high-tension (EHT) 33–66 kV · extra-super-voltage beyond 132 kV. For 3-phase: belted cables (up to 11 kV), screened cables (H-type and S.L.-type, up to 66 kV), pressure cables (oil-filled and gas-pressure, beyond 66 kV).

**Grading of cables**: the process of making the dielectric stress uniform across the insulation. *Why non-uniform stress is undesirable:* thicker insulation is needed (bigger, costlier cable) and the insulation near the core may break down. Methods: **capacitance grading** (layers of different ε, highest ε near the core) and **intersheath grading** (metallic intersheaths held at suitable potentials).

**Thermal resistance**: the opposition to heat flow. **S = temperature difference/heat flow per second = k·l/A**, k = thermal resistivity (thermal Ω-m). For a cable dielectric S = (k/2π) ln(r₂/r₁). Permissible current I = √(t/(nRS)). Current-carrying capacity depends on the maximum permissible temperature rise (losses: Cu loss, dielectric loss, sheath and armour loss). Safe conductor temperature: 60 °C for armoured cables, 50 °C for lead-sheathed cables (as given in your class notes).

**Types of cable faults**: (i) **open-circuit**: a break in the conductor (Megger reads ∞ between the conductor and the far end). (ii) **short-circuit**: insulation failure between two conductors (Megger reads 0 between cores). (iii) **earth fault**: a conductor makes contact with earth/sheath (Megger reads 0 between core and earth). Located by the **Murray loop** (X = Q/(P+Q) × loop) and the **Varley loop** tests.

**Megger**: a portable instrument (hand generator + ohmmeter) used to measure insulation resistance.

**Monopolar link (HVDC)**: uses **one conductor** (usually negative polarity) with **earth or sea as the return path**. Cheap but has earth-current problems. Bipolar = two conductors (+ and −), mid-point earthed, can run monopolar if one pole fails. Homopolar = two or more conductors of the same polarity with earth return.

---

## Ch-12: Stability

**Power angle (load angle) δ**: the angle between the rotor emf E (rotor axis) and the terminal/infinite-bus voltage V. P<sub>e</sub> = (|E||V|/X) sin δ; maximum power at δ = 90°.

**Stability**: the ability of a power system to return to steady operation (synchronism) after a disturbance. *Steady-state stability*: after small, gradual changes. *Transient stability*: after large, sudden disturbances (faults, switching, load loss).

**Equal-area criterion**: a graphical method to judge the transient stability of a single machine connected to an infinite bus (or any 2-machine system) without solving the swing equation. The system is stable if the accelerating area **A₁ = decelerating area A₂** can be met: **∫<sub>δ₀</sub><sup>δ</sup>(P<sub>m</sub> − P<sub>e</sub>)dδ = 0**.

**Inertia constant H**: stored kinetic energy at synchronous speed per MVA of rating (MJ/MVA). M = GH/(πf).

**Factors affecting stability**: line reactance (less is better: use series capacitors or parallel lines), fast fault clearing (high-speed breakers, auto-reclosure), excitation (high E), generator inertia H, and the voltage level.

---

## HVDC / FACTS / Compensation

**HVDC: definition and economics** ⭐⭐⭐
High-voltage DC transmission: AC is converted to DC by a converter, transmitted at high DC voltage, then inverted back to AC.
*Economics:* HVDC terminal equipment (converters) is very expensive, but the **line is cheaper** (2 conductors or 1 vs 3, smaller towers, thinner conductors, no skin effect, less corona, no reactive power or charging current). AC cost rises faster with distance, so beyond the **break-even distance (about 600–800 km overhead, about 50 km for cables)** HVDC is cheaper. Draw cost vs distance: the HVAC line starts low but rises steeply; the HVDC line starts high but rises slowly; they cross at the break-even point.
*Advantages:* links grids of different frequency (asynchronous), less corona, fewer conductors, no stability limit, easy power control. *Disadvantages:* costly converters, harmonics, reactive power needed at the converters, DC circuit breakers are difficult.
*Bangladesh:* HVDC back-to-back link at Bheramara for import from India.

**Types of HVDC links**: monopolar, bipolar, homopolar (see above) + back-to-back.

**FACTS devices and applications**
FACTS = flexible AC transmission systems: power-electronic controllers that increase line loading capability and controllability.
- **SVC** (static VAR compensator): shunt thyristor-controlled reactor/capacitor; voltage control.
- **STATCOM**: shunt VSC-based; fast reactive-power support and voltage stability.
- **TCSC** (thyristor-controlled series capacitor): changes the line reactance → power-flow control, damping.
- **SSSC**: series VSC; injects a series voltage.
- **UPFC** (unified power flow controller): series + shunt; controls V, Z and angle (P and Q flow).
*Applications:* more power transfer, better transient stability, damping of oscillations, voltage control, power-flow control.

**Compensation**
*Load compensation:* managing reactive power at the load to improve power quality (power factor, voltage regulation, load balancing).
*Line compensation:* changing the line's characteristics. **Series capacitor:** X′ = X − X<sub>C</sub> → (i) smaller voltage drop, (ii) prevents voltage collapse, (iii) more steady-state power transfer, (iv) better transient stability. **Shunt reactors** absorb the line's charging VAR at light load (Ferranti effect); **shunt capacitors** supply VAR at heavy load.
Loading capability limits: dielectric (insulation), thermal capability, stability.
