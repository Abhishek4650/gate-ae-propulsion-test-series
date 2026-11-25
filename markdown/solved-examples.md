# GATE AE Propulsion: Solved Examples

Last updated 25 Nov 2026

## How to use this booklet

Each topic below has solved examples of every question type GATE AE asks in propulsion, ordered from basic to advanced. Cover the solution, attempt the question, then check your working step by step.

When a topic feels solid, test yourself with [GATE AE Propulsion Test Series: Question Papers](question-papers.md) or the timed online version at [Propulsion Mock Tests](https://abhishek4650.github.io/gate-ae-propulsion-test-series/).

### GATE question types and marking

| Type | What you do | Marks | Negative marking |
| --- | --- | --- | --- |
| MCQ | Pick the one correct option | 1 or 2 | 1/3 mark (1-mark Q), 2/3 mark (2-mark Q) |
| MSQ | Pick every correct option (one or more) | 1 or 2 | None, but no partial credit |
| NAT | Type a number; accepted within a range | 1 or 2 | None |

### Standard data (unless a question says otherwise)

- Air: γ = 1.4, cp = 1.005 kJ/kg·K, R = 287 J/kg·K
- Hot combustion gas: γg = 4/3, cpg = 1.148 kJ/kg·K
- g0 = 9.81 m/s²
- Component work and heat always use stagnation (total) temperatures, written with subscript 0 (T01, T02 …); velocities come from static temperatures.

### Notation (matches your notes)

- ci = flight speed, cj = jet speed, f = ṁf/ṁa (fuel–air ratio), B = bypass ratio (β in your notes)
- Axial machines: Ca = axial velocity, U = blade speed, α = absolute flow angle, β = relative flow angle, both measured from the axial direction
- φ = Ca/U (flow coefficient), ψ = Δh0/U² (blade loading), R = degree of reaction, λ = work-done factor, σ = slip factor
- Axial compressor stations: 1 rotor inlet, 2 rotor exit, 3 stator exit. Axial turbine stations: 1 nozzle inlet, 2 nozzle exit (rotor inlet), 3 rotor exit.

### Where each syllabus item is covered

| GATE 2027 syllabus item (Section 5, Propulsion) | Topic here |
| --- | --- |
| Basics of thermodynamics | 1 |
| Brayton cycle | 2 |
| Thrust, efficiency and range | 3 |
| Intakes and nozzles (non-rotating components) | 4, 5 |
| Combustors: types, combustion, stoichiometric fuel–air ratio; afterburners | 6 |
| Ramjet, turbojet, turbofan, turboprop and turboshaft performance | 7 |
| Axial compressors: work, efficiency, reaction, multistaging | 8 |
| Centrifugal compressors: inducer, impeller, diffuser | 9 |
| Axial turbines; turbine blade cooling (special topic) | 10 |
| Compressor–turbine matching (special topic) | 11 |
| Rockets: thrust, specific impulse, multistaging, solid and liquid propellants | 12 |

Syllabus source: [GATE 2027 syllabus PDF, IIT Madras](https://govtserviceinfo.com/wp-content/uploads/2026/09/GATE2027-Syllabus.pdf).

## 1. Thermodynamics basics

Stagnation properties, isentropic relations and the steady-flow energy equation sit underneath every later topic. These relations solve most basic questions:

- T0/T = 1 + ((γ − 1)/2)·M²
- P0/P = (T0/T)^(γ/(γ − 1))
- cp = γR/(γ − 1) and cv = R/(γ − 1)
- s2 − s1 = cp·ln(T2/T1) − R·ln(p2/p1)
- Adiabatic machine: w = h01 − h02 = cp(T01 − T02)

### Example 1.1 · NAT · 1 mark · Stagnation pressure

An aircraft flies at Mach 0.8 where T = 223.3 K and p = 26.5 kPa. Find the stagnation pressure (kPa) of the oncoming air. Take γ = 1.4.

**Solution.** T0/T = 1 + 0.2 × 0.8² = 1.128, so T0 = 251.9 K. P0/P = 1.128^3.5 = 1.524, so P0 = 26.5 × 1.524 = 40.4 kPa.

**Answer: 40.4 kPa (range 40.2 to 40.6)**

### Example 1.2 · MCQ · 1 mark · γ from degrees of freedom

At high temperature the vibrational modes of a diatomic gas become active, giving it 7 degrees of freedom. Its ratio of specific heats is:

- (A) 1.400
- (B) 1.286
- (C) 1.333
- (D) 1.667

**Solution.** γ = 1 + 2/f = 1 + 2/7 = 1.286. With f = 5 (translation and rotation only) you get the familiar 1.4. A monatomic gas (f = 3) gives 1.667.

**Answer: (B)**

### Example 1.3 · NAT · 1 mark · cp of hot gas

Combustion gases have R = 287 J/kg·K and γ = 4/3. Find cp in kJ/kg·K.

**Solution.** cp = γR/(γ − 1) = (4/3)(287)/(1/3) = 4 × 287 = 1148 J/kg·K. This is where the standard hot-gas value of 1.148 kJ/kg·K comes from.

**Answer: 1.148 kJ/kg·K (range 1.14 to 1.15)**

### Example 1.4 · NAT · 2 marks · Entropy rise in a compressor

Air is compressed adiabatically from 300 K, 100 kPa to 600 K, 800 kPa. Find the specific entropy rise in J/kg·K. Use cp = 1005 J/kg·K and R = 287 J/kg·K.

**Solution.**

Δs = cp·ln(T2/T1) − R·ln(p2/p1) = 1005 ln 2 − 287 ln 8 = 696.6 − 596.8 = 99.8 J/kg·K.

The rise is positive in an adiabatic process, so the compression is irreversible. For comparison, the isentropic exit temperature is 300 × 8^0.2857 = 543.4 K, giving ηc = 243.4/300 = 0.811.

**Answer: 99.8 J/kg·K (range 98 to 102)**

### Example 1.5 · NAT · 1 mark · Steady-flow work

An adiabatic compressor raises air from T01 = 288 K to T02 = 520 K at 20 kg/s. Find the power input in MW. Take cp = 1.005 kJ/kg·K.

**Solution.** With q = 0, the steady-flow energy equation gives w = cp(T02 − T01) = 1.005 × 232 = 233.2 kJ/kg. Power = 20 × 233.2 = 4663 kW. Using stagnation temperatures already accounts for kinetic energy.

**Answer: 4.66 MW (range 4.60 to 4.72)**

### Example 1.6 · MSQ · 1 mark · Insulated duct with friction

Air flows steadily through an insulated duct with wall friction and no work transfer. Which statements are correct?

- (A) Stagnation temperature stays constant
- (B) Stagnation pressure stays constant
- (C) Stagnation pressure falls along the duct
- (D) Specific entropy rises along the duct

**Solution.** With q = 0 and w = 0, h0 and hence T0 stay constant, so (A) holds. Friction is irreversible, so s rises, which is (D). At constant T0, Δs = −R ln(P02/P01) > 0 forces P02 < P01, which is (C).

**Answer: (A), (C), (D)**

## 2. Brayton cycle

The gas turbine cycle is two isentropic processes joined by two constant-pressure ones. Write t = T3/T1 and c = r^((γ − 1)/γ), where r is the pressure ratio.

- Ideal efficiency: η = 1 − 1/c
- Ideal net work: Wnet/(cp·T1) = (c − 1)(t/c − 1)
- Maximum work when c = √t, i.e. T2 = T4; then Wmax = cp·T1(√t − 1)²
- Perfect heat exchanger: η = 1 − c/t
- Real components: ΔTc = T1(c − 1)/ηc and ΔTt = ηt·T3(1 − 1/c)
- Polytropic: T02/T01 = r^((γ − 1)/(γ·η∞c)) for compression, T03/T04 = r^(η∞t(γ − 1)/γ) for expansion

### Example 2.1 · NAT · 1 mark · Ideal cycle efficiency

An ideal Brayton cycle uses air (γ = 1.4) with a pressure ratio of 10. Find the thermal efficiency in percent.

**Solution.** c = 10^0.2857 = 1.931. η = 1 − 1/1.931 = 0.482.

**Answer: 48.2% (range 48.0 to 48.4)**

### Example 2.2 · NAT · 2 marks · Maximum specific work

In an ideal Brayton cycle, T1 = 300 K and T3 = 1200 K. Find the maximum net specific work in kJ/kg. Take cp = 1.005 kJ/kg·K and γ = 1.4.

**Solution.** t = 1200/300 = 4. Work is maximum when c = √t = 2, which makes T2 = T4 = 600 K. The pressure ratio is then 2^3.5 = 11.3. Wmax = cp·T1(√t − 1)² = 1.005 × 300 × 1² = 301.5 kJ/kg, and the efficiency there is 1 − 1/2 = 50%.

**Answer: 301.5 kJ/kg (range 300 to 303)**

### Example 2.3 · NAT · 2 marks · Real cycle with component efficiencies

A gas turbine has T1 = 288 K, pressure ratio 8, ηc = 0.85, T3 = 1200 K and ηt = 0.88. Treat the gas as air throughout (cp = 1.005 kJ/kg·K, γ = 1.4) and neglect pressure losses and fuel mass. Find the thermal efficiency in percent.

**Solution.**

1. c = 8^0.2857 = 1.8114.
2. Compressor: ΔTc = 288 × 0.8114/0.85 = 274.9 K, so T2 = 562.9 K and Wc = 276.3 kJ/kg.
3. Turbine: T4' = 1200/1.8114 = 662.5 K, so ΔTt = 0.88 × 537.5 = 473.0 K and Wt = 475.4 kJ/kg.
4. Wnet = 475.4 − 276.3 = 199.1 kJ/kg. Heat added = 1.005 × (1200 − 562.9) = 640.2 kJ/kg.
5. η = 199.1/640.2 = 0.311.

The ideal cycle at this pressure ratio gives 44.8%, so component losses cost almost 14 points. The back-work ratio is 276.3/475.4 = 0.58, which is why gas turbines are so sensitive to component efficiency.

**Answer: 31.1% (range 30.6 to 31.6)**

### Example 2.4 · NAT · 1 mark · Polytropic to isentropic efficiency

A compressor with pressure ratio 20 has a polytropic efficiency of 0.90. Find its isentropic efficiency (γ = 1.4).

**Solution.** Actual temperature ratio = 20^(0.2857/0.90) = 20^0.3175 = 2.588. Isentropic ratio = 20^0.2857 = 2.354. ηc = (2.354 − 1)/(2.588 − 1) = 0.852.

For a compressor the isentropic efficiency is lower than the polytropic value, and the gap widens as pressure ratio rises. For a turbine the reverse holds.

**Answer: 0.852 (range 0.845 to 0.858)**

### Example 2.5 · MCQ · 1 mark · Heat exchanger

An ideal Brayton cycle with a perfect heat exchanger runs with T1 = 300 K, T3 = 1200 K and pressure ratio 4 (γ = 1.4). Its thermal efficiency is closest to:

- (A) 33%
- (B) 48%
- (C) 63%
- (D) 75%

**Solution.** c = 4^0.2857 = 1.486 and t = 4. With a perfect heat exchanger, η = 1 − c/t = 1 − 1.486/4 = 0.628. Without it, η = 1 − 1/1.486 = 0.327, which is distractor (A). The exchanger only helps while T4 > T2, that is, while c < √t.

**Answer: (C)**

### Example 2.6 · MSQ · 2 marks · Brayton cycle statements

For an ideal simple Brayton cycle, which statements are correct?

- (A) Thermal efficiency depends only on pressure ratio and γ
- (B) Net specific work is maximum when compressor exit temperature equals turbine exit temperature
- (C) Adding a heat exchanger raises efficiency at every pressure ratio
- (D) Raising T3 at a fixed pressure ratio raises the thermal efficiency

**Solution.** (A) is true because η = 1 − 1/c contains no temperature. (B) is true because c = √t gives T2 = T4. (C) is false: above c = √t, T4 < T2 and the exchanger would heat the exhaust instead. (D) is false: higher T3 raises the specific work, not the ideal efficiency.

**Answer: (A), (B)**

## 3. Thrust, efficiencies, TSFC and range

Thrust comes from the momentum change of the air plus any pressure imbalance at the nozzle exit. Efficiency questions then split the fuel energy into what reaches the jet and what does useful work.

- Thrust: F = (ṁa + ṁf)cj − ṁa·ci + (pe − pa)Ae
- Specific thrust Fs = F/ṁa; TSFC = ṁf/F (multiply by 3600 for kg/(N·h))
- Propulsive efficiency: ηp = 2/(1 + cj/ci) = 2α/(1 + α), with α = ci/cj
- Thermal efficiency: ηth = ½ṁa(cj² − ci²)/(ṁf·QR); overall η0 = ηp·ηth = F·ci/(ṁf·QR)
- Breguet range for a jet: R = (V/(g·TSFC))·(L/D)·ln(Wi/Wf), with TSFC in kg/(N·s)

### Example 3.1 · NAT · 1 mark · Net thrust

A turbojet takes in 50 kg/s of air at a flight speed of 250 m/s. The fuel–air ratio is 0.02 and the fully expanded jet leaves at 600 m/s. Find the net thrust in kN.

**Solution.** F = ṁa(1 + f)cj − ṁa·ci = 50 × 1.02 × 600 − 50 × 250 = 30,600 − 12,500 = 18,100 N. The term ṁa·ci is the ram (intake momentum) drag.

**Answer: 18.1 kN (range 18.0 to 18.2)**

### Example 3.2 · NAT · 2 marks · Thrust with a pressure term

A turbojet flies at 200 m/s with ṁa = 30 kg/s and f = 0.02. Its nozzle is under-expanded: jet speed 550 m/s, exit area 0.12 m², exit pressure 40 kPa above ambient. Find the total thrust in kN.

**Solution.** Momentum thrust = 30 × 1.02 × 550 − 30 × 200 = 16,830 − 6,000 = 10,830 N. Pressure thrust = (pe − pa)Ae = 40,000 × 0.12 = 4,800 N. Total F = 15,630 N.

**Answer: 15.63 kN (range 15.5 to 15.8)**

### Example 3.3 · NAT · 1 mark · Propulsive efficiency

An engine flies at 270 m/s with a jet velocity of 600 m/s. Neglecting fuel mass and pressure thrust, find the propulsive efficiency.

**Solution.** ηp = 2ci/(ci + cj) = 540/870 = 0.621. Producing the same thrust from more air at a lower jet speed would raise ηp, which is the whole case for turbofans.

**Answer: 0.621 (range 0.615 to 0.627)**

### Example 3.4 · MCQ · 1 mark · Maximum thrust power

For a fixed jet velocity cj and air mass flow, the thrust power F·ci is maximum when the flight speed ci equals:

- (A) cj
- (B) cj/2
- (C) 0
- (D) 2cj

**Solution.** Thrust power = ṁa(cj − ci)ci. Setting its derivative to zero gives ci = cj/2, where ηp = 2/(1 + 2) = 66.7%. At ci = cj the efficiency is 100% but thrust is zero; at ci = 0 thrust is largest but ηp = 0.

**Answer: (B)**

### Example 3.5 · NAT · 2 marks · TSFC and overall efficiency

An engine produces 30 kN at 250 m/s while burning 0.8 kg/s of fuel with a calorific value of 43 MJ/kg. Find the overall efficiency.

**Solution.** TSFC = 0.8/30,000 = 2.667 × 10⁻⁵ kg/(N·s) = 0.096 kg/(N·h). η0 = F·ci/(ṁf·QR) = (30,000 × 250)/(0.8 × 43 × 10⁶) = 7.5 × 10⁶/3.44 × 10⁷ = 0.218.

**Answer: 0.218 (range 0.215 to 0.221)**

### Example 3.6 · NAT · 2 marks · Breguet range

A jet aircraft cruises at 230 m/s with L/D = 16 and TSFC = 0.07 kg/(N·h). Its initial-to-final cruise weight ratio is 1.25. Find the range in km.

**Solution.**

1. TSFC = 0.07/3600 = 1.944 × 10⁻⁵ kg/(N·s), so g·TSFC = 1.9075 × 10⁻⁴ s⁻¹.
2. R = (230/1.9075 × 10⁻⁴) × 16 × ln 1.25 = 1.2058 × 10⁶ × 16 × 0.2231.
3. R = 4.305 × 10⁶ m.

Range grows with speed, L/D and fuel fraction, and falls as TSFC rises.

**Answer: 4305 km (range 4250 to 4360)**

### Example 3.7 · MSQ · 1 mark · Static (take-off) thrust

A turbojet is running on the ground (ci = 0) with a fully expanded jet. Which statements are correct?

- (A) Ram drag is zero
- (B) Propulsive efficiency is zero
- (C) Thrust ≈ ṁa(1 + f)cj
- (D) Thrust power is at its maximum

**Solution.** With ci = 0, the ram drag ṁa·ci vanishes (A) and the thrust is just the jet momentum (C). Thrust power F·ci and ηp = 2ci/(ci + cj) are both zero, so (B) is true and (D) is false.

**Answer: (A), (B), (C)**

## 4. Intakes and diffusers

An intake slows the air down while losing as little stagnation pressure as possible. The flow is adiabatic, so T0 stays constant while P0 falls.

- Intake isentropic efficiency: ηi = (T01' − Ta)/(T01 − Ta), where T01' is reached isentropically at the actual P01
- Pressure rise: P01/pa = \[1 + ηi·((γ − 1)/2)·Ma²\]^(γ/(γ − 1))
- Ram efficiency: ηram = (P01 − pa)/(P0a − pa)
- Pressure recovery: πd = P01/P0a
- Diffuser efficiency from recovery: ηd = \[πd^((γ − 1)/γ)·(1 + ((γ − 1)/2)M²) − 1\] / \[((γ − 1)/2)M²\]
- Normal shock: P02/P01 = \[(γ + 1)M²/((γ − 1)M² + 2)\]^(γ/(γ − 1)) · \[(γ + 1)/(2γM² − (γ − 1))\]^(1/(γ − 1))

### Example 4.1 · NAT · 1 mark · Pressure at the compressor face

An aircraft flies at Mach 0.8 where Ta = 223.3 K and pa = 26.5 kPa. The intake isentropic efficiency is 0.93 (γ = 1.4). Find the stagnation pressure at the compressor face in kPa.

**Solution.** P01/pa = (1 + 0.93 × 0.2 × 0.64)^3.5 = 1.1190^3.5 = 1.4824, so P01 = 26.5 × 1.4824 = 39.28 kPa. A loss-free intake would deliver the free-stream P0a = 40.40 kPa from Example 1.1, so this intake loses about 2.8%. T01 stays at 251.9 K whatever the losses.

**Answer: 39.3 kPa (range 39.1 to 39.5)**

### Example 4.2 · NAT · 1 mark · Ram efficiency

At Mach 0.85 and pa = 30 kPa, the measured stagnation pressure at the compressor face is 46 kPa. Find the ram efficiency (γ = 1.4).

**Solution.** P0a = 30 × (1 + 0.2 × 0.7225)^3.5 = 30 × 1.1445^3.5 = 48.11 kPa. ηram = (46 − 30)/(48.11 − 30) = 16/18.11 = 0.883.

**Answer: 0.883 (range 0.878 to 0.888)**

### Example 4.3 · NAT · 2 marks · Diffuser efficiency from pressure recovery

A subsonic diffuser receives air at Mach 0.85 and has a stagnation pressure recovery πd = 0.95. Find the diffuser isentropic efficiency (γ = 1.4).

**Solution.**

1. ((γ − 1)/2)M² = 0.2 × 0.7225 = 0.1445.
2. πd^0.2857 = 0.95^0.2857 = 0.98545.
3. ηd = (0.98545 × 1.1445 − 1)/0.1445 = 0.12785/0.1445 = 0.885.

A small P0 loss shows up as a large efficiency drop at low Mach numbers, because the available temperature rise is small.

**Answer: 0.885 (range 0.880 to 0.890)**

### Example 4.4 · NAT · 2 marks · Pitot intake at supersonic speed

A pitot-type intake flies at Mach 2.0 with a normal shock standing at its lip (γ = 1.4). The subsonic diffuser behind the shock has a recovery of 0.97. Find the overall stagnation pressure recovery.

**Solution.** For M = 2.0 the first bracket of the normal-shock formula is (2.4 × 4/3.6)^3.5 = 2.667^3.5 and the second is (2.4/10.8)^2.5 = 0.2222^2.5. Their product gives P02/P01 = 0.7209, with a downstream Mach number of 0.577. Overall recovery = 0.7209 × 0.97 = 0.699.

**Answer: 0.699 (range 0.69 to 0.71)**

### Example 4.5 · MCQ · 1 mark · Shock systems in supersonic intakes

At Mach 2, which intake gives the highest stagnation pressure recovery?

- (A) A single normal shock
- (B) One oblique shock followed by a normal shock
- (C) Two oblique shocks followed by a weak normal shock
- (D) All give the same recovery, since T0 is conserved

**Solution.** Shock loss rises steeply with the normal Mach number, so splitting the compression into several weak shocks keeps each loss small. At M = 2 a single normal shock recovers 0.72, while a 10° oblique shock plus a normal shock recovers about 0.87. Two oblique shocks do better still. (D) confuses T0, which is conserved, with P0, which is not.

**Answer: (C)**

### Example 4.6 · MSQ · 1 mark · What changes across an intake

For adiabatic flow with friction through a subsonic intake, which statements are correct?

- (A) T0 at the compressor face equals the free-stream T0
- (B) P0 at the compressor face is less than the free-stream P0
- (C) Static pressure rises as the air decelerates towards the compressor face
- (D) An intake efficiency of 0.93 means 7% of the static pressure is lost

**Solution.** No heat or work crosses the intake, so T0 is unchanged (A). Friction destroys stagnation pressure (B). A diffusing flow converts kinetic energy into static pressure (C). (D) is false because intake efficiency is defined on temperature (enthalpy) rise, not on pressure.

**Answer: (A), (B), (C)**

## 5. Propelling nozzles

A propelling nozzle turns stagnation enthalpy into jet velocity. Always start by comparing P04/pa with the critical pressure ratio to see whether the nozzle is choked.

- Nozzle efficiency: ηj = (T04 − T5)/(T04 − T5')
- Isentropic critical ratio: P0/Pc = ((γ + 1)/2)^(γ/(γ − 1)), which is 1.893 for air and 1.853 for γ = 4/3
- With losses: P04/Pc = 1/\[1 − (1/ηj)((γ − 1)/(γ + 1))\]^(γ/(γ − 1))
- Choked (P04/pa above critical): Tc = 2T04/(γ + 1), cj = √(γRTc), and pe = Pc > pa adds pressure thrust
- Unchoked: pe = pa and cj = √(2cp·ηj·T04\[1 − (pa/P04)^((γ − 1)/γ)\])
- Area–velocity relation: dA/A = (M² − 1)·du/u, so supersonic flow needs a diverging passage

### Example 5.1 · NAT · 1 mark · Critical pressure ratio

Find the critical pressure ratio P0/Pc for isentropic flow of combustion gas with γ = 4/3.

**Solution.** ((γ + 1)/2)^(γ/(γ − 1)) = (7/6)^4 = 1.853. For air (γ = 1.4) the same formula gives 1.893.

**Answer: 1.853 (range 1.84 to 1.86)**

### Example 5.2 · MCQ · 2 marks · Is the nozzle choked?

A convergent nozzle with ηj = 0.95 receives gas (γ = 4/3) at P04 = 200 kPa and exhausts to pa = 100 kPa. The nozzle is:

- (A) Unchoked, with exit pressure equal to 100 kPa
- (B) Choked, with exit pressure of about 104 kPa
- (C) Choked, with exit pressure equal to 100 kPa
- (D) Choked, with exit pressure of about 108 kPa

**Solution.** The bracket is 1 − (1/0.95)(1/7) = 0.8496, so P04/Pc = 1/0.8496^4 = 1.919. P04/pa = 2.0 exceeds this, so the nozzle is choked and Pc = 200/1.919 = 104.2 kPa. Option (D) uses the isentropic ratio 1.853; losses raise the critical ratio, so that is wrong.

**Answer: (B)**

### Example 5.3 · NAT · 2 marks · Exit area of a choked nozzle

Use the nozzle of Example 5.2 with T04 = 1000 K and a mass flow of 25 kg/s. Find the exit area in m². Take R = 287 J/kg·K.

**Solution.**

1. Tc = 2T04/(γ + 1) = 1000 × 6/7 = 857.1 K.
2. cj = √(γRTc) = √(1.333 × 287 × 857.1) = 572.7 m/s.
3. ρc = Pc/(RTc) = 104,217/(287 × 857.1) = 0.4236 kg/m³.
4. A = ṁ/(ρc·cj) = 25/(0.4236 × 572.7) = 0.1030 m².

The pressure thrust is (104.2 − 100) kPa × 0.1030 m² = 0.43 kN. It adds to a momentum thrust of 25 × 572.7 = 14.3 kN when static.

**Answer: 0.103 m² (range 0.101 to 0.105)**

### Example 5.4 · NAT · 1 mark · Unchoked nozzle jet velocity

Gas at T04 = 900 K expands through a convergent nozzle with P04/pa = 1.6 and ηj = 0.95. Take cp = 1148 J/kg·K and γ = 4/3. Find the jet velocity in m/s.

**Solution.** 1.6 is below the critical 1.919, so the nozzle is unchoked and pe = pa. Isentropic drop = 900 × \[1 − (1/1.6)^0.25\] = 900 × 0.11086 = 99.77 K. Actual drop = 0.95 × 99.77 = 94.79 K. cj = √(2 × 1148 × 94.79) = 466.5 m/s.

**Answer: 466.5 m/s (range 463 to 470)**

### Example 5.5 · NAT · 1 mark · Convergent–divergent nozzle

Air (γ = 1.4) expands isentropically in a convergent–divergent nozzle from P0 = 1 MPa to pe = 58.5 kPa. Find the exit-to-throat area ratio.

**Solution.** P0/pe = 17.09. From P0/p = (1 + 0.2M²)^3.5, Me = √(5 × (17.09^0.2857 − 1)) = 2.50. A/A\* = (1/M)\[(2/(γ + 1))(1 + 0.2M²)\]^3 = (1/2.5) × 1.875³ = 2.637.

**Answer: 2.64 (range 2.62 to 2.66)**

### Example 5.6 · MCQ · 1 mark · Over-expansion

A convergent–divergent nozzle designed for an exit pressure of 50 kPa runs at sea level (101 kPa) with its design chamber conditions. The flow at exit is:

- (A) Under-expanded, with expansion fans at the lip
- (B) Over-expanded, with oblique shocks at the lip
- (C) Perfectly expanded
- (D) Sonic at the exit plane

**Solution.** pe = 50 kPa is below pa = 101 kPa, so the jet is over-expanded. It adjusts to ambient through oblique shocks at the lip, or a normal shock inside the nozzle if pa is high enough. Under-expansion (pe > pa) gives expansion fans instead.

**Answer: (B)**

### Example 5.7 · MSQ · 2 marks · Lowering back pressure on a choked nozzle

A convergent nozzle is already choked. The ambient pressure is lowered further while P04 and T04 stay fixed. Which statements are correct?

- (A) Mass flow increases
- (B) Exit-plane pressure stays the same
- (C) Thrust increases because of the pressure term
- (D) Exit Mach number stays 1

**Solution.** Once the nozzle is choked, downstream changes cannot travel upstream, so ṁ, Pc and the exit Mach number of 1 are frozen. That makes (B) and (D) true and (A) false. Thrust still rises because (pe − pa)Ae grows as pa falls, so (C) is true.

**Answer: (B), (C), (D)**

## 6. Combustors and afterburners

The combustor sets the turbine entry temperature through the fuel–air ratio. The overall mixture is very lean, so the air is split into zones to keep the flame stable.

- Energy balance: (1 + f)cpg·T03 = cpa·T02 + f·ηb·QR, so f = (cpg·T03 − cpa·T02)/(ηb·QR − cpg·T03)
- Stoichiometric ratio for CxHy + (x + y/4)(O2 + 3.76N2): f\_st = (12x + y)/(137.28(x + y/4)); for CnH2n+2 this is (7n + 1)/(34.32(3n + 1))
- Equivalence ratio: φ = f/f\_st, lean when φ < 1 and rich when φ > 1
- Combustion efficiency: ηb = f\_theoretical/f\_actual for the same temperature rise
- Pressure loss factor: PLF = ΔP0/(ṁ²/(2ρ1·Am²)) = K1 + K2(T03/T02 − 1), the cold (friction) loss plus the hot (heating) loss
- Zones: primary (near stoichiometric, recirculation holds the flame), secondary (completes burning), dilution (cools gas to the turbine limit and shapes its temperature profile)

### Example 6.1 · NAT · 1 mark · Stoichiometric fuel–air ratio

Kerosene is approximated as C12H26. Find the stoichiometric fuel–air ratio, taking air as O2 + 3.76N2.

**Solution.** For CnH2n+2 with n = 12: f\_st = 85/(34.32 × 37) = 85/1269.8 = 0.0669. From first principles, oxygen needed = 12 + 26/4 = 18.5 mol per mol of fuel. Air mass = 18.5 × 137.28 = 2539.7 g against 170 g of fuel, giving 0.0669 again (air–fuel ratio about 15).

**Answer: 0.0669 (range 0.066 to 0.068)**

### Example 6.2 · NAT · 1 mark · Equivalence ratio

A combustor burning the kerosene of Example 6.1 runs at an overall fuel–air ratio of 0.02. Find the equivalence ratio.

**Solution.** φ = f/f\_st = 0.02/0.0669 = 0.299. Such a lean mixture would not burn on its own, so only the primary-zone air burns near stoichiometric while the rest cools and dilutes.

**Answer: 0.299 (range 0.29 to 0.31)**

### Example 6.3 · NAT · 2 marks · Fuel–air ratio from an energy balance

Air enters a combustor at T02 = 600 K and leaves at T03 = 1400 K. Take cpa = 1.005 kJ/kg·K, cpg = 1.148 kJ/kg·K, QR = 43,000 kJ/kg and ηb = 0.98. Find the fuel–air ratio.

**Solution.** f = (cpg·T03 − cpa·T02)/(ηb·QR − cpg·T03) = (1607.2 − 603.0)/(42,140 − 1607.2) = 1004.2/40,532.8 = 0.0248.

**Answer: 0.0248 (range 0.0244 to 0.0252)**

### Example 6.4 · NAT · 1 mark · Combustion efficiency

Complete combustion would need a fuel–air ratio of 0.0230 to reach the required turbine entry temperature, but the engine actually uses 0.0240. Find the combustion efficiency.

**Solution.** ηb = f\_theoretical/f\_actual = 0.0230/0.0240 = 0.958.

**Answer: 0.958 (range 0.955 to 0.961)**

### Example 6.5 · NAT · 2 marks · Combustor pressure loss

A combustor passes 20 kg/s of air at P02 = 1.2 MPa and T02 = 600 K through a maximum casing area Am = 0.1 m². Its loss factor is PLF = 20 + 2(T03/T02 − 1) with T03 = 1350 K. Find the stagnation pressure loss as a percentage of P02 (R = 287 J/kg·K).

**Solution.**

1. ρ1 = P02/(RT02) = 1.2 × 10⁶/(287 × 600) = 6.969 kg/m³.
2. Reference dynamic head = ṁ²/(2ρ1·Am²) = 400/(2 × 6.969 × 0.01) = 2870 Pa.
3. PLF = 20 + 2 × (2.25 − 1) = 22.5, so ΔP0 = 22.5 × 2870 = 64.6 kPa.
4. ΔP0/P02 = 64.6/1200 = 5.38%.

**Answer: 5.38% (range 5.3 to 5.5)**

### Example 6.6 · NAT · 2 marks · Afterburner thrust augmentation

A turbojet flies at 250 m/s. Without afterburning, gas leaves the turbine at 950 K and the fully expanded jet speed is 560 m/s. The afterburner raises the stagnation temperature to 1900 K at the same nozzle pressure ratio, with the nozzle area opening to suit. Neglecting fuel mass and pressure losses, find the ratio of thrust with afterburning to thrust without.

**Solution.**

1. At a fixed nozzle pressure ratio, cj is proportional to √T0, so cj,ab = 560 × √(1900/950) = 792.0 m/s.
2. Thrust ratio = (792.0 − 250)/(560 − 250) = 542.0/310 = 1.748.

On the ground (ci = 0) the same reheat gives only 792/560 = 1.41, so afterburning pays off most at high flight speed. It costs a lot of fuel: with ηab = 0.95, fab = 1.148 × 950/(0.95 × 43,000 − 1.148 × 1900) = 0.028.

**Answer: 1.75 (range 1.72 to 1.78)**

### Example 6.7 · MSQ · 1 mark · Combustor types and zones

Which statements about gas turbine combustors are correct?

- (A) An annular combustor is shorter and lighter, with lower pressure loss, than separate cans for the same airflow
- (B) Separate can combustors allow development testing on a single can at small airflow
- (C) Dilution air is mainly used to hold the flame in the primary zone
- (D) Combustor volume is sized for the highest operating altitude, where low pressure slows the reaction rate

**Solution.** (A) and (B) are the standard trade-off: annular saves length, weight and loss, while cans are easy to develop and maintain. Can-annular designs put separate flame tubes in one annular casing as a compromise. (C) is false because the recirculating primary zone holds the flame; dilution air cools the gas. (D) is true, as in your notes.

**Answer: (A), (B), (D)**

## 7. Engine performance: turbojet, turbofan, turboprop, turboshaft, ramjet

Cycle analysis is a chain: intake, compressor, combustor, turbine work balance, nozzle, thrust. Carry T0 and P0 station by station and the rest follows.

- Work balance (fuel mass neglected): cpg(T03 − T04) = cpa(T02 − T01)/ηm
- Turbofan: ṁh = ṁa/(B + 1) and ṁc = B·ṁa/(B + 1); F = ṁc(cjc − ci) + ṁh\[(1 + f)cjh − ci\], plus any pressure terms
- Turboprop: thrust power = ηpr·SP + Fjet·V; equivalent shaft power ESP = SP + Fjet·V/ηpr
- Turboshaft: the useful output is shaft power from a free power turbine
- Ideal ramjet (pe = pa, constant γ): ue/u0 = √(T04/T0a), so F/ṁ = u0(√(T04/T0a) − 1)

### Example 7.1 · NAT · 2 marks · Complete turbojet analysis

A turbojet flies at Mach 0.85 at 11 km (Ta = 216.65 K, pa = 22.63 kPa). Intake ηi = 0.93. Compressor πc = 10, ηc = 0.86. Combustor loss 5% of P02, T03 = 1250 K, ηb = 0.98, QR = 43 MJ/kg. Turbine ηt = 0.89, ηm = 0.99. Convergent nozzle ηj = 0.95. Use cpa = 1.005 kJ/kg·K, γa = 1.4, cpg = 1.148 kJ/kg·K, γg = 4/3 and R = 287 J/kg·K. Neglect fuel mass in the work balance and thrust. Find the specific thrust in N·s/kg.

**Solution.**

1. Flight speed: ci = 0.85 × √(1.4 × 287 × 216.65) = 250.8 m/s.
2. Intake: T01 = 216.65 × 1.1445 = 248.0 K and P01 = 22.63 × (1 + 0.93 × 0.1445)^3.5 = 35.18 kPa.
3. Compressor: ΔTc = 248.0 × (10^0.2857 − 1)/0.86 = 268.3 K, so T02 = 516.3 K and P02 = 351.8 kPa.
4. Combustor: P03 = 0.95 × 351.8 = 334.2 kPa and f = (1.148 × 1250 − 1.005 × 516.3)/(0.98 × 43,000 − 1.148 × 1250) = 0.0225.
5. Turbine: ΔTt = 1.005 × 268.3/(0.99 × 1.148) = 237.3 K, so T04 = 1012.7 K. T04' = 1250 − 237.3/0.89 = 983.4 K, so P03/P04 = (1250/983.4)^4 = 2.611 and P04 = 128.0 kPa.
6. Nozzle: P04/pa = 5.66 exceeds the critical 1.919, so it is choked. Tc = 1012.7 × 6/7 = 868.0 K, Pc = 128.0/1.919 = 66.7 kPa and cj = √(1.333 × 287 × 868.0) = 576.3 m/s.
7. Exit area per unit flow: A/ṁ = RTc/(Pc·cj) = (287 × 868.0)/(66,716 × 576.3) = 0.006479 m²·s/kg.
8. Fs = (cj − ci) + (Pc − pa)·A/ṁ = 325.6 + 44,086 × 0.006479 = 325.6 + 285.6 = 611.2 N·s/kg.

TSFC = f/Fs = 0.0225/611.2 = 3.68 × 10⁻⁵ kg/(N·s), or 0.133 kg/(N·h). Almost half the thrust comes from the pressure term of the choked convergent nozzle at altitude.

**Answer: 611 N·s/kg (range 600 to 622)**

### Example 7.2 · NAT · 1 mark · Turbofan static thrust

A separate-exhaust turbofan with bypass ratio 5 swallows 300 kg/s on the test bed. The cold jet leaves at 300 m/s and the hot jet at 450 m/s, both fully expanded. Neglecting fuel mass, find the thrust in kN.

**Solution.** ṁh = 300/6 = 50 kg/s and ṁc = 250 kg/s. F = 250 × 300 + 50 × 450 = 75,000 + 22,500 = 97,500 N. The fan stream gives 77% of the thrust, typical of a high-bypass engine.

**Answer: 97.5 kN (range 97 to 98)**

### Example 7.3 · NAT · 2 marks · Turbofan at cruise

A turbofan with B = 5 and a total airflow of 240 kg/s flies at 250 m/s. The cold jet leaves at 360 m/s and the hot jet at 480 m/s, both fully expanded. The fuel–air ratio is 0.018 based on core air. Find the TSFC in kg/(N·h).

**Solution.**

1. ṁh = 240/6 = 40 kg/s, ṁc = 200 kg/s and ṁf = 0.018 × 40 = 0.72 kg/s.
2. Cold thrust = 200 × (360 − 250) = 22,000 N.
3. Hot thrust = 40 × (1.018 × 480 − 250) = 40 × 238.6 = 9,546 N.
4. F = 31,546 N, so TSFC = 0.72 × 3600/31,546 = 0.0822 kg/(N·h).

**Answer: 0.0822 kg/(N·h) (range 0.081 to 0.083)**

### Example 7.4 · NAT · 1 mark · Turboprop equivalent shaft power

A turboprop delivers 3000 kW to its propeller (ηpr = 0.85) and also produces 2000 N of residual jet thrust at a flight speed of 150 m/s. Find the equivalent shaft power in kW.

**Solution.** Jet thrust power = 2000 × 150 = 300 kW. ESP = SP + Fjet·V/ηpr = 3000 + 300/0.85 = 3352.9 kW. The total thrust power is 0.85 × 3000 + 300 = 2850 kW. At a fuel flow of 0.25 kg/s, ESFC = 0.25 × 3600/3352.9 = 0.268 kg/(kW·h).

**Answer: 3353 kW (range 3340 to 3365)**

### Example 7.5 · NAT · 2 marks · Turboshaft free power turbine

A gas generator supplies 10 kg/s of gas at T04 = 1050 K and P04 = 300 kPa to a free power turbine exhausting at 105 kPa. The power turbine isentropic efficiency is 0.88 (cpg = 1.148 kJ/kg·K, γ = 4/3). Find the shaft power in MW.

**Solution.** Isentropic drop = 1050 × \[1 − (105/300)^0.25\] = 1050 × 0.2308 = 242.4 K. Actual drop = 0.88 × 242.4 = 213.3 K. Power = 10 × 1.148 × 213.3 = 2449 kW.

**Answer: 2.45 MW (range 2.42 to 2.48)**

### Example 7.6 · NAT · 2 marks · Ideal ramjet

An ideal ramjet flies at Mach 3 where Ta = 220 K, and its burner exit stagnation temperature is 2000 K. Take γ = 1.4 throughout, R = 287 J/kg·K, full expansion and negligible fuel mass. Find the specific thrust in N·s/kg.

**Solution.**

1. u0 = 3 × √(1.4 × 287 × 220) = 891.9 m/s and T0a = 220 × (1 + 0.2 × 9) = 616 K.
2. With no P0 loss and pe = pa, the exit Mach number equals the flight Mach number, so ue/u0 = √(T04/T0a) = √(2000/616) = 1.802.
3. F/ṁ = u0(1.802 − 1) = 715 N·s/kg, and ηp = 2/(1 + 1.802) = 0.714.

**Answer: 715 N·s/kg (range 708 to 722)**

### Example 7.7 · MSQ · 2 marks · Performance trends

Which statements are correct?

- (A) At the same thrust, a turbofan has a higher propulsive efficiency than a turbojet
- (B) At a fixed turbine entry temperature, a turbojet's specific thrust keeps rising as compressor pressure ratio increases
- (C) At a fixed turbine entry temperature, raising the pressure ratio from 5 to 15 lowers a turbojet's SFC
- (D) At a fixed flight Mach number, thrust falls with altitude

**Solution.** (A) is true because more air at a lower jet speed raises ηp. (B) is false: specific thrust peaks at an optimum pressure ratio, as in the carpet plot in your notes. (C) is true because higher pressure ratio raises thermal efficiency over this range. (D) is true because air density, and so mass flow, falls with altitude.

**Answer: (A), (C), (D)**

## 8. Axial compressors

Each stage is a rotor followed by a stator. The rotor adds energy through the Euler equation; the stator only diffuses. With angles from the axial direction and constant Ca:

- Velocity triangles: U/Ca = tanα1 + tanβ1 = tanα2 + tanβ2
- Stage work: W = λ·U·Ca(tanβ1 − tanβ2) = λ·U·Ca(tanα2 − tanα1), and ΔT0s = W/cp
- Stage pressure ratio: Rs = (1 + ηs·ΔT0s/T01)^(γ/(γ − 1))
- Degree of reaction: R = (φ/2)(tanβ1 + tanβ2) = 1 − (φ/2)(tanα1 + tanα2)
- 50% reaction gives symmetric triangles: α1 = β2 and α2 = β1
- Multistaging: number of stages = overall ΔT0/ΔT0s; λ falls below 1 in rear stages as the axial velocity profile peaks
- de Haller criterion: keep W2/W1 above about 0.72 to avoid excessive diffusion

### Example 8.1 · NAT · 1 mark · Stage temperature rise

An axial compressor stage has U = 280 m/s and Ca = 160 m/s. Inlet guide vanes give α1 = 15°, and the rotor relative outlet angle is β2 = 40°, both from the axial direction. With work-done factor λ = 0.93, find the stage stagnation temperature rise (cp = 1005 J/kg·K).

**Solution.** tanβ1 = U/Ca − tanα1 = 1.75 − 0.2679 = 1.4821, so β1 = 56.0°. W = λ·U·Ca(tanβ1 − tanβ2) = 0.93 × 280 × 160 × (1.4821 − 0.8391) = 26,788 J/kg. ΔT0s = 26,788/1005 = 26.7 K.

**Answer: 26.7 K (range 26.4 to 26.9)**

### Example 8.2 · NAT · 1 mark · Stage pressure ratio

For the stage of Example 8.1, T01 = 288 K and the stage isentropic efficiency is 0.88. Find the stage pressure ratio (γ = 1.4).

**Solution.** Rs = (1 + 0.88 × 26.65/288)^3.5 = 1.0814^3.5 = 1.315.

**Answer: 1.315 (range 1.31 to 1.32)**

### Example 8.3 · NAT · 1 mark · Degree of reaction

Find the degree of reaction of the stage in Example 8.1.

**Solution.** R = (φ/2)(tanβ1 + tanβ2) = (160/560) × (1.4821 + 0.8391) = 0.2857 × 2.3212 = 0.663. As a check, tanα2 = 1.75 − 0.8391 = 0.9109 (α2 = 42.3°), and R = 1 − 0.2857 × (0.2679 + 0.9109) = 0.663. The rotor does about two-thirds of the static enthalpy rise.

**Answer: 0.663 (range 0.655 to 0.670)**

### Example 8.4 · NAT · 2 marks · Number of stages

An axial compressor must deliver an overall pressure ratio of 6 from T01 = 288 K, with an overall isentropic efficiency of 0.86. Each stage gives ΔT0s = 22 K. Find the minimum number of stages (γ = 1.4).

**Solution.** Overall ΔT0 = 288 × (6^0.2857 − 1)/0.86 = 288 × 0.6685/0.86 = 223.9 K. Stages = 223.9/22 = 10.18, so 11 stages are needed; 10 would fall short of the pressure ratio.

**Answer: 11**

### Example 8.5 · NAT · 2 marks · Designing a 50% reaction stage

A 50% reaction stage has U = 300 m/s, flow coefficient φ = 0.5 and blade loading ψ = Δh0/U² = 0.35 (λ = 1). Find the rotor inlet relative angle β1 in degrees.

**Solution.**

1. ψ = φ(tanβ1 − tanβ2) gives tanβ1 − tanβ2 = 0.7.
2. R = (φ/2)(tanβ1 + tanβ2) = 0.5 gives tanβ1 + tanβ2 = 2.
3. So tanβ1 = 1.35 (β1 = 53.5°) and tanβ2 = 0.65 (β2 = 33.0°). By symmetry α2 = 53.5° and α1 = 33.0°.

The de Haller number W2/W1 = cosβ1/cosβ2 = 0.595/0.839 = 0.71, just under 0.72, so this loading sits at the diffusion limit. The stage ΔT0 = 0.35 × 300²/1005 = 31.3 K.

**Answer: 53.5° (range 53 to 54)**

### Example 8.6 · MSQ · 1 mark · What happens in the rotor

In an axial compressor rotor, which statements are correct?

- (A) The relative velocity decreases
- (B) The absolute velocity increases
- (C) The stagnation pressure increases
- (D) The stagnation enthalpy stays constant

**Solution.** The rotor passages diffuse the relative flow (A) while turning the absolute flow, which raises its swirl and speed (B). Work input raises h0 and P0, so (C) holds and (D) fails. What stays constant in the rotor is rothalpy, h + W²/2 − U²/2; the stator then lowers C and raises static pressure at constant h0.

**Answer: (A), (B), (C)**

## 9. Centrifugal compressors

Air enters axially through the inducer, is flung outward by the impeller and is slowed in the diffuser. With no inlet swirl the Euler work is U2·Ct2, and slip keeps Ct2 below U2.

- Tip speed: U2 = πD2N/60
- Slip factor: σ = Ct2/U2; for radial vanes, Stanitz gives σ = 1 − 0.63π/n
- Work input: W = ψ·σ·U2², where ψ ≥ 1 is the power input factor (disc friction and windage)
- Temperature rise: T02 − T01 = ψσU2²/cp
- Pressure ratio: P03/P01 = \[1 + ηc·ψσU2²/(cp·T01)\]^(γ/(γ − 1))
- Vane shape (outlet angle β2 from the tangent, as in your notes): forward β2 > 90°, radial = 90°, backward < 90°; W = U2² − U2·Cr2·cotβ2 = k1 − k2·Q
- Inducer: the relative Mach number peaks at the inducer tip; keeping it below about 0.9 limits shock losses

### Example 9.1 · NAT · 1 mark · Impeller tip speed

An impeller with a 0.5 m tip diameter runs at 18,000 rpm. Find the tip speed in m/s.

**Solution.** U2 = π × 0.5 × 18,000/60 = 471.2 m/s.

**Answer: 471.2 m/s (range 470 to 472.5)**

### Example 9.2 · NAT · 1 mark · Slip factor

Estimate the slip factor of a radial-vaned impeller with 19 vanes using Stanitz's formula.

**Solution.** σ = 1 − 0.63π/n = 1 − (0.63 × 3.1416)/19 = 1 − 0.1042 = 0.896. This matches the rule of thumb in your notes that 19 to 21 vanes give σ ≈ 0.9.

**Answer: 0.896 (range 0.89 to 0.90)**

### Example 9.3 · NAT · 2 marks · Pressure ratio

A centrifugal compressor has U2 = 450 m/s, σ = 0.9, power input factor ψ = 1.04 and overall isentropic efficiency 0.80. Inlet T01 = 295 K. Find the total pressure ratio (cp = 1.005 kJ/kg·K, γ = 1.4).

**Solution.**

1. T02 − T01 = ψσU2²/cp = 1.04 × 0.9 × 450²/1005 = 188.6 K.
2. P03/P01 = (1 + 0.80 × 188.6/295)^3.5 = 1.5115^3.5 = 4.24.

At 9 kg/s the power needed is 9 × 1.005 × 188.6 = 1706 kW. As your notes say, designers want σ as high and ψ as low as possible.

**Answer: 4.24 (range 4.20 to 4.29)**

### Example 9.4 · NAT · 2 marks · Inducer tip relative Mach number

An inducer has a tip diameter of 0.30 m and runs at 16,000 rpm. Air enters axially at 150 m/s with T01 = 295 K. Find the relative Mach number at the inducer tip (γ = 1.4, R = 287 J/kg·K, cp = 1005 J/kg·K).

**Solution.**

1. Static temperature: T1 = 295 − 150²/(2 × 1005) = 283.8 K, so a1 = √(1.4 × 287 × 283.8) = 337.7 m/s.
2. Tip speed: Ut = π × 0.30 × 16,000/60 = 251.3 m/s.
3. W1 = √(150² + 251.3²) = 292.7 m/s, so M\_rel = 292.7/337.7 = 0.867.

The inducer blade angle at the tip is tan⁻¹(251.3/150) = 59.2° from the axial direction. Prewhirl from inlet guide vanes would lower W1 and M\_rel, at the cost of some work.

**Answer: 0.867 (range 0.86 to 0.875)**

### Example 9.5 · MCQ · 1 mark · Vane shape and stability

Neglecting losses, how does the work input of a backward-curved impeller change as the flow rate rises at constant speed?

- (A) It rises linearly
- (B) It stays constant
- (C) It falls linearly
- (D) It first rises, then falls

**Solution.** W = U2² − U2·Cr2·cotβ2 = k1 − k2·Q. For backward vanes (β2 < 90°) cotβ2 is positive, so work falls as Q rises. Radial vanes give constant work and forward vanes give rising work. The falling characteristic of backward vanes is the most stable.

**Answer: (C)**

### Example 9.6 · MSQ · 1 mark · Vaneless diffuser

In the vaneless space after a centrifugal impeller (constant width, incompressible flow assumed), which statements are correct?

- (A) r·Ct stays constant (free vortex)
- (B) The tangential velocity increases with radius
- (C) The radial velocity decreases with radius
- (D) The flow path is a logarithmic spiral

**Solution.** With no blades there is no torque, so angular momentum r·Ct is conserved (A) and Ct falls as r grows, which rules out (B). Continuity through the area 2πrb gives Cr ∝ 1/r (C). Both components fall as 1/r, so the flow angle is constant and the path is a logarithmic spiral (D).

**Answer: (A), (C), (D)**

## 10. Axial turbines and blade cooling

A turbine stage is a nozzle row followed by a rotor. Angles are from the axial direction, Ca is constant, and swirl is counted positive in the direction that does work.

- Velocity triangles: U/Ca = tanα2 − tanβ2 = tanβ3 − tanα3
- Stage work: W = U·Ca(tanα2 + tanα3) = U·Ca(tanβ2 + tanβ3), and ΔT0s = W/cpg
- Blade loading: ψ = W/U² = φ(tanβ2 + tanβ3), with flow coefficient φ = Ca/U
- Degree of reaction: R = (φ/2)(tanβ3 − tanβ2) = 1/2 + (φ/2)(tanα3 − tanβ2)
- Impulse stage (R = 0): β2 = β3. 50% reaction: α2 = β3 and β2 = α3
- Total-to-total efficiency: ηtt = (T01 − T03)/(T01 − T03'), with T01/T03' = (P01/P03)^((γ − 1)/γ)
- Cooling effectiveness: ε = (Tg − Tb)/(Tg − Tc) for gas, blade and coolant temperatures

### Example 10.1 · NAT · 1 mark · Stage temperature drop

A turbine stage has U = 350 m/s and Ca = 280 m/s. The nozzle exit angle is α2 = 60° and the flow leaves the rotor axially (α3 = 0). Find the stage stagnation temperature drop (cpg = 1148 J/kg·K).

**Solution.** Ct2 = Ca·tanα2 = 280 × 1.7321 = 485.0 m/s and Ct3 = 0. W = U(Ct2 + Ct3) = 350 × 485.0 = 169,741 J/kg. ΔT0s = 169,741/1148 = 147.9 K.

**Answer: 147.9 K (range 146.5 to 149)**

### Example 10.2 · NAT · 2 marks · Blade angles, loading and reaction

For the stage of Example 10.1, find the degree of reaction.

**Solution.**

1. tanβ2 = tanα2 − U/Ca = 1.7321 − 1.25 = 0.4821, so β2 = 25.7°.
2. tanβ3 = tanα3 + U/Ca = 1.25, so β3 = 51.3°.
3. ψ = W/U² = 169,741/350² = 1.386, which matches φ(tanβ2 + tanβ3) = 0.8 × 1.7321.
4. R = (φ/2)(tanβ3 − tanβ2) = 0.4 × (1.25 − 0.4821) = 0.307.

**Answer: 0.307 (range 0.30 to 0.315)**

### Example 10.3 · NAT · 1 mark · 50% reaction with axial exit

A 50% reaction turbine stage has axial exit flow (α3 = 0) and a mean blade speed of 320 m/s. Find the stage stagnation temperature drop (cpg = 1148 J/kg·K).

**Solution.** For R = 0.5 the triangles are symmetric, so β2 = α3 = 0 and tanβ3 = 1/φ. Then ψ = φ(0 + 1/φ) = 1, so W = U². ΔT0s = 320²/1148 = 89.2 K.

**Answer: 89.2 K (range 88.5 to 90)**

### Example 10.4 · NAT · 2 marks · Impulse stage blade speed

An impulse stage (R = 0, symmetric blades) receives gas from its nozzles at C2 = 600 m/s with α2 = 70° from the axial direction. The flow must leave axially. Find the required mean blade speed in m/s.

**Solution.** Impulse blading has β2 = β3, so Wt2 = Wt3. Axial exit gives Wt3 = U, while Wt2 = Ct2 − U. Equating them gives Ct2 = 2U, so U = C2·sinα2/2 = 600 × 0.9397/2 = 281.9 m/s. The work is W = U·Ct2 = 2U² = 158.9 kJ/kg, so ψ = 2 for impulse against 1 for 50% reaction.

**Answer: 281.9 m/s (range 279 to 285)**

### Example 10.5 · NAT · 1 mark · Stage efficiency

A turbine stage has T01 = 1200 K and a stagnation pressure ratio P01/P03 = 1.7. The actual stagnation temperature drop is 135 K. Find the total-to-total efficiency (γ = 4/3).

**Solution.** Ideal drop = 1200 × \[1 − (1/1.7)^0.25\] = 1200 × 0.12423 = 149.1 K. ηtt = 135/149.1 = 0.906.

**Answer: 0.906 (range 0.90 to 0.91)**

### Example 10.6 · NAT · 1 mark · Blade cooling effectiveness (special topic)

Gas at 1700 K flows over a turbine blade cooled internally by compressor bleed air at 850 K. The cooling effectiveness is 0.6. Find the blade metal temperature in K.

**Solution.** ε = (Tg − Tb)/(Tg − Tc), so Tb = Tg − ε(Tg − Tc) = 1700 − 0.6 × 850 = 1190 K. Cooling lets the gas run about 500 K hotter than the metal.

**Answer: 1190 K (range 1185 to 1195)**

### Example 10.7 · MSQ · 1 mark · Blade cooling methods (special topic)

Which statements about turbine blade cooling are correct?

- (A) Film cooling ejects air through surface holes to form a protective cool layer
- (B) Transpiration cooling passes coolant through a porous blade wall
- (C) Cooling air is bled from the compressor, so it costs some cycle efficiency
- (D) Plain internal convection suffices at the leading edge, so impingement is never needed there

**Solution.** (A), (B) and (C) are correct. (D) is false: the leading edge is a stagnation region with the highest heat load, so it is usually cooled by internal impingement jets, often with film holes as well. Nickel-based superalloys, as in your notes, and thermal barrier coatings complete the picture.

**Answer: (A), (B), (C)**

## 11. Compressor–turbine matching, surge, stall and choking (special topic)

Off design, the compressor and turbine must agree on speed (on a common shaft), mass flow and work. Non-dimensional groups let one map cover every inlet condition.

- Map groups: P02/P01 = f(ṁ√T01/P01, N/√T01); the same groups mean the same operating point
- Work balance: cpa(T02 − T01) = ηm(1 + f)cpg(T03 − T04)
- Flow compatibility: ṁ√T01/P01 = (ṁ√T03/P03)·(P03/P02)·(P02/P01)·√(T01/T03); with choked turbine nozzles the first factor is constant
- Surge at low flow (left of the map), choking at high flow (right); blow-off valves, variable stators and multiple spools keep the working line clear of surge

### Example 11.1 · NAT · 1 mark · Corrected mass flow

On a sea-level test (T01 = 288 K, P01 = 101.3 kPa) a compressor passes 50 kg/s at 10,000 rpm. At altitude the inlet conditions are T01 = 250 K and P01 = 50 kPa. If it runs at the same non-dimensional point, find the mass flow in kg/s.

**Solution.** ṁ√T01/P01 stays fixed, so ṁ = 50 × (50/101.3) × √(288/250) = 50 × 0.4936 × 1.0733 = 26.5 kg/s. N/√T01 also stays fixed, so the speed becomes 10,000 × √(250/288) = 9317 rpm.

**Answer: 26.5 kg/s (range 26.3 to 26.7)**

### Example 11.2 · NAT · 2 marks · Work balance and turbine pressure ratio

A single-spool engine has T01 = 288 K, T02 = 560 K, T03 = 1250 K, f = 0.02 and ηm = 0.99. The turbine isentropic efficiency is 0.88. Take cpa = 1.005 kJ/kg·K, cpg = 1.148 kJ/kg·K and γg = 4/3. Find the turbine pressure ratio P03/P04.

**Solution.**

1. Work balance: T03 − T04 = (1.005 × 272)/(0.99 × 1.02 × 1.148) = 273.4/1.1593 = 235.8 K, so T04 = 1014.2 K.
2. Isentropic outlet temperature: T04' = 1250 − 235.8/0.88 = 982.0 K.
3. P03/P04 = (1250/982.0)^4 = 2.625.

**Answer: 2.625 (range 2.60 to 2.65)**

### Example 11.3 · NAT · 2 marks · Working line with a choked turbine

An engine's turbine nozzles are choked, so ṁ√T03/P03 is fixed, and the combustor loses a fixed fraction of pressure. At one operating point πc = 8 and T03/T01 = 4.0. Fuel flow is then raised so that T03/T01 = 4.84 at the same compressor non-dimensional flow. Find the new compressor pressure ratio.

**Solution.** Flow compatibility gives ṁ√T01/P01 = constant × πc × √(T01/T03). Holding the compressor flow fixed means πc ∝ √(T03/T01). So πc = 8 × √(4.84/4.0) = 8 × 1.1 = 8.8. A hotter turbine pushes the operating point up the speed line toward surge, which is why slamming the throttle is a surge risk.

**Answer: 8.8 (range 8.7 to 8.9)**

### Example 11.4 · MCQ · 1 mark · Reading the compressor map

On a compressor map, moving along a constant N/√T01 line toward lower ṁ√T01/P01 eventually leads to:

- (A) Choking
- (B) Surge
- (C) Windmilling
- (D) Flameout

**Solution.** Lower flow at constant speed raises blade incidence until the blades stall and the system surges. Choking (A) lies at the other end, at maximum flow. Your notes put it the same way: maximum flow is the choking limit, minimum flow is the surge or stall limit.

**Answer: (B)**

### Example 11.5 · MSQ · 2 marks · Avoiding surge at off-design

A multistage axial compressor tends to surge at low speed. Which measures help?

- (A) Blow-off (bleed) valves at intermediate stages
- (B) Variable inlet guide vanes and stators
- (C) Splitting the compressor between two shafts (two spools)
- (D) Reducing the propelling nozzle area at low speed

**Solution.** At low speed the front stages are pushed toward stall and the rear stages toward choke. Bleeding air mid-way (A), re-staggering vanes (B) and letting each spool find its own speed (C) all ease this mismatch. A smaller nozzle (D) raises the working line toward surge; opening it helps instead.

**Answer: (A), (B), (C)**

## 12. Rocket propulsion

A rocket carries its own oxidiser, so it has no ram drag and its thrust does not depend on flight speed. Most questions reduce to the thrust equation, c\* and CF, or the rocket equation.

- Thrust: F = ṁ·ve + (pe − pa)Ae = ṁ·c, where c is the effective exhaust velocity
- Specific impulse: Isp = F/(ṁ·g0) = c/g0, in seconds
- c\* = Pc·At/ṁ (combustion quality) and CF = F/(Pc·At) (nozzle quality), so c = c\*·CF and F = CF·Pc·At
- Ideal exhaust velocity: ve = √{(2γ/(γ − 1))·R·T0·\[1 − (pe/Pc)^((γ − 1)/γ)\]}
- Rocket equation: ΔV = c·ln(m0/mf) = g0·Isp·ln(m0/mf)
- Identical stages: λ = mPL/(mp + ms), ε = ms/(mp + ms), stage mass ratio n = (1 + λ)/(ε + λ), and ΔV = N·g0·Isp·ln n for N stages
- Solid motor: r = a·Pc^n; equilibrium Pc^(1 − n) = ρp·a·c\*·(Ab/At), stable only if n < 1
- Propulsive efficiency: ηp = 2(u/c)/(1 + (u/c)²), equal to 1 when u = c

### Example 12.1 · NAT · 1 mark · Thrust and specific impulse

A rocket engine at sea level (pa = 101.3 kPa) has ṁ = 100 kg/s, exhaust velocity 2800 m/s, exit pressure 70 kPa and exit area 0.8 m². Find the specific impulse in seconds.

**Solution.** F = 100 × 2800 + (70 − 101.3) × 10³ × 0.8 = 280,000 − 25,060 = 254,940 N. Isp = 254,940/(100 × 9.81) = 259.9 s. In vacuum the pressure term becomes +56,000 N, giving Isp = 342.5 s, so over-expansion at sea level costs thrust.

**Answer: 259.9 s (range 258 to 262)**

### Example 12.2 · NAT · 2 marks · Ideal exhaust velocity

Combustion products (γ = 1.2, molar mass 22 kg/kmol) at T0 = 3200 K and Pc = 7 MPa expand isentropically to pe = 0.1 MPa. Find the exhaust velocity in m/s, taking the universal gas constant as 8314 J/kmol·K.

**Solution.**

1. R = 8314/22 = 377.9 J/kg·K and 2γ/(γ − 1) = 12.
2. (pe/Pc)^((γ − 1)/γ) = (1/70)^(1/6) = 0.4926, so the bracket is 0.5074.
3. ve = √(12 × 377.9 × 3200 × 0.5074) = √(7.363 × 10⁶) = 2714 m/s.

With pe = pa, Isp = 2714/9.81 = 276.6 s. A hotter chamber or lighter exhaust raises ve roughly as √(T0/M).

**Answer: 2714 m/s (range 2690 to 2740)**

### Example 12.3 · NAT · 2 marks · c\*, CF and Isp

A rocket chamber at Pc = 5 MPa has a throat area of 0.02 m², a propellant flow of 65 kg/s and a thrust of 180 kN. Find the specific impulse in seconds.

**Solution.** c\* = Pc·At/ṁ = (5 × 10⁶ × 0.02)/65 = 1538.5 m/s. CF = F/(Pc·At) = 180,000/100,000 = 1.80. c = c\*·CF = 2769 m/s, so Isp = 2769/9.81 = 282.3 s.

**Answer: 282.3 s (range 280 to 285)**

### Example 12.4 · NAT · 1 mark · Rocket equation

A single-stage rocket has Isp = 300 s and a mass ratio m0/mf = 4. Neglecting gravity and drag, find the velocity gain in m/s.

**Solution.** ΔV = g0·Isp·ln(m0/mf) = 9.81 × 300 × ln 4 = 2943 × 1.3863 = 4080 m/s.

**Answer: 4080 m/s (range 4060 to 4100)**

### Example 12.5 · NAT · 1 mark · Rocket propulsive efficiency

A rocket with an effective exhaust velocity of 2500 m/s is flying at 1500 m/s. Find its propulsive efficiency.

**Solution.** u/c = 0.6, so ηp = (2 × 0.6)/(1 + 0.36) = 0.882. Unlike a jet engine, a rocket reaches ηp = 1 at u = c while still producing full thrust.

**Answer: 0.882 (range 0.875 to 0.89)**

### Example 12.6 · NAT · 2 marks · Two-stage rocket

A two-stage rocket has identical stages, each with payload ratio λ = 0.1, structural ratio ε = 0.1 and Isp = 300 s. Neglecting gravity and drag, find the total velocity gain in m/s.

**Solution.** Stage mass ratio n = (1 + λ)/(ε + λ) = 1.1/0.2 = 5.5. ΔV = 2 × 9.81 × 300 × ln 5.5 = 5886 × 1.7047 = 10,034 m/s. For the same overall payload fraction (0.83%), a single stage with ε = 0.1 reaches only 6,565 m/s, which is the case for staging.

**Answer: 10,034 m/s (range 9,950 to 10,120)**

### Example 12.7 · NAT · 2 marks · Solid motor chamber pressure

A solid propellant burns as r = 3.5·Pc^0.4 mm/s with Pc in MPa. Its density is 1750 kg/m³, c\* = 1500 m/s and the burning-surface-to-throat area ratio Ab/At = 250. Find the equilibrium chamber pressure in MPa.

**Solution.**

1. Gas generated = ρp·Ab·r and nozzle outflow = Pc·At/c\*. Equating them gives Pc^(1 − n) = ρp·a·c\*·(Ab/At).
2. With a = 3.5 × 10⁻³ m/s per MPa^0.4 and Pc in MPa (10⁶ converts MPa to Pa): Pc^0.6 = (1750 × 3.5 × 10⁻³ × 1500 × 250)/10⁶ = 2.297.
3. Pc = 2.297^(1/0.6) = 4.00 MPa, and the burn rate is 3.5 × 4^0.4 = 6.09 mm/s.

Because n < 1, a pressure rise increases nozzle outflow faster than gas generation, so the motor is stable.

**Answer: 4.0 MPa (range 3.95 to 4.05)**

### Example 12.8 · NAT · 1 mark · Liquid bipropellant flows

A liquid rocket runs at an oxidiser-to-fuel mixture ratio O/F = 2.5 with a total propellant flow of 70 kg/s. Find the oxidiser mass flow in kg/s.

**Solution.** ṁox = ṁ·(O/F)/(1 + O/F) = 70 × 2.5/3.5 = 50 kg/s, leaving 20 kg/s of fuel.

**Answer: 50 kg/s**

### Example 12.9 · MSQ · 1 mark · Chemical rocket classification

Which of these propellant combinations are hypergolic (ignite on contact)?

- (A) N2O4 with UDMH
- (B) Liquid oxygen with liquid hydrogen
- (C) N2O4 with MMH
- (D) Liquid oxygen with kerosene (RP-1)

**Solution.** Nitrogen tetroxide ignites on contact with hydrazine-family fuels such as UDMH and MMH, which suits restartable upper stages. LOX/LH2 is cryogenic, gives the highest Isp but needs an igniter. LOX/RP-1 is also non-hypergolic. Solid composites (AP + HTPB + Al) and hybrids (solid fuel with a liquid oxidiser) complete the classification.

**Answer: (A), (C)**

## Formula sheet for last-minute revision

Every formula used in this booklet, plus the numbers worth memorising.

| Topic | Formula or fact |
| --- | --- |
| Stagnation | T0/T = 1 + ((γ − 1)/2)M²; P0/P = (T0/T)^(γ/(γ − 1)) |
| Gas properties | cp = γR/(γ − 1); γ = 1 + 2/f; cp is 1.005 kJ/kg·K for air, 1.148 for hot gas |
| Entropy | Δs = cp ln(T2/T1) − R ln(p2/p1) |
| Brayton (ideal) | η = 1 − 1/c with c = r^((γ − 1)/γ); maximum work at c = √t |
| Heat exchanger | η = 1 − c/t, useful only while c < √t |
| Polytropic | (n − 1)/n = (γ − 1)/(γ·η∞c) in compression; η∞t(γ − 1)/γ in expansion |
| Thrust | F = (ṁa + ṁf)cj − ṁa·ci + (pe − pa)Ae |
| Efficiencies | ηp = 2/(1 + cj/ci); η0 = ηp·ηth = F·ci/(ṁf·QR) |
| Maximum thrust power | ci = cj/2, where ηp = 66.7% |
| Range | R = (V/(g·TSFC))(L/D)ln(Wi/Wf), TSFC in kg/(N·s) |
| Intake | P01/pa = \[1 + ηi((γ − 1)/2)M²\]^(γ/(γ − 1)); ηram = (P01 − pa)/(P0a − pa) |
| Normal shock at M = 2 | P02/P01 = 0.721 and M2 = 0.577 |
| Nozzle critical ratio | 1.893 for air, 1.853 for γ = 4/3; with losses 1/\[1 − (1/ηj)(γ − 1)/(γ + 1)\]^(γ/(γ − 1)) |
| Choked nozzle | Tc = 2T04/(γ + 1); cj = √(γRTc); pressure thrust (Pc − pa)A |
| Fuel–air ratio | f = (cpg·T03 − cpa·T02)/(ηb·QR − cpg·T03) |
| Stoichiometric CnH2n+2 | f\_st = (7n + 1)/(34.32(3n + 1)); about 0.067 for kerosene |
| Combustor loss | PLF = K1 + K2(T03/T02 − 1) |
| Turbofan | ṁh = ṁ/(B + 1); ṁc = B·ṁ/(B + 1) |
| Turboprop | ESP = SP + Fjet·V/ηpr |
| Ideal ramjet | F/ṁ = u0(√(T04/T0a) − 1) |
| Euler work | W = U2·Ct2 − U1·Ct1 |
| Axial compressor | W = λU·Ca(tanβ1 − tanβ2); R = (φ/2)(tanβ1 + tanβ2) |
| Stage pressure ratio | Rs = (1 + ηs·ΔT0s/T01)^(γ/(γ − 1)) |
| de Haller | W2/W1 above about 0.72 |
| Centrifugal | ΔT0 = ψσU2²/cp; σ = 1 − 0.63π/n |
| Axial turbine | W = U·Ca(tanβ2 + tanβ3); R = (φ/2)(tanβ3 − tanβ2) |
| Turbine special cases | 50% reaction with axial exit: ψ = 1. Impulse with axial exit: ψ = 2 and U = C2·sinα2/2 |
| Blade cooling | ε = (Tg − Tb)/(Tg − Tc) |
| Matching | ṁ√T01/P01 and N/√T01 fixed at a map point; with a choked turbine, πc ∝ √(T03/T01) at fixed compressor flow |
| Rocket thrust | F = ṁve + (pe − pa)Ae; Isp = F/(ṁg0) |
| c\* and CF | c\* = Pc·At/ṁ; CF = F/(Pc·At); c = c\*·CF |
| Rocket equation | ΔV = g0·Isp·ln(m0/mf) |
| Staging | n = (1 + λ)/(ε + λ); ΔV = N·g0·Isp·ln n |
| Solid motor | Pc^(1 − n) = ρp·a·c\*·(Ab/At), stable only if n < 1 |
