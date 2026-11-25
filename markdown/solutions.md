# GATE AE Propulsion Test Series: Solutions

Last updated 25 Nov 2026

## How to score yourself

Check each answer against the key at the top of its test, then read the worked solution for every question you got wrong or guessed.

The questions are in [GATE AE Propulsion Test Series: Question Papers](question-papers.md), and the same tests run online with a timer and automatic scoring at [Propulsion Mock Tests](https://abhishek4650.github.io/gate-ae-propulsion-test-series/).

- MCQ: +1 or +2 if correct; −1/3 or −2/3 if wrong; 0 if left blank.
- MSQ: full marks only for exactly the correct set of options; no negative marks.
- NAT: full marks if your value lies inside the range given; no negative marks.
- If you score below 40% on a topic test, work through that topic in the Solved Examples doc before moving on.

## Test N1 solutions · Thermodynamics, Brayton cycle, thrust and efficiencies

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 450 K (range 448 to 452) |
| 2 | MCQ | 1 | (B) |
| 3 | NAT | 1 | 54.71% (range 54.3 to 55.1) |
| 4 | NAT | 1 | 0.5 (range 0.495 to 0.505) |
| 5 | MSQ | 1 | (A), (C) |
| 6 | NAT | 2 | 17.96 (range 17.8 to 18.2) |
| 7 | NAT | 2 | 280.3 kJ/kg (range 277 to 284) |
| 8 | NAT | 2 | 0.1536 kg/(N·h) (range 0.152 to 0.156) |
| 9 | NAT | 2 | 0.9149 (range 0.909 to 0.921) |
| 10 | NAT | 2 | 0.2896 (range 0.286 to 0.293) |

### Q1 · NAT · 1 mark

**Answer: 450 K (range 448 to 452)**

T0 = T(1 + 0.2M²) = 250 × (1 + 0.2 × 4) = 250 × 1.8 = 450 K.

### Q2 · MCQ · 1 mark

**Answer: (B)**

cv = cp − R = 0.80 kJ/kg·K, so γ = cp/cv = 1.10/0.80 = 1.375. Option (D) is the hot-gas value and (C) is air; neither applies here.

### Q3 · NAT · 1 mark

**Answer: 54.71% (range 54.3 to 55.1)**

c = 16^0.2857 = 2.2082. η = 1 − 1/c = 1 − 0.4529 = 0.5471, or 54.7%.

### Q4 · NAT · 1 mark

**Answer: 0.5 (range 0.495 to 0.505)**

ηp = 2ci/(ci + cj) = 500/1000 = 0.50. Equivalently ηp = 2/(1 + cj/ci) = 2/(1 + 3) = 0.5.

### Q5 · MSQ · 1 mark

**Answer: (A), (C)**

Thrust = ṁ(cj − ci) can be had from more air at a lower jet speed, which wastes less kinetic energy in the jet. That is (A), and a higher bypass ratio (C) does exactly this. (B) is the opposite. Afterburning (D) raises jet speed, so ηp falls.

### Q6 · NAT · 2 marks

**Answer: 17.96 (range 17.8 to 18.2)**

1. t = T3/T1 = 1500/288 = 5.2083.
2. Maximum work needs c = √t = 2.2822, which makes T2 = T4.
3. r = c^(γ/(γ − 1)) = 2.2822^3.5 = (T3/T1)^1.75 = 17.96.

The cycle efficiency at this pressure ratio is 1 − 1/√t = 0.562.

### Q7 · NAT · 2 marks

**Answer: 280.3 kJ/kg (range 277 to 284)**

1. c = 10^0.2857 = 1.9307.
2. Compressor: ΔTc = 300 × 0.9307/0.85 = 328.5 K, so T2 = 628.5 K.
3. Turbine: T4' = 1400/1.9307 = 725.1 K, so ΔTt = 0.90 × 674.9 = 607.4 K.
4. Wnet = 1.005 × (607.4 − 328.5) = 280.3 kJ/kg.

For interest, heat added = 1.005 × (1400 − 628.5) = 775.4 kJ/kg, so η = 0.362.

### Q8 · NAT · 2 marks

**Answer: 0.1536 kg/(N·h) (range 0.152 to 0.156)**

1. Momentum thrust = 40 × 1.018 × 520 − 40 × 220 = 21,174.4 − 8,800 = 12,374.4 N.
2. Pressure thrust = 30,000 × 0.15 = 4,500 N, so F = 16,874.4 N.
3. Fuel flow = 0.018 × 40 = 0.72 kg/s.
4. TSFC = 0.72 × 3600/16,874.4 = 0.1536 kg/(N·h).

### Q9 · NAT · 2 marks

**Answer: 0.9149 (range 0.909 to 0.921)**

1. Actual temperature ratio: T03/T04 = 4^(0.90 × 0.25) = 4^0.225 = 1.3660.
2. Isentropic ratio: 4^0.25 = 1.4142.
3. ηt = (1 − 1/1.3660)/(1 − 1/1.4142) = 0.2680/0.2929 = 0.915.

For a turbine the isentropic efficiency exceeds the polytropic value, the reverse of a compressor, because of the reheat effect.

### Q10 · NAT · 2 marks

**Answer: 0.2896 (range 0.286 to 0.293)**

1. Jet velocity: cj = ci + F/ṁ = 240 + 25,000/60 = 656.67 m/s.
2. Propulsive efficiency: ηp = 2 × 240/(240 + 656.67) = 0.5353.
3. Overall efficiency: η0 = F·ci/(ṁf·QR) = (25,000 × 240)/(0.9 × 43 × 10⁶) = 0.1550.
4. Thermal efficiency: ηth = η0/ηp = 0.1550/0.5353 = 0.290.

Check: ½ × 60 × (656.67² − 240²)/(0.9 × 43 × 10⁶) gives the same 0.290.

## Test N2 solutions · Intakes, nozzles and combustors

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 274.5 K (range 273 to 276) |
| 2 | NAT | 1 | 0.9298 (range 0.926 to 0.934) |
| 3 | MCQ | 1 | (B) |
| 4 | NAT | 1 | 0.3746 (range 0.371 to 0.378) |
| 5 | MSQ | 1 | (A), (B), (D) |
| 6 | NAT | 2 | 0.97 (range 0.962 to 0.978) |
| 7 | NAT | 2 | 132.2 kPa (range 131 to 133) |
| 8 | NAT | 2 | 0.1017 m² (range 0.100 to 0.103) |
| 9 | NAT | 2 | 0.02559 (range 0.0253 to 0.0259) |
| 10 | NAT | 2 | 91.52 kPa (range 90.7 to 92.3) |

### Q1 · NAT · 1 mark

**Answer: 274.5 K (range 273 to 276)**

The intake is adiabatic, so T01 = T0a = 250 × (1 + 0.2 × 0.49) = 250 × 1.098 = 274.5 K. Intake losses reduce P01 but never T01.

### Q2 · NAT · 1 mark

**Answer: 0.9298 (range 0.926 to 0.934)**

First bracket: (2.4 × 2.25)/(0.4 × 2.25 + 2) = 5.4/2.9 = 1.8621, raised to 3.5 gives 8.8102. Second bracket: 2.4/(2.8 × 2.25 − 0.4) = 2.4/5.9 = 0.4068, raised to 2.5 gives 0.1055. Their product is 0.9298, so a pitot intake loses only about 7% at Mach 1.5.

### Q3 · MCQ · 1 mark

**Answer: (B)**

The isentropic critical pressure ratio for air is 1.2^3.5 = 1.893. Since 1.7 is below this, the nozzle is unchoked, the exit is subsonic and the jet leaves at ambient pressure. A convergent nozzle can never be over-expanded, which rules out (C).

### Q4 · NAT · 1 mark

**Answer: 0.3746 (range 0.371 to 0.378)**

For CnH2n+2 with n = 10: f\_st = (7n + 1)/(34.32(3n + 1)) = 71/(34.32 × 31) = 0.0667. φ = 0.025/0.0667 = 0.375, a lean overall mixture.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

The primary zone burns near stoichiometric, with recirculation from the swirler holding the flame (A, D). Secondary air completes the burning of CO and unburnt fuel (B). Dilution air lowers the gas temperature to what the turbine can take, so (C) is backwards.

### Q6 · NAT · 2 marks

**Answer: 0.97 (range 0.962 to 0.978)**

1. Use P01/pa = \[1 + ηi × 0.2 × M²\]^3.5.
2. P01/pa = 50/30 = 1.6667, so the bracket = 1.6667^(1/3.5) = 1.15714.
3. ηi = (1.15714 − 1)/(0.2 × 0.81) = 0.15714/0.162 = 0.970.

A loss-free intake would give P0a = 30 × 1.162^3.5 = 50.74 kPa, so this intake loses only about 1.5% of P0.

### Q7 · NAT · 2 marks

**Answer: 132.2 kPa (range 131 to 133)**

1. Critical ratio with losses: 1 − (1/0.97)(1/7) = 0.85272, so P04/Pc = 1/0.85272^4 = 1.8913.
2. P04/pa = 250/90 = 2.778, above 1.891, so the nozzle is choked.
3. Exit pressure Pc = 250/1.8913 = 132.2 kPa, well above ambient.

The exit temperature is Tc = 950 × 6/7 = 814.3 K and the jet speed is √(1.333 × 287 × 814.3) = 558.2 m/s.

### Q8 · NAT · 2 marks

**Answer: 0.1017 m² (range 0.100 to 0.103)**

1. P04/pa = 1.5 is below the critical ratio (about 1.92 with losses), so the nozzle is unchoked and pe = pa = 100 kPa.
2. Isentropic exit temperature: T5' = 800 × (1/1.5)^0.25 = 722.88 K.
3. Actual drop = 0.95 × 77.12 = 73.26 K, so T5 = 726.74 K and cj = √(2 × 1148 × 73.26) = 410.1 m/s.
4. ρ5 = 100,000/(287 × 726.74) = 0.4794 kg/m³.
5. A = ṁ/(ρ5·cj) = 20/(0.4794 × 410.1) = 0.1017 m².

### Q9 · NAT · 2 marks

**Answer: 0.02559 (range 0.0253 to 0.0259)**

1. Energy balance: (1 + f)cpg·T03 = cpa·T02 + f·ηb·QR.
2. f = (1.148 × 1500 − 1.005 × 700)/(0.97 × 42,800 − 1.148 × 1500) = (1722 − 703.5)/(41,516 − 1722).
3. f = 1018.5/39,794 = 0.0256.

### Q10 · NAT · 2 marks

**Answer: 91.52 kPa (range 90.7 to 92.3)**

1. Free-stream: P0a = 20 × (1 + 0.2 × 3.24)^3.5 = 20 × 5.7458 = 114.92 kPa.
2. Normal shock at M = 1.8: P02/P01 = 0.8127 (shock tables or the formula).
3. Compressor face: P01 = 114.92 × 0.8127 × 0.98 = 91.5 kPa.

Overall recovery is 0.796; at higher Mach numbers the normal-shock loss grows quickly, which is why oblique-shock intakes are used.

## Test N3 solutions · Turbojet, turbofan, turboprop, ramjet, afterburner and range

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 50 kg/s |
| 2 | NAT | 1 | 11.43 kN (range 11.3 to 11.6) |
| 3 | MCQ | 1 | (A) |
| 4 | NAT | 1 | 7221 km (range 7148 to 7294) |
| 5 | MSQ | 1 | (A), (B), (C) |
| 6 | NAT | 2 | 608.8 m/s (range 602 to 615) |
| 7 | NAT | 2 | 41.52 kN (range 41.1 to 41.9) |
| 8 | NAT | 2 | 674.1 N·s/kg (range 667 to 681) |
| 9 | NAT | 2 | 0.03081 (range 0.0304 to 0.0312) |
| 10 | NAT | 2 | 0.2567 kg/(kW·h) (range 0.254 to 0.260) |

### Q1 · NAT · 1 mark

**Answer: 50 kg/s**

ṁh = ṁ/(B + 1) = 450/9 = 50 kg/s, and the bypass stream carries the other 400 kg/s.

### Q2 · NAT · 1 mark

**Answer: 11.43 kN (range 11.3 to 11.6)**

Thrust power = ηpr × shaft power = 0.80 × 2000 = 1600 kW. Thrust = 1,600,000/140 = 11,429 N = 11.43 kN.

### Q3 · MCQ · 1 mark

**Answer: (A)**

A ramjet relies entirely on ram compression in its diffuser. At zero speed there is no pressure rise, so burning fuel cannot create a pressure difference to drive a jet. Fuel burns perfectly well (B is false), and nozzle choking (C, D) is irrelevant without a pressure ratio.

### Q4 · NAT · 1 mark

**Answer: 7221 km (range 7148 to 7294)**

TSFC = 0.06/3600 = 1.667 × 10⁻⁵ kg/(N·s), so g·TSFC = 1.635 × 10⁻⁴ s⁻¹. R = (250/1.635 × 10⁻⁴) × 18 × ln 1.3 = 1,529,052 × 18 × 0.2624 = 7,221,035 m, about 7,221 km.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (C)**

The same core energy now accelerates more air to a lower mean jet speed. That raises propulsive efficiency (A) and cuts TSFC (C), but each kilogram of air gives less thrust, so specific thrust falls (B). Jet velocity falls, not rises, so (D) is false.

### Q6 · NAT · 2 marks

**Answer: 608.8 m/s (range 602 to 615)**

1. Compressor: ΔTc = 288 × (6^0.2857 − 1)/0.85 = 288 × 0.6685/0.85 = 226.5 K.
2. Work balance: ΔTt = 1.005 × 226.5/(0.99 × 1.148) = 200.3 K, so T04 = 1150 − 200.3 = 949.7 K.
3. Nozzle: isentropic drop = 949.7 × \[1 − (1/2.2)^0.25\] = 949.7 × 0.1789 = 169.9 K; actual drop = 0.95 × 169.9 = 161.4 K.
4. cj = √(2 × 1148 × 161.4) = 608.8 m/s.

### Q7 · NAT · 2 marks

**Answer: 41.52 kN (range 41.1 to 41.9)**

1. ṁh = 350/7 = 50 kg/s and ṁc = 300 kg/s.
2. Cold stream: 300 × (330 − 240) = 27,000 N.
3. Hot stream: 50 × (1.02 × 520 − 240) = 50 × 290.4 = 14,520 N.
4. F = 27,000 + 14,520 = 41,520 N = 41.52 kN.

Fuel flow = 0.02 × 50 = 1.0 kg/s, so TSFC = 3600/41,520 = 0.0867 kg/(N·h).

### Q8 · NAT · 2 marks

**Answer: 674.1 N·s/kg (range 667 to 681)**

1. u0 = 2.5 × √(1.4 × 287 × 220) = 743.3 m/s.
2. T0a = 220 × (1 + 0.2 × 6.25) = 495 K.
3. Ideal ramjet: ue/u0 = √(T04/T0a) = √(1800/495) = 1.9069.
4. F/ṁ = u0(ue/u0 − 1) = 743.3 × 0.9069 = 674.1 N·s/kg.

Propulsive efficiency = 2/(1 + 1.9069) = 0.688.

### Q9 · NAT · 2 marks

**Answer: 0.03081 (range 0.0304 to 0.0312)**

1. Energy balance on 1 kg of entering gas: (1 + fab)·cpg·T06 = cpg·T05 + fab·ηab·QR.
2. fab = cpg(T06 − T05)/(ηab·QR − cpg·T06) = 1.148 × 1000/(0.92 × 43,000 − 1.148 × 2000).
3. fab = 1148/(39,560 − 2296) = 1148/37,264 = 0.0308.

This is more than the main combustor usually burns, which is why afterburning raises TSFC so sharply.

### Q10 · NAT · 2 marks

**Answer: 0.2567 kg/(kW·h) (range 0.254 to 0.260)**

1. Jet thrust power = 2500 × 160 = 400 kW.
2. Equivalent shaft power = 4000 + 400/0.82 = 4487.8 kW.
3. ESFC = 0.32 × 3600/4487.8 = 0.2567 kg/(kW·h).

## Test N4 solutions · Axial and centrifugal compressors, axial turbines, matching

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 377 m/s (range 375 to 379) |
| 2 | NAT | 1 | 143.3 K (range 142 to 145) |
| 3 | MCQ | 1 | (A) |
| 4 | NAT | 1 | 11 |
| 5 | MSQ | 1 | (A), (B), (C) |
| 6 | NAT | 2 | 1.383 (range 1.37 to 1.40) |
| 7 | NAT | 2 | 0.5837 (range 0.578 to 0.589) |
| 8 | NAT | 2 | 5.064 (range 5.02 to 5.11) |
| 9 | NAT | 2 | 0.4112 (range 0.407 to 0.416) |
| 10 | NAT | 2 | 12.65 (range 12.5 to 12.8) |

### Q1 · NAT · 1 mark

**Answer: 377 m/s (range 375 to 379)**

U = πDN/60 = π × 0.6 × 12,000/60 = 377.0 m/s.

### Q2 · NAT · 1 mark

**Answer: 143.3 K (range 142 to 145)**

ΔT0 = ψσU2²/cp = 1.0 × 0.9 × 400²/1005 = 144,000/1005 = 143.3 K.

### Q3 · MCQ · 1 mark

**Answer: (A)**

A 50% reaction stage has symmetric velocity triangles, so β2 = α1 = 20° and α2 = β1 = 50°. Rotor and stator blades are then mirror images.

### Q4 · NAT · 1 mark

**Answer: 11**

250/24 = 10.42, so 11 stages are needed. Ten stages would give only 240 K.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (C)**

In a 50% reaction stage the triangles are symmetric, so nozzle and rotor blades are mirror images (A). An ideal impulse rotor has no static pressure or enthalpy drop (B). Higher ψ extracts more work per stage, so fewer stages are needed (C). Negative reaction means the rotor diffuses the relative flow and static pressure rises across it, so (D) is false.

### Q6 · NAT · 2 marks

**Answer: 1.383 (range 1.37 to 1.40)**

1. tan58° − tan42° = 1.6003 − 0.9004 = 0.6999.
2. W = λU·Ca(tanβ1 − tanβ2) = 0.95 × 300 × 165 × 0.6999 = 32,914 J/kg.
3. ΔT0s = 32,914/1005 = 32.75 K.
4. Rs = (1 + 0.89 × 32.75/300)^3.5 = 1.09716^3.5 = 1.3834.

### Q7 · NAT · 2 marks

**Answer: 0.5837 (range 0.578 to 0.589)**

1. tanβ1 = U/Ca − tanα1 = 1.8824 − 0.4663 = 1.4160 (β1 = 54.8°).
2. φ = Ca/U = 0.5312.
3. R = (φ/2)(tanβ1 + tanβ2) = 0.2656 × (1.4160 + 0.7813) = 0.584.

Prewhirl in the direction of rotation lowers the relative inlet velocity, which keeps the rotor tip relative Mach number down.

### Q8 · NAT · 2 marks

**Answer: 5.064 (range 5.02 to 5.11)**

1. Slip factor: σ = 1 − 0.63π/20 = 0.9010.
2. Tip speed: U2 = π × 0.45 × 20,000/60 = 471.2 m/s.
3. ΔT0 = ψσU2²/cp = 1.04 × 0.9010 × 471.2²/1005 = 207.1 K.
4. πc = (1 + 0.82 × 207.1/288)^3.5 = 1.5895^3.5 = 5.06.

### Q9 · NAT · 2 marks

**Answer: 0.4112 (range 0.407 to 0.416)**

1. U/Ca = 340/240 = 1.4167, so φ = 0.7059.
2. tanβ2 = tanα2 − U/Ca = 1.8807 − 1.4167 = 0.4641.
3. tanβ3 = tanα3 + U/Ca = 0.2126 + 1.4167 = 1.6292.
4. R = (φ/2)(tanβ3 − tanβ2) = 0.3529 × 1.1652 = 0.411.

The stage work is U·Ca(tanα2 + tanα3) = 170,812 J/kg, a temperature drop of 148.8 K with cpg = 1148 J/kg·K.

### Q10 · NAT · 2 marks

**Answer: 12.65 (range 12.5 to 12.8)**

1. Flow compatibility: ṁ√T01/P01 = (ṁ√T03/P03) × (P03/P02) × (P02/P01) × √(T01/T03).
2. The turbine flow function and P03/P02 are fixed, so at fixed compressor flow, πc is proportional to √(T03/T01).
3. πc = 12 × √(5.0/4.5) = 12 × 1.0541 = 12.65.

Raising T03 pushes the operating point up the constant-flow line toward the surge line.

## Test N5 solutions · Rocket propulsion

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 299.8 s (range 298 to 302) |
| 2 | NAT | 1 | 3779.5 m/s (range 3760 to 3799) |
| 3 | MCQ | 1 | (A) |
| 4 | NAT | 1 | 30 kg/s |
| 5 | MSQ | 1 | (A), (B), (D) |
| 6 | NAT | 2 | 330.3 s (range 328 to 333) |
| 7 | NAT | 2 | 147.1 kg/s (range 146 to 148) |
| 8 | NAT | 2 | 2916.7 m/s (range 2893 to 2941) |
| 9 | NAT | 2 | 8841.6 m/s (range 8770 to 8913) |
| 10 | NAT | 2 | 4.848 MPa (range 4.80 to 4.89) |

### Q1 · NAT · 1 mark

**Answer: 299.8 s (range 298 to 302)**

Isp = F/(ṁ·g0) = 500,000/(170 × 9.81) = 299.8 s. The effective exhaust velocity is 500,000/170 = 2941 m/s.

### Q2 · NAT · 1 mark

**Answer: 3779.5 m/s (range 3760 to 3799)**

ΔV = g0·Isp·ln(m0/mf) = 9.81 × 320 × ln(50/15) = 3139.2 × 1.2040 = 3780 m/s.

### Q3 · MCQ · 1 mark

**Answer: (A)**

Extending the nozzle adds momentum thrust but makes the pressure term (pe − pa)Ae more negative once pe drops below pa. The two effects balance exactly at pe = pa, the optimum expansion condition. Under-expansion (B) wastes available expansion; over-expansion (C) adds negative pressure thrust.

### Q4 · NAT · 1 mark

**Answer: 30 kg/s**

ṁfuel = ṁ/(1 + O/F) = 210/7 = 30 kg/s, and the oxygen flow is 180 kg/s.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Once lit, a solid motor burns its whole grain, so throttling and shutdown are hard (A). Good liquid bipropellants beat solid propellants on Isp (B). A burn-rate pressure exponent n must be below 1 for a stable chamber pressure, so (C) is wrong. A hybrid burns a solid fuel grain with a liquid or gaseous oxidiser (D).

### Q6 · NAT · 2 marks

**Answer: 330.3 s (range 328 to 333)**

1. Momentum thrust = 200 × 3000 = 600,000 N.
2. Pressure thrust = (60 − 20) × 10³ × 1.2 = 48,000 N.
3. F = 648,000 N, so Isp = 648,000/(200 × 9.81) = 330.3 s.

At sea level (101.3 kPa) the pressure term would be −49,560 N, giving Isp = 280.5 s. Isp rises with altitude.

### Q7 · NAT · 2 marks

**Answer: 147.1 kg/s (range 146 to 148)**

1. Throat area: At = F/(CF·Pc) = 400,000/(1.70 × 6 × 10⁶) = 0.03922 m².
2. Mass flow: ṁ = Pc·At/c\* = (6 × 10⁶ × 0.03922)/1600 = 147.1 kg/s.

Shortcut: ṁ = F/(c\*·CF) = 400,000/(1600 × 1.70) = 147.1 kg/s, and Isp = 1600 × 1.70/9.81 = 277.3 s.

### Q8 · NAT · 2 marks

**Answer: 2916.7 m/s (range 2893 to 2941)**

1. R = 8314/20 = 415.7 J/kg·K and 2γ/(γ − 1) = 10.
2. (pe/Pc)^((γ − 1)/γ) = (1/100)^0.2 = 0.3981, so the bracket is 0.6019.
3. ve = √(10 × 415.7 × 3400 × 0.6019) = √(8,507,033) = 2917 m/s.

With pe = pa this gives Isp = 2917/9.81 = 297 s.

### Q9 · NAT · 2 marks

**Answer: 8841.6 m/s (range 8770 to 8913)**

1. Stage mass ratio n = (1 + λ)/(ε + λ) = 1.15/0.23 = 5.0.
2. Each stage gives g0·Isp·ln n = 9.81 × 280 × ln 5 = 4421 m/s.
3. Two stages: ΔV = 8842 m/s.

### Q10 · NAT · 2 marks

**Answer: 4.848 MPa (range 4.80 to 4.89)**

1. Mass balance: ρp·Ab·a·Pc^n = Pc·At/c\*, so Pc^(1 − n) = ρp·a·c\*·(Ab/At) in consistent units.
2. With a = 5 × 10⁻³ m/s per MPa^0.35 and Pc in MPa: Pc^0.65 = (1800 × 5 × 10⁻³ × 1550 × 200)/10⁶ = 2.790.
3. Pc = 2.790^(1/0.65) = 4.85 MPa, and the burn rate is 5 × 4.85^0.35 = 8.69 mm/s.

Sensitivity: a 10% rise in Ab/At raises Pc by 1.1^(1/0.65) − 1 = 15.8%, which is why grain cracks are dangerous.

## Test N6 solutions · Full-syllabus GATE-level mock

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | NAT | 1 | 14.79 kN (range 14.7 to 14.9) |
| 2 | MCQ | 1 | (C) |
| 3 | NAT | 1 | 0.7222 (range 0.717 to 0.727) |
| 4 | NAT | 1 | 0.05828 (range 0.0579 to 0.0587) |
| 5 | NAT | 1 | 11757.6 rpm (range 11722 to 11793) |
| 6 | MSQ | 1 | (A), (C), (D) |
| 7 | NAT | 2 | 597.4 N·s/kg (range 590 to 605) |
| 8 | NAT | 2 | 13 |
| 9 | NAT | 2 | 787.9 kW (range 781 to 795) |
| 10 | NAT | 2 | 61.7° (range 61.3 to 62.1) |
| 11 | NAT | 2 | 1.555 (range 1.54 to 1.57) |
| 12 | NAT | 2 | 7826.9 km (range 7748 to 7906) |

### Q1 · NAT · 1 mark

**Answer: 14.79 kN (range 14.7 to 14.9)**

With ci = 0 there is no ram drag: F = ṁa(1 + f)cj = 25 × 1.02 × 580 = 14,790 N = 14.79 kN.

### Q2 · MCQ · 1 mark

**Answer: (C)**

Impulse blading has β2 = β3, so Wt2 = Wt3. Axial exit gives Wt3 = U, while Wt2 = Ct2 − U, so Ct2 = 2U. The work is U(Ct2 + Ct3) = 2U², giving ψ = 2. A 50% reaction stage with axial exit gives ψ = 1.

### Q3 · NAT · 1 mark

**Answer: 0.7222 (range 0.717 to 0.727)**

ε = (Tg − Tb)/(Tg − Tc) = (1800 − 1150)/(1800 − 900) = 650/900 = 0.722.

### Q4 · NAT · 1 mark

**Answer: 0.05828 (range 0.0579 to 0.0587)**

CH4 + 2(O2 + 3.76N2) → CO2 + 2H2O + 7.52N2. Air mass = 2 × 137.28 = 274.56 g per 16 g of fuel, so f\_st = 16/274.56 = 0.0583. The CnH2n+2 formula with n = 1 gives 8/(34.32 × 4), the same value.

### Q5 · NAT · 1 mark

**Answer: 11757.6 rpm (range 11722 to 11793)**

N/√T01 is held fixed, so Ncorr = 12,000 × √(288/300) = 12,000 × 0.97980 = 11,758 rpm.

### Q6 · MSQ · 1 mark

**Answer: (A), (C), (D)**

An air-breathing engine takes its oxidiser from the air, so its Isp based on fuel flow (thousands of seconds) far exceeds a rocket's (A). A rocket's thrust does not depend on flight speed, so (B) is false. At subsonic speeds a ramjet has little ram compression, so its TSFC is far worse than a turbojet's (C). At the same thrust and flight speed a turbofan's lower jet speed gives a higher ηp (D).

### Q7 · NAT · 2 marks

**Answer: 597.4 N·s/kg (range 590 to 605)**

1. Compressor: ΔTc = 288 × (5^0.2857 − 1)/0.85 = 197.8 K, so T02 = 485.8 K; P02 = 506.5 kPa and P03 = 0.96 × 506.5 = 486.2 kPa.
2. Turbine: ΔTt = 1.005 × 197.8/(0.99 × 1.148) = 174.9 K, so T04 = 925.1 K. T04' = 1100 − 174.9/0.88 = 901.2 K, so P03/P04 = (1100/901.2)^4 = 2.2194 and P04 = 219.1 kPa.
3. Nozzle: P04/pa = 2.163, above the critical 1.919, so it is choked. Tc = 925.1 × 6/7 = 792.9 K, cj = √(1.333 × 287 × 792.9) = 550.8 m/s, Pc = 219.1/1.919 = 114.2 kPa.
4. A/ṁ = RTc/(Pc·cj) = (287 × 792.9)/(114,162 × 550.8) = 0.003619 m²·s/kg.
5. Fs = cj + (Pc − pa)·A/ṁ = 550.8 + 12,862 × 0.003619 = 550.8 + 46.5 = 597.4 N·s/kg.

### Q8 · NAT · 2 marks

**Answer: 13**

1. With polytropic efficiency: T02/T01 = 12^(0.2857/0.90) = 12^0.3175 = 2.2009.
2. Overall ΔT0 = 288 × 1.2009 = 345.9 K.
3. Stages = 345.9/28 = 12.35, so 13 stages are needed.

### Q9 · NAT · 2 marks

**Answer: 787.9 kW (range 781 to 795)**

1. Tip speed: U2 = π × 0.40 × 22,000/60 = 460.8 m/s.
2. Slip factor: σ = 1 − 0.63π/17 = 0.8836.
3. Power = ṁ·ψ·σ·U2² = 4 × 1.05 × 0.8836 × 460.8² = 787,872 W = 787.9 kW.

### Q10 · NAT · 2 marks

**Answer: 61.7° (range 61.3 to 62.1)**

1. ψ = φ(tanβ2 + tanβ3) gives tanβ2 + tanβ3 = 1.6/0.7 = 2.2857.
2. R = (φ/2)(tanβ3 − tanβ2) = 0.5 gives tanβ3 − tanβ2 = 1/0.7 = 1.4286.
3. So tanβ3 = 1.8571 (β3 = 61.7°) and tanβ2 = 0.4286 (β2 = 23.2°).
4. For 50% reaction the triangles are symmetric, so α2 = β3 = 61.7° and α3 = β2 = 23.2°.

### Q11 · NAT · 2 marks

**Answer: 1.555 (range 1.54 to 1.57)**

For optimum expansion the pressure term vanishes and CF = √{(2γ²/(γ − 1)) · (2/(γ + 1))^((γ + 1)/(γ − 1)) · \[1 − (pe/Pc)^((γ − 1)/γ)\]}.

1. 2γ²/(γ − 1) = 2 × 1.44/0.2 = 14.40.
2. (2/2.2)^(2.2/0.2) = 0.9091^11 = 0.3505.
3. 1 − (1/50)^(0.2/1.2) = 1 − 0.5210 = 0.4790.
4. CF = √(14.40 × 0.3505 × 0.4790) = √2.4176 = 1.555.

Combined with c\* this gives the effective exhaust velocity: c = c\*·CF.

### Q12 · NAT · 2 marks

**Answer: 7826.9 km (range 7748 to 7906)**

1. Since η0 = F·V/(ṁf·QR) and F = D in cruise, V/(g·TSFC) = η0·QR/g, so R = η0·(QR/g)·(L/D)·ln(Wi/Wf).
2. QR/g = 43 × 10⁶/9.81 = 4,383,282 m.
3. R = 0.35 × 4,383,282 × 17 × ln 1.35 = 0.35 × 4,383,282 × 17 × 0.3001 = 7,826,887 m, about 7,827 km.

In this form, range depends only on overall efficiency, fuel energy, aerodynamic efficiency and fuel fraction, not on speed separately.

## Test C1 solutions · Cycles, thrust, efficiencies and engine types

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | MCQ | 1 | (A) |
| 2 | MCQ | 1 | (A) |
| 3 | MCQ | 1 | (B) |
| 4 | NAT | 1 | 1.667 (range 1.66 to 1.67) |
| 5 | NAT | 1 | 0.5 (range 0.490 to 0.510) |
| 6 | MCQ | 1 | (B) |
| 7 | MCQ | 1 | (D) |
| 8 | MSQ | 1 | (A), (C), (D) |
| 9 | MCQ | 1 | (B) |
| 10 | MCQ | 1 | (C) |
| 11 | MCQ | 1 | (A) |
| 12 | MSQ | 1 | (A), (C), (D) |
| 13 | MCQ | 1 | (D) |
| 14 | MCQ | 1 | (C) |
| 15 | MSQ | 1 | (A), (D) |

### Q1 · MCQ · 1 mark

**Answer: (A)**

No heat or work crosses the nozzle, so h0, and with it T0, stays constant. Friction lowers P0 and raises entropy, and static temperature falls as the gas speeds up.

### Q2 · MCQ · 1 mark

**Answer: (A)**

η = 1 − 1/r^((γ − 1)/γ) contains no temperature. Turbine inlet temperature changes the specific work, not the ideal efficiency.

### Q3 · MCQ · 1 mark

**Answer: (B)**

Maximum work occurs at c = √(T3/T1), which makes T2 = T4 = √(T1·T3). Pushing the pressure ratio to its maximum (T2 = T3) drives the work to zero.

### Q4 · NAT · 1 mark

**Answer: 1.667 (range 1.66 to 1.67)**

γ = 1 + 2/f = 1 + 2/3 = 5/3 = 1.667. A diatomic gas with 5 degrees of freedom gives the familiar 1.4.

### Q5 · NAT · 1 mark

**Answer: 0.5 (range 0.490 to 0.510)**

ηp = 2/(1 + cj/ci) = 2/(1 + 3) = 0.5.

### Q6 · MCQ · 1 mark

**Answer: (B)**

ηp = 2/(1 + cj/ci) equals 1 when cj = ci. But thrust ṁ(cj − ci) is then zero, so no practical engine runs there.

### Q7 · MCQ · 1 mark

**Answer: (D)**

A high-bypass turbofan moves the most air at the lowest jet speed for a given thrust, so its jet speed is closest to the flight speed. A ramjet barely works at Mach 0.8.

### Q8 · MSQ · 1 mark

**Answer: (A), (C), (D)**

TSFC is fuel flow per unit thrust, so lower is better (C), and kg/(N·h) is a common unit (A). Turbofans beat turbojets at subsonic cruise (D). A ramjet has almost no compression at subsonic speed, so its TSFC is the worst, not the best.

### Q9 · MCQ · 1 mark

**Answer: (B)**

The engine must take free-stream air moving at ci and bring it along, which costs momentum ṁa·ci. That is the negative term in F = (ṁa + ṁf)cj − ṁa·ci + (pe − pa)Ae.

### Q10 · MCQ · 1 mark

**Answer: (C)**

Each stage's losses heat the air entering the next stage, which then needs more work. So the overall isentropic efficiency falls below the stage (polytropic) value, and the gap grows with pressure ratio.

### Q11 · MCQ · 1 mark

**Answer: (A)**

With losses, turbine work grows with T3 while compressor work stays fixed, so both net work and efficiency rise. Option (C) is true only for the ideal cycle, which is the trap here.

### Q12 · MSQ · 1 mark

**Answer: (A), (C), (D)**

A propeller moves a huge mass of air slowly, so ηp is high at low speed (A), but its tips go transonic as flight speed rises (D). A turboprop gets most of its thrust from the propeller, not the jet, so (B) is false. A turboshaft drives a rotor or generator (C).

### Q13 · MCQ · 1 mark

**Answer: (D)**

A ramjet has no rotating parts. It slows the incoming air in its diffuser, converting kinetic energy into pressure, which is why it needs forward speed to work.

### Q14 · MCQ · 1 mark

**Answer: (C)**

The turbine extracts just enough work to drive the compressor and accessories. The remaining energy expands in the nozzle to produce thrust.

### Q15 · MSQ · 1 mark

**Answer: (A), (D)**

Thrust scales with mass flow, which falls with density (A, D). Ram drag ṁa·ci actually falls with mass flow. A colder intake raises T03/T01 and helps the cycle, partly offsetting the loss, so (C) is wrong.

## Test C2 solutions · Intakes, nozzles, combustors and afterburners

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | MCQ | 1 | (C) |
| 2 | MCQ | 1 | (C) |
| 3 | MCQ | 1 | (C) |
| 4 | MCQ | 1 | (B) |
| 5 | MSQ | 1 | (B), (C) |
| 6 | MCQ | 1 | (A) |
| 7 | MCQ | 1 | (D) |
| 8 | MCQ | 1 | (C) |
| 9 | MSQ | 1 | (B), (C) |
| 10 | MCQ | 1 | (D) |
| 11 | MCQ | 1 | (B) |
| 12 | MCQ | 1 | (A) |
| 13 | MSQ | 1 | (A), (C), (D) |
| 14 | MCQ | 1 | (D) |
| 15 | MCQ | 1 | (B) |

### Q1 · MCQ · 1 mark

**Answer: (C)**

The intake is adiabatic with no work, so T0 is unchanged. Friction lowers P0, while static pressure rises and Mach number falls as the air slows.

### Q2 · MCQ · 1 mark

**Answer: (C)**

From dA/A = (M² − 1)du/u, subsonic flow (M < 1) slows down when the area increases.

### Q3 · MCQ · 1 mark

**Answer: (C)**

With M > 1, the factor (M² − 1) is positive, so du < 0 needs dA < 0. A supersonic diffuser therefore converges, the reverse of the subsonic case.

### Q4 · MCQ · 1 mark

**Answer: (B)**

Shock loss rises steeply with the normal Mach number. Several weak shocks compress the air with far less P0 loss than one strong normal shock.

### Q5 · MSQ · 1 mark

**Answer: (B), (C)**

Choking fixes M = 1 at the exit (C) and the flow per unit area at a value set by P04 and T04 (B). Exit pressure then exceeds ambient, giving pressure thrust, and downstream changes cannot raise the flow.

### Q6 · MCQ · 1 mark

**Answer: (A)**

Under-expanded means pe > pa, so the jet keeps expanding outside the nozzle through expansion fans. Shocks and separation belong to over-expanded nozzles.

### Q7 · MCQ · 1 mark

**Answer: (D)**

With losses, a larger pressure ratio is needed to reach sonic speed. For γ = 4/3 it rises from 1.853 to 1.919 at ηj = 0.95.

### Q8 · MCQ · 1 mark

**Answer: (C)**

The primary zone burns near stoichiometric to give a stable, fast-burning flame. The overall mixture is much leaner (φ ≈ 0.3) once secondary and dilution air are added.

### Q9 · MSQ · 1 mark

**Answer: (B), (C)**

Dilution air is added last to bring the gas down to the turbine limit and smooth its profile (B, C). The recirculating primary zone anchors the flame, and the primary air supplies its oxygen.

### Q10 · MCQ · 1 mark

**Answer: (D)**

Reaction rate falls with pressure, so the combustor must still burn stably and relight at the lowest pressure it will meet, at high altitude.

### Q11 · MCQ · 1 mark

**Answer: (B)**

Adding heat lowers the density, so the gas accelerates and stagnation pressure falls (Rayleigh flow). Friction gives the separate cold loss.

### Q12 · MCQ · 1 mark

**Answer: (A)**

Burning extra fuel in the jet pipe raises T0, and jet velocity scales with √T0 at a given nozzle pressure ratio. Mass flow and P0 do not rise; P0 actually falls slightly.

### Q13 · MSQ · 1 mark

**Answer: (A), (C), (D)**

The nozzle must open to pass the hotter, less dense gas (C), and flame holders stabilise the flame in the fast jet-pipe flow (D). Heat is added at low pressure, so efficiency falls and TSFC rises sharply.

### Q14 · MCQ · 1 mark

**Answer: (D)**

An annular liner wraps the whole engine, saving length, weight and loss. Cans are easier to develop, and separate flame tubes with crossfire tubes describe can or can-annular designs.

### Q15 · MCQ · 1 mark

**Answer: (B)**

Heat transfer rises with mass flux ρu, which peaks at the throat where the area is smallest. That is why throats get the most intense cooling.

## Test C3 solutions · Turbomachinery, blade cooling, surge and matching

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | MCQ | 1 | (B) |
| 2 | MCQ | 1 | (A) |
| 3 | MCQ | 1 | (D) |
| 4 | MCQ | 1 | (C) |
| 5 | MCQ | 1 | (A) |
| 6 | MSQ | 1 | (A), (B), (D) |
| 7 | MCQ | 1 | (D) |
| 8 | MCQ | 1 | (D) |
| 9 | MCQ | 1 | (A) |
| 10 | MCQ | 1 | (A) |
| 11 | MCQ | 1 | (B) |
| 12 | MCQ | 1 | (B) |
| 13 | MCQ | 1 | (C) |
| 14 | MSQ | 1 | (A), (C), (D) |
| 15 | MCQ | 1 | (C) |

### Q1 · MCQ · 1 mark

**Answer: (B)**

A stator does no work, so h0 is constant. It turns and slows the absolute flow, converting kinetic energy into static pressure.

### Q2 · MCQ · 1 mark

**Answer: (A)**

Equal enthalpy rise in rotor and stator makes the velocity triangles symmetric, so rotor and stator blades are mirror images.

### Q3 · MCQ · 1 mark

**Answer: (D)**

As the annulus boundary layers thicken, mid-span axial velocity rises and the blades there do less work. The average stage work drops, which λ accounts for.

### Q4 · MCQ · 1 mark

**Answer: (C)**

W2/W1 measures how much the rotor slows the relative flow. Too much deceleration against the adverse pressure gradient separates the boundary layer.

### Q5 · MCQ · 1 mark

**Answer: (A)**

Accelerating turbine flow keeps boundary layers thin, so large turning and expansion are possible. Decelerating compressor flow separates if pushed too hard.

### Q6 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Surge is a system-wide oscillation (A), while rotating stall is local stalled cells moving around the annulus (D). Both happen at low flow, not high, so (C) is false. Bleeding air mid-way relieves the front stages (B).

### Q7 · MCQ · 1 mark

**Answer: (D)**

Once some passage reaches sonic speed, the mass flow cannot rise further. Each speed line then drops almost vertically at its maximum flow.

### Q8 · MCQ · 1 mark

**Answer: (D)**

The relative eddy in the passage means the air does not leave at the blade angle, so Ct2 < U2 and σ = Ct2/U2 < 1. Slip reduces the work the impeller can do.

### Q9 · MCQ · 1 mark

**Answer: (A)**

Extra work is spent on disc friction and windage, so the work input is ψσU2² with ψ slightly above 1, typically 1.03 to 1.05.

### Q10 · MCQ · 1 mark

**Answer: (A)**

W = U2² − U2·Cr2·cotβ2 falls with flow for backward vanes, which is stabilising. Radial vanes give constant work and forward vanes a rising, unstable curve.

### Q11 · MCQ · 1 mark

**Answer: (B)**

The rotor does work, so h0 changes. Rothalpy is the rotating-frame equivalent that stays constant; for an axial rotor with constant U it reduces to h + W²/2.

### Q12 · MCQ · 1 mark

**Answer: (B)**

All the expansion happens in the nozzles. The rotor only turns the flow at constant relative speed, so static pressure and enthalpy stay the same across it.

### Q13 · MCQ · 1 mark

**Answer: (C)**

Negative reaction means static enthalpy rises in the rotor, so W3 < W2 and the rotor acts as a diffuser. Designers avoid it because diffusing passages lose more.

### Q14 · MSQ · 1 mark

**Answer: (A), (C), (D)**

Film, impingement and convection cooling keep the metal below the gas temperature, and ceramic thermal barrier coatings insulate it (A, C, D). Hot turbine blades are nickel-based superalloys; aluminium would melt.

### Q15 · MCQ · 1 mark

**Answer: (C)**

ṁ√T01/P01 is fixed, so ṁ is proportional to P01/√T01. P01 falls much faster than √T01 with altitude, so the actual mass flow drops.

## Test C4 solutions · Rockets and cross-topic traps

| Q | Type | Marks | Answer |
| --- | --- | --- | --- |
| 1 | MCQ | 1 | (C) |
| 2 | MCQ | 1 | (A) |
| 3 | MCQ | 1 | (A) |
| 4 | MCQ | 1 | (C) |
| 5 | MSQ | 1 | (A), (B), (D) |
| 6 | MCQ | 1 | (C) |
| 7 | MCQ | 1 | (B) |
| 8 | MCQ | 1 | (B) |
| 9 | MCQ | 1 | (A) |
| 10 | MSQ | 1 | (A), (D) |
| 11 | MCQ | 1 | (B) |
| 12 | MCQ | 1 | (D) |
| 13 | MCQ | 1 | (D) |
| 14 | MSQ | 1 | (A), (B), (D) |
| 15 | MCQ | 1 | (D) |

### Q1 · MCQ · 1 mark

**Answer: (C)**

A rocket takes in no air, so there is no ram drag and F = ṁve + (pe − pa)Ae does not contain flight speed. Thrust changes with altitude through pa, not with speed.

### Q2 · MCQ · 1 mark

**Answer: (A)**

In vacuum pa = 0, so the pressure term (pe − pa)Ae is largest. More thrust for the same propellant flow means higher Isp.

### Q3 · MCQ · 1 mark

**Answer: (A)**

c\* = Pc·At/ṁ depends on T0, molar mass and γ of the combustion products, not on the nozzle's expansion. CF measures the nozzle.

### Q4 · MCQ · 1 mark

**Answer: (C)**

CF = F/(Pc·At) captures how well the nozzle turns chamber pressure into thrust, so it depends on expansion and back pressure. Chamber temperature enters through c\*, not CF.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Dropping empty tanks and engines is the core benefit (B, D), and upper stages can use large-area-ratio nozzles for vacuum (A). Staging does not change an engine's own Isp, so (C) is false.

### Q6 · MCQ · 1 mark

**Answer: (C)**

With n < 1, a pressure rise increases nozzle outflow (proportional to Pc) faster than gas generation (proportional to Pc^n), so the pressure returns to equilibrium. With n > 1 it runs away.

### Q7 · MCQ · 1 mark

**Answer: (B)**

High cross-flow velocity in the port thins the boundary layer and raises heat transfer to the propellant, so it burns faster. It matters most early in the burn, when the port is narrow.

### Q8 · MCQ · 1 mark

**Answer: (B)**

Exhaust velocity scales roughly with √(T0/M). LOX/LH2 exhaust is mostly water and excess hydrogen, with a very low molar mass. Its flame temperature is not unusually high, and its density is very low.

### Q9 · MCQ · 1 mark

**Answer: (A)**

ηp = 2(u/c)/(1 + (u/c)²) peaks at 1 when u = c, because the exhaust is then left at rest relative to the ground. Unlike a jet engine, the rocket still has full thrust there.

### Q10 · MSQ · 1 mark

**Answer: (A), (D)**

A shock is adiabatic and does no work, so T0 is constant (D), and continuity keeps ρu constant (A). It is irreversible, so P0 falls and entropy rises; that is the trap.

### Q11 · MCQ · 1 mark

**Answer: (B)**

An air-breathing engine carries only fuel and takes its oxidiser free from the air, so its thrust per unit of carried propellant is much higher. A rocket must carry its oxidiser too.

### Q12 · MCQ · 1 mark

**Answer: (D)**

Gravity loss is roughly the integral of g·cosθ over the burn, so finishing the burn sooner and turning toward horizontal both cut it. This is the impulsive launch idea in your notes.

### Q13 · MCQ · 1 mark

**Answer: (D)**

Flow accelerates to sonic speed at the throat and becomes supersonic in the diverging section. That needs M = 1 exactly at the minimum area.

### Q14 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Compressors divide ideal by actual work (A); turbines and nozzles divide actual by ideal (B, D). P01/P0a is the pressure recovery factor, not the isentropic efficiency, so (C) is the trap.

### Q15 · MCQ · 1 mark

**Answer: (D)**

Hypergolic pairs such as N2O4 with MMH ignite on contact, so they suit spacecraft thrusters that restart many times. They are toxic, storable at room temperature, and have moderate Isp.
