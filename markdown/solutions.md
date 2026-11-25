# GATE AE Propulsion Test Series: Solutions

Last updated 25 Nov 2026

## How to score yourself

Check each answer against the key at the top of its test, then read the worked solution for every question you got wrong or guessed.

The questions are in [GATE AE Propulsion Test Series: Question Papers](question-papers.md), and the same tests run online with a timer and automatic scoring at [Propulsion Mock Tests](https://abhishek4650.github.io/gate-ae-propulsion-test-series/).

- MCQ: +1 or +2 if correct; $`\displaystyle - \frac{1}{3}`$ or $`\displaystyle - \frac{2}{3}`$ if wrong; 0 if left blank.
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

$`T_0 = T (1 + 0.2 M^{2})`$​$`{} = 250 \times (1 + 0.2 \times 4)`$​$`{} = 250 \times 1.8`$​$`{} = 450\ \mathrm{K}`$.

### Q2 · MCQ · 1 mark

**Answer: (B)**

$`C_v = C_p - R`$​$`{} = 0.80\ \mathrm{kJ/kg{\cdot}K}`$, so $`\displaystyle \gamma = \frac{C_p}{C_v}`$​$`\displaystyle {} = \frac{1.10}{0.80}`$​$`{} = 1.375`$. Option (D) is the hot-gas value and (C) is air; neither applies here.

### Q3 · NAT · 1 mark

**Answer: 54.71% (range 54.3 to 55.1)**

$`c = 16^{0.2857}`$​$`{} = 2.2082`$. $`\displaystyle \eta = 1 - \frac{1}{c}`$​$`{} = 1 - 0.4529`$​$`{} = 0.5471`$, or 54.7%.

### Q4 · NAT · 1 mark

**Answer: 0.5 (range 0.495 to 0.505)**

$`\displaystyle \eta_{\mathrm{p}} = \frac{2 C_{\mathrm{i}}}{C_{\mathrm{i}} + C_{\mathrm{j}}}`$​$`\displaystyle {} = \frac{500}{1000}`$​$`{} = 0.50`$. Equivalently $`\displaystyle \eta_{\mathrm{p}} = \frac{2}{1 + \frac{C_{\mathrm{j}}}{C_{\mathrm{i}}}}`$​$`\displaystyle {} = \frac{2}{1 + 3}`$​$`{} = 0.5`$.

### Q5 · MSQ · 1 mark

**Answer: (A), (C)**

Thrust $`= \dot m (C_{\mathrm{j}} - C_{\mathrm{i}})`$ can be had from more air at a lower jet speed, which wastes less kinetic energy in the jet. That is (A), and a higher bypass ratio (C) does exactly this. (B) is the opposite. Afterburning (D) raises jet speed, so $`\eta_{\mathrm{p}}`$ falls.

### Q6 · NAT · 2 marks

**Answer: 17.96 (range 17.8 to 18.2)**

1. $`\displaystyle t = \frac{T_3}{T_1}`$​$`\displaystyle {} = \frac{1500}{288}`$​$`{} = 5.2083`$.
2. Maximum work needs $`c = \sqrt{t}`$​$`{} = 2.2822`$, which makes $`T_2 = T_4`$.
3. $`\displaystyle r = c^{\frac{\gamma}{\gamma - 1}}`$​$`{} = 2.2822^{3.5}`$​$`\displaystyle {} = \left(\frac{T_3}{T_1}\right)^{1.75}`$​$`{} = 17.96`$.

The cycle efficiency at this pressure ratio is $`\displaystyle 1 - \frac{1}{\sqrt{t}} = 0.562`$.

### Q7 · NAT · 2 marks

**Answer: 280.3 kJ/kg (range 277 to 284)**

1. $`c = 10^{0.2857}`$​$`{} = 1.9307`$.
2. Compressor: $`\displaystyle \Delta T_{\mathrm{c}} = \frac{300 \times 0.9307}{0.85}`$​$`{} = 328.5\ \mathrm{K}`$, so $`T_2 = 628.5\ \mathrm{K}`$.
3. Turbine: $`\displaystyle T_4' = \frac{1400}{1.9307}`$​$`{} = 725.1\ \mathrm{K}`$, so $`\Delta T_{\mathrm{t}} = 0.90 \times 674.9`$​$`{} = 607.4\ \mathrm{K}`$.
4. $`W_{\mathrm{net}} = 1.005 \times {}`$​$`(607.4 - 328.5)`$​$`{} = 280.3\ \mathrm{kJ/kg}`$.

For interest, heat added $`= 1.005 \times (1400 - 628.5)`$​$`{} = 775.4\ \mathrm{kJ/kg}`$, so $`\eta = 0.362`$.

### Q8 · NAT · 2 marks

**Answer: 0.1536 kg/(N·h) (range 0.152 to 0.156)**

1. Momentum thrust $`= 40 \times 1.018 \times 520 - 40 \times {}`$​$`220`$​$`{} = 21{,}174.4 - 8{,}800`$​$`{} = 12{,}374.4\ \mathrm{N}`$.
2. Pressure thrust $`= 30{,}000 \times 0.15 = 4{,}500\ \mathrm{N}`$, so $`F = 16{,}874.4\ \mathrm{N}`$.
3. Fuel flow $`= 0.018 \times 40 = 0.72\ \mathrm{kg/s}`$.
4. $`\mathrm{TSFC} = 0.72 \times {}`$​$`\displaystyle \frac{3600}{16{,}874.4}`$​$`{} = 0.1536\ \mathrm{kg/(N{\cdot}h)}`$.

### Q9 · NAT · 2 marks

**Answer: 0.9149 (range 0.909 to 0.921)**

1. Actual temperature ratio: $`\displaystyle \frac{T_{03}}{T_{04}} = 4^{0.90 \times 0.25}`$​$`{} = 4^{0.225}`$​$`{} = 1.3660`$.
2. Isentropic ratio: $`4^{0.25} = 1.4142`$.
3. $`\displaystyle \eta_{\mathrm{t}} = \frac{1 - \frac{1}{1.3660}}{1 - \frac{1}{1.4142}}`$​$`\displaystyle {} = \frac{0.2680}{0.2929}`$​$`{} = 0.915`$.

For a turbine the isentropic efficiency exceeds the polytropic value, the reverse of a compressor, because of the reheat effect.

### Q10 · NAT · 2 marks

**Answer: 0.2896 (range 0.286 to 0.293)**

1. Jet velocity: $`\displaystyle C_{\mathrm{j}} = C_{\mathrm{i}} + \frac{F}{\dot m}`$​$`\displaystyle {} = 240 + \frac{25{,}000}{60}`$​$`{} = 656.67\ \mathrm{m/s}`$.
2. Propulsive efficiency: $`\eta_{\mathrm{p}} = 2 \times {}`$​$`\displaystyle \frac{240}{240 + 656.67}`$​$`{} = 0.5353`$.
3. Overall efficiency: $`\displaystyle \eta_{\mathrm{ov}} = \frac{F\,C_{\mathrm{i}}}{\dot m_{\mathrm{f}}\,Q_{\mathrm{cv}}}`$​$`\displaystyle {} = \frac{25{,}000 \times 240}{0.9 \times 43 \times 10^{6}}`$​$`{} = 0.1550`$.
4. Thermal efficiency: $`\displaystyle \eta_{\mathrm{th}} = \frac{\eta_{\mathrm{ov}}}{\eta_{\mathrm{p}}}`$​$`\displaystyle {} = \frac{0.1550}{0.5353}`$​$`{} = 0.290`$.

Check: $`\tfrac{1}{2} \times 60 \times {}`$​$`\displaystyle \frac{656.67^{2} - 240^{2}}{0.9 \times 43 \times 10^{6}}`$ gives the same 0.290.

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

The intake is adiabatic, so $`T_{01} = T_{0\mathrm{a}}`$​$`{} = 250 \times (1 + 0.2 \times 0.49)`$​$`{} = 250 \times 1.098`$​$`{} = 274.5\ \mathrm{K}`$. Intake losses reduce $`P_{01}`$ but never $`T_{01}`$.

### Q2 · NAT · 1 mark

**Answer: 0.9298 (range 0.926 to 0.934)**

First bracket: $`\displaystyle \frac{2.4 \times 2.25}{0.4 \times 2.25 + 2}`$​$`\displaystyle {} = \frac{5.4}{2.9}`$​$`{} = 1.8621`$, raised to 3.5 gives 8.8102. Second bracket: $`\displaystyle \frac{2.4}{2.8 \times 2.25 - 0.4}`$​$`\displaystyle {} = \frac{2.4}{5.9}`$​$`{} = 0.4068`$, raised to 2.5 gives 0.1055. Their product is 0.9298, so a pitot intake loses only about 7% at Mach 1.5.

### Q3 · MCQ · 1 mark

**Answer: (B)**

The isentropic critical pressure ratio for air is $`1.2^{3.5} = 1.893`$. Since 1.7 is below this, the nozzle is unchoked, the exit is subsonic and the jet leaves at ambient pressure. A convergent nozzle can never be over-expanded, which rules out (C).

### Q4 · NAT · 1 mark

**Answer: 0.3746 (range 0.371 to 0.378)**

For $`\mathrm{C}_n\mathrm{H}_{2n+2}`$ with $`n = 10`$: $`\displaystyle f_{\mathrm{st}} = \frac{7 n + 1}{34.32 (3 n + 1)}`$​$`\displaystyle {} = \frac{71}{34.32 \times 31}`$​$`{} = 0.0667`$. $`\displaystyle \phi = \frac{0.025}{0.0667}`$​$`{} = 0.375`$, a lean overall mixture.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

The primary zone burns near stoichiometric, with recirculation from the swirler holding the flame (A, D). Secondary air completes the burning of CO and unburnt fuel (B). Dilution air lowers the gas temperature to what the turbine can take, so (C) is backwards.

### Q6 · NAT · 2 marks

**Answer: 0.97 (range 0.962 to 0.978)**

1. Use $`\displaystyle \frac{P_{01}}{P_{\mathrm{a}}} = [1 + \eta_{\mathrm{in}} \times 0.2 \times M^{2}]^{3.5}`$.
2. $`\displaystyle \frac{P_{01}}{P_{\mathrm{a}}} = \frac{50}{30}`$​$`{} = 1.6667`$, so the bracket $`\displaystyle = 1.6667^{\frac{1}{3.5}} = 1.15714`$.
3. $`\displaystyle \eta_{\mathrm{in}} = \frac{1.15714 - 1}{0.2 \times 0.81}`$​$`\displaystyle {} = \frac{0.15714}{0.162}`$​$`{} = 0.970`$.

A loss-free intake would give $`P_{0\mathrm{a}} = 30 \times 1.162^{3.5}`$​$`{} = 50.74\ \mathrm{kPa}`$, so this intake loses only about 1.5% of $`P_0`$.

### Q7 · NAT · 2 marks

**Answer: 132.2 kPa (range 131 to 133)**

1. Critical ratio with losses: $`\displaystyle 1 - \left(\frac{1}{0.97}\right) \left(\frac{1}{7}\right)`$​$`{} = 0.85272`$, so $`\displaystyle \frac{P_{04}}{P_{\mathrm{c}}} = \frac{1}{0.85272^{4}}`$​$`{} = 1.8913`$.
2. $`\displaystyle \frac{P_{04}}{P_{\mathrm{a}}} = \frac{250}{90}`$​$`{} = 2.778`$, above 1.891, so the nozzle is choked.
3. Exit pressure $`\displaystyle P_{\mathrm{c}} = \frac{250}{1.8913}`$​$`{} = 132.2\ \mathrm{kPa}`$, well above ambient.

The exit temperature is $`\displaystyle T_{\mathrm{c}} = \frac{950 \times 6}{7}`$​$`{} = 814.3\ \mathrm{K}`$ and the jet speed is $`\sqrt{1.333 \times 287 \times 814.3}`$​$`{} = 558.2\ \mathrm{m/s}`$.

### Q8 · NAT · 2 marks

**Answer: 0.1017 m² (range 0.100 to 0.103)**

1. $`\displaystyle \frac{P_{04}}{P_{\mathrm{a}}} = 1.5`$ is below the critical ratio (about 1.92 with losses), so the nozzle is unchoked and $`P_{\mathrm{e}} = P_{\mathrm{a}}`$​$`{} = 100\ \mathrm{kPa}`$.
2. Isentropic exit temperature: $`\displaystyle T_5' = 800 \times \left(\frac{1}{1.5}\right)^{0.25}`$​$`{} = 722.88\ \mathrm{K}`$.
3. Actual drop $`= 0.95 \times 77.12 = 73.26\ \mathrm{K}`$, so $`T_5 = 726.74\ \mathrm{K}`$ and $`C_{\mathrm{j}} = \sqrt{2 \times 1148 \times 73.26}`$​$`{} = 410.1\ \mathrm{m/s}`$.
4. $`\displaystyle \rho_5 = \frac{100{,}000}{287 \times 726.74}`$​$`{} = 0.4794\ \mathrm{kg/m^3}`$.
5. $`\displaystyle A = \frac{\dot m}{\rho_5\,C_{\mathrm{j}}}`$​$`\displaystyle {} = \frac{20}{0.4794 \times 410.1}`$​$`{} = 0.1017\ \mathrm{m^2}`$.

### Q9 · NAT · 2 marks

**Answer: 0.02559 (range 0.0253 to 0.0259)**

1. Energy balance: $`(1 + f) C_{p\mathrm{g}}\,T_{03}`$​$`{} = C_{p\mathrm{a}}\,T_{02} + f\,\eta_{\mathrm{b}}\,Q_{\mathrm{cv}}`$.
2. $`\displaystyle f = \frac{1.148 \times 1500 - 1.005 \times 700}{0.97 \times 42{,}800 - 1.148 \times 1500}`$​$`\displaystyle {} = \frac{1722 - 703.5}{41{,}516 - 1722}`$.
3. $`\displaystyle f = \frac{1018.5}{39{,}794}`$​$`{} = 0.0256`$.

### Q10 · NAT · 2 marks

**Answer: 91.52 kPa (range 90.7 to 92.3)**

1. Free-stream: $`P_{0\mathrm{a}} = 20 \times {}`$​$`(1 + 0.2 \times 3.24)^{3.5}`$​$`{} = 20 \times 5.7458`$​$`{} = 114.92\ \mathrm{kPa}`$.
2. Normal shock at $`M = 1.8`$: $`\displaystyle \frac{P_{02}}{P_{01}} = 0.8127`$ (shock tables or the formula).
3. Compressor face: $`P_{01} = 114.92 \times 0.8127 \times {}`$​$`0.98`$​$`{} = 91.5\ \mathrm{kPa}`$.

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

$`\displaystyle \dot m_{\mathrm{h}} = \frac{\dot m}{\beta + 1}`$​$`\displaystyle {} = \frac{450}{9}`$​$`{} = 50\ \mathrm{kg/s}`$, and the bypass stream carries the other 400 kg/s.

### Q2 · NAT · 1 mark

**Answer: 11.43 kN (range 11.3 to 11.6)**

Thrust power $`= \eta_{\mathrm{pr}} \times`$ shaft power $`= 0.80 \times 2000 = 1600\ \mathrm{kW}`$. Thrust $`\displaystyle = \frac{1{,}600{,}000}{140} = 11{,}429\ \mathrm{N}`$​$`{} = 11.43\ \mathrm{kN}`$.

### Q3 · MCQ · 1 mark

**Answer: (A)**

A ramjet relies entirely on ram compression in its diffuser. At zero speed there is no pressure rise, so burning fuel cannot create a pressure difference to drive a jet. Fuel burns perfectly well (B is false), and nozzle choking (C, D) is irrelevant without a pressure ratio.

### Q4 · NAT · 1 mark

**Answer: 7221 km (range 7148 to 7294)**

$`\displaystyle \mathrm{TSFC} = \frac{0.06}{3600}`$​$`{} = 1.667 \times 10^{-5}\ \mathrm{kg/(N{\cdot}s)}`$, so $`g\,\mathrm{TSFC} = 1.635 \times 10^{-4}\ \mathrm{s^{-1}}`$. $`\displaystyle R = \left(\frac{250}{1.635 \times 10^{-4}}\right) \times {}`$​$`18 \times \ln 1.3`$​$`{} = 1{,}529{,}052 \times 18 \times 0.2624`$​$`{} = 7{,}221{,}035\ \mathrm{m}`$, about 7,221 km.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (C)**

The same core energy now accelerates more air to a lower mean jet speed. That raises propulsive efficiency (A) and cuts TSFC (C), but each kilogram of air gives less thrust, so specific thrust falls (B). Jet velocity falls, not rises, so (D) is false.

### Q6 · NAT · 2 marks

**Answer: 608.8 m/s (range 602 to 615)**

1. Compressor: $`\Delta T_{\mathrm{c}} = 288 \times {}`$​$`\displaystyle \frac{6^{0.2857} - 1}{0.85}`$​$`\displaystyle {} = \frac{288 \times 0.6685}{0.85}`$​$`{} = 226.5\ \mathrm{K}`$.
2. Work balance: $`\Delta T_{\mathrm{t}} = 1.005 \times {}`$​$`\displaystyle \frac{226.5}{0.99 \times 1.148}`$​$`{} = 200.3\ \mathrm{K}`$, so $`T_{04} = 1150 - 200.3`$​$`{} = 949.7\ \mathrm{K}`$.
3. Nozzle: isentropic drop $`= 949.7 \times {}`$​$`\displaystyle \left[1 - \left(\frac{1}{2.2}\right)^{0.25}\right]`$​$`{} = 949.7 \times 0.1789`$​$`{} = 169.9\ \mathrm{K}`$; actual drop $`= 0.95 \times 169.9 = 161.4\ \mathrm{K}`$.
4. $`C_{\mathrm{j}} = \sqrt{2 \times 1148 \times 161.4}`$​$`{} = 608.8\ \mathrm{m/s}`$.

### Q7 · NAT · 2 marks

**Answer: 41.52 kN (range 41.1 to 41.9)**

1. $`\displaystyle \dot m_{\mathrm{h}} = \frac{350}{7}`$​$`{} = 50\ \mathrm{kg/s}`$ and $`\dot m_{\mathrm{c}} = 300\ \mathrm{kg/s}`$.
2. Cold stream: $`300 \times (330 - 240)`$​$`{} = 27{,}000\ \mathrm{N}`$.
3. Hot stream: $`50 \times (1.02 \times 520 - 240)`$​$`{} = 50 \times 290.4`$​$`{} = 14{,}520\ \mathrm{N}`$.
4. $`F = 27{,}000 + 14{,}520`$​$`{} = 41{,}520\ \mathrm{N}`$​$`{} = 41.52\ \mathrm{kN}`$.

Fuel flow $`= 0.02 \times 50 = 1.0\ \mathrm{kg/s}`$, so $`\displaystyle \mathrm{TSFC} = \frac{3600}{41{,}520}`$​$`{} = 0.0867\ \mathrm{kg/(N{\cdot}h)}`$.

### Q8 · NAT · 2 marks

**Answer: 674.1 N·s/kg (range 667 to 681)**

1. $`C_{\mathrm{i}} = 2.5 \times {}`$​$`\sqrt{1.4 \times 287 \times 220}`$​$`{} = 743.3\ \mathrm{m/s}`$.
2. $`T_{0\mathrm{a}} = 220 \times {}`$​$`(1 + 0.2 \times 6.25)`$​$`{} = 495\ \mathrm{K}`$.
3. Ideal ramjet: $`\displaystyle \frac{C_{\mathrm{j}}}{C_{\mathrm{i}}} = \sqrt{\frac{T_{04}}{T_{0\mathrm{a}}}}`$​$`\displaystyle {} = \sqrt{\frac{1800}{495}}`$​$`{} = 1.9069`$.
4. $`\displaystyle \frac{F}{\dot m} = C_{\mathrm{i}} \left(\frac{C_{\mathrm{j}}}{C_{\mathrm{i}}} - 1\right)`$​$`{} = 743.3 \times 0.9069`$​$`{} = 674.1\ \mathrm{N{\cdot}s/kg}`$.

Propulsive efficiency $`\displaystyle = \frac{2}{1 + 1.9069} = 0.688`$.

### Q9 · NAT · 2 marks

**Answer: 0.03081 (range 0.0304 to 0.0312)**

1. Energy balance on 1 kg of entering gas: $`(1 + f_{\mathrm{ab}})\,C_{p\mathrm{g}}\,T_{06}`$​$`{} = C_{p\mathrm{g}}\,T_{05} + f_{\mathrm{ab}}\,\eta_{\mathrm{ab}}\,Q_{\mathrm{cv}}`$.
2. $`\displaystyle f_{\mathrm{ab}} = \frac{C_{p\mathrm{g}} (T_{06} - T_{05})}{\eta_{\mathrm{ab}}\,Q_{\mathrm{cv}} - C_{p\mathrm{g}}\,T_{06}}`$​$`{} = 1.148 \times {}`$​$`\displaystyle \frac{1000}{0.92 \times 43{,}000 - 1.148 \times 2000}`$.
3. $`\displaystyle f_{\mathrm{ab}} = \frac{1148}{39{,}560 - 2296}`$​$`\displaystyle {} = \frac{1148}{37{,}264}`$​$`{} = 0.0308`$.

This is more than the main combustor usually burns, which is why afterburning raises TSFC so sharply.

### Q10 · NAT · 2 marks

**Answer: 0.2567 kg/(kW·h) (range 0.254 to 0.260)**

1. Jet thrust power $`= 2500 \times 160 = 400\ \mathrm{kW}`$.
2. Equivalent shaft power $`\displaystyle = 4000 + \frac{400}{0.82}`$​$`{} = 4487.8\ \mathrm{kW}`$.
3. $`\mathrm{ESFC} = 0.32 \times {}`$​$`\displaystyle \frac{3600}{4487.8}`$​$`{} = 0.2567\ \mathrm{kg/(kW{\cdot}h)}`$.

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

$`\displaystyle U = \frac{\pi D N}{60}`$​$`\displaystyle {} = \frac{\pi \times 0.6 \times 12{,}000}{60}`$​$`{} = 377.0\ \mathrm{m/s}`$.

### Q2 · NAT · 1 mark

**Answer: 143.3 K (range 142 to 145)**

$`\displaystyle \Delta T_0 = \frac{\psi\sigma U_2^{2}}{C_p}`$​$`\displaystyle {} = \frac{1.0 \times 0.9 \times 400^{2}}{1005}`$​$`\displaystyle {} = \frac{144{,}000}{1005}`$​$`{} = 143.3\ \mathrm{K}`$.

### Q3 · MCQ · 1 mark

**Answer: (A)**

A 50% reaction stage has symmetric velocity triangles, so $`\beta_2 = \alpha_1`$​$`{} = 20^\circ`$ and $`\alpha_2 = \beta_1`$​$`{} = 50^\circ`$. Rotor and stator blades are then mirror images.

### Q4 · NAT · 1 mark

**Answer: 11**

$`\displaystyle \frac{250}{24} = 10.42`$, so 11 stages are needed. Ten stages would give only 240 K.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (C)**

In a 50% reaction stage the triangles are symmetric, so nozzle and rotor blades are mirror images (A). An ideal impulse rotor has no static pressure or enthalpy drop (B). Higher $`\psi`$ extracts more work per stage, so fewer stages are needed (C). Negative reaction means the rotor diffuses the relative flow and static pressure rises across it, so (D) is false.

### Q6 · NAT · 2 marks

**Answer: 1.383 (range 1.37 to 1.40)**

1. $`\tan 58^\circ - \tan 42^\circ = 1.6003 - {}`$​$`0.9004`$​$`{} = 0.6999`$.
2. $`W = \Omega U\,C_{\mathrm{a}} (\tan\beta_1 - \tan\beta_2)`$​$`{} = 0.95 \times 300 \times 165 \times {}`$​$`0.6999`$​$`{} = 32{,}914\ \mathrm{J/kg}`$.
3. $`\displaystyle (\Delta T_0)_{\mathrm{stage}} = \frac{32{,}914}{1005}`$​$`{} = 32.75\ \mathrm{K}`$.
4. $`\displaystyle \pi_{\mathrm{cs}} = \left(1 + \frac{0.89 \times 32.75}{300}\right)^{3.5}`$​$`{} = 1.09716^{3.5}`$​$`{} = 1.3834`$.

### Q7 · NAT · 2 marks

**Answer: 0.5837 (range 0.578 to 0.589)**

1. $`\displaystyle \tan\beta_1 = \frac{U}{C_{\mathrm{a}}} - \tan\alpha_1`$​$`{} = 1.8824 - 0.4663`$​$`{} = 1.4160\quad (\beta_1 = 54.8^\circ)`$.
2. $`\displaystyle \phi = \frac{C_{\mathrm{a}}}{U}`$​$`{} = 0.5312`$.
3. $`\displaystyle R = \left(\frac{\phi}{2}\right) (\tan\beta_1 + \tan\beta_2)`$​$`{} = 0.2656 \times {}`$​$`(1.4160 + 0.7813)`$​$`{} = 0.584`$.

Prewhirl in the direction of rotation lowers the relative inlet velocity, which keeps the rotor tip relative Mach number down.

### Q8 · NAT · 2 marks

**Answer: 5.064 (range 5.02 to 5.11)**

1. Slip factor: $`\displaystyle \sigma = 1 - \frac{0.63 \pi}{20}`$​$`{} = 0.9010`$.
2. Tip speed: $`\displaystyle U_2 = \frac{\pi \times 0.45 \times 20{,}000}{60}`$​$`{} = 471.2\ \mathrm{m/s}`$.
3. $`\displaystyle \Delta T_0 = \frac{\psi\sigma U_2^{2}}{C_p}`$​$`{} = 1.04 \times 0.9010 \times {}`$​$`\displaystyle \frac{471.2^{2}}{1005}`$​$`{} = 207.1\ \mathrm{K}`$.
4. $`\displaystyle \pi_{\mathrm{c}} = \left(1 + \frac{0.82 \times 207.1}{288}\right)^{3.5}`$​$`{} = 1.5895^{3.5}`$​$`{} = 5.06`$.

### Q9 · NAT · 2 marks

**Answer: 0.4112 (range 0.407 to 0.416)**

1. $`\displaystyle \frac{U}{C_{\mathrm{a}}} = \frac{340}{240}`$​$`{} = 1.4167`$, so $`\phi = 0.7059`$.
2. $`\displaystyle \tan\beta_2 = \tan\alpha_2 - \frac{U}{C_{\mathrm{a}}}`$​$`{} = 1.8807 - 1.4167`$​$`{} = 0.4641`$.
3. $`\displaystyle \tan\beta_3 = \tan\alpha_3 + \frac{U}{C_{\mathrm{a}}}`$​$`{} = 0.2126 + 1.4167`$​$`{} = 1.6292`$.
4. $`\displaystyle R = \left(\frac{\phi}{2}\right) (\tan\beta_3 - \tan\beta_2)`$​$`{} = 0.3529 \times 1.1652`$​$`{} = 0.411`$.

The stage work is $`U\,C_{\mathrm{a}} (\tan\alpha_2 + \tan\alpha_3)`$​$`{} = 170{,}812\ \mathrm{J/kg}`$, a temperature drop of 148.8 K with $`C_{p\mathrm{g}} = 1148\ \mathrm{J/kg{\cdot}K}`$.

### Q10 · NAT · 2 marks

**Answer: 12.65 (range 12.5 to 12.8)**

1. Flow compatibility: $`\displaystyle \frac{\dot m \sqrt{T_{01}}}{P_{01}}`$​$`\displaystyle {} = \left(\frac{\dot m \sqrt{T_{03}}}{P_{03}}\right) \times {}`$​$`\displaystyle \left(\frac{P_{03}}{P_{02}}\right) \times \left(\frac{P_{02}}{P_{01}}\right) \times {}`$​$`\displaystyle \sqrt{\frac{T_{01}}{T_{03}}}`$.
2. The turbine flow function and $`\displaystyle \frac{P_{03}}{P_{02}}`$ are fixed, so at fixed compressor flow, $`\pi_{\mathrm{c}}`$ is proportional to $`\displaystyle \sqrt{\frac{T_{03}}{T_{01}}}`$.
3. $`\displaystyle \pi_{\mathrm{c}} = 12 \times \sqrt{\frac{5.0}{4.5}}`$​$`{} = 12 \times 1.0541`$​$`{} = 12.65`$.

Raising $`T_{03}`$ pushes the operating point up the constant-flow line toward the surge line.

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

$`\displaystyle I_{\mathrm{sp}} = \frac{F}{\dot m\,g_0}`$​$`\displaystyle {} = \frac{500{,}000}{170 \times 9.81}`$​$`{} = 299.8\ \mathrm{s}`$. The effective exhaust velocity is $`\displaystyle \frac{500{,}000}{170} = 2941\ \mathrm{m/s}`$.

### Q2 · NAT · 1 mark

**Answer: 3779.5 m/s (range 3760 to 3799)**

$`\displaystyle \Delta V = g_0\,I_{\mathrm{sp}}\,\ln \left(\frac{m_0}{m_{\mathrm{f}}}\right)`$​$`\displaystyle {} = 9.81 \times 320 \times \ln \left(\frac{50}{15}\right)`$​$`{} = 3139.2 \times 1.2040`$​$`{} = 3780\ \mathrm{m/s}`$.

### Q3 · MCQ · 1 mark

**Answer: (A)**

Extending the nozzle adds momentum thrust but makes the pressure term $`(P_{\mathrm{e}} - P_{\mathrm{a}}) A_{\mathrm{e}}`$ more negative once $`P_{\mathrm{e}}`$ drops below $`P_{\mathrm{a}}`$. The two effects balance exactly at $`P_{\mathrm{e}} = P_{\mathrm{a}}`$, the optimum expansion condition. Under-expansion (B) wastes available expansion; over-expansion (C) adds negative pressure thrust.

### Q4 · NAT · 1 mark

**Answer: 30 kg/s**

$`\displaystyle \dot m_{\mathrm{fuel}} = \frac{\dot m}{1 + \mathrm{O/F}}`$​$`\displaystyle {} = \frac{210}{7}`$​$`{} = 30\ \mathrm{kg/s}`$, and the oxygen flow is 180 kg/s.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Once lit, a solid motor burns its whole grain, so throttling and shutdown are hard (A). Good liquid bipropellants beat solid propellants on $`I_{\mathrm{sp}}`$ (B). A burn-rate pressure exponent n must be below 1 for a stable chamber pressure, so (C) is wrong. A hybrid burns a solid fuel grain with a liquid or gaseous oxidiser (D).

### Q6 · NAT · 2 marks

**Answer: 330.3 s (range 328 to 333)**

1. Momentum thrust $`= 200 \times 3000 = 600{,}000\ \mathrm{N}`$.
2. Pressure thrust $`= (60 - 20) \times 10^{3} \times 1.2`$​$`{} = 48{,}000\ \mathrm{N}`$.
3. $`F = 648{,}000\ \mathrm{N}`$, so $`\displaystyle I_{\mathrm{sp}} = \frac{648{,}000}{200 \times 9.81}`$​$`{} = 330.3\ \mathrm{s}`$.

At sea level (101.3 kPa) the pressure term would be −49,560 N, giving $`I_{\mathrm{sp}} = 280.5\ \mathrm{s}`$. $`I_{\mathrm{sp}}`$ rises with altitude.

### Q7 · NAT · 2 marks

**Answer: 147.1 kg/s (range 146 to 148)**

1. Throat area: $`\displaystyle A_{\mathrm{t}} = \frac{F}{C_{\mathrm{F}}\,P_{\mathrm{c}}}`$​$`\displaystyle {} = \frac{400{,}000}{1.70 \times 6 \times 10^{6}}`$​$`{} = 0.03922\ \mathrm{m^2}`$.
2. Mass flow: $`\displaystyle \dot m = \frac{P_{\mathrm{c}}\,A_{\mathrm{t}}}{c^{*}}`$​$`\displaystyle {} = \frac{6 \times 10^{6} \times 0.03922}{1600}`$​$`{} = 147.1\ \mathrm{kg/s}`$.

Shortcut: $`\displaystyle \dot m = \frac{F}{c^{*}\,C_{\mathrm{F}}}`$​$`\displaystyle {} = \frac{400{,}000}{1600 \times 1.70}`$​$`{} = 147.1\ \mathrm{kg/s}`$, and $`\displaystyle I_{\mathrm{sp}} = \frac{1600 \times 1.70}{9.81}`$​$`{} = 277.3\ \mathrm{s}`$.

### Q8 · NAT · 2 marks

**Answer: 2916.7 m/s (range 2893 to 2941)**

1. $`\displaystyle R = \frac{8314}{20}`$​$`{} = 415.7\ \mathrm{J/kg{\cdot}K}`$ and $`\displaystyle \frac{2 \gamma}{\gamma - 1} = 10`$.
2. $`\displaystyle \left(\frac{P_{\mathrm{e}}}{P_{\mathrm{c}}}\right)^{\frac{\gamma - 1}{\gamma}}`$​$`\displaystyle {} = \left(\frac{1}{100}\right)^{0.2}`$​$`{} = 0.3981`$, so the bracket is 0.6019.
3. $`v_{\mathrm{e}} = \sqrt{10 \times 415.7 \times 3400 \times 0.6019}`$​$`{} = \sqrt{8{,}507{,}033}`$​$`{} = 2917\ \mathrm{m/s}`$.

With $`P_{\mathrm{e}} = P_{\mathrm{a}}`$ this gives $`\displaystyle I_{\mathrm{sp}} = \frac{2917}{9.81}`$​$`{} = 297\ \mathrm{s}`$.

### Q9 · NAT · 2 marks

**Answer: 8841.6 m/s (range 8770 to 8913)**

1. Stage mass ratio $`\displaystyle n = \frac{1 + \lambda}{\varepsilon + \lambda}`$​$`\displaystyle {} = \frac{1.15}{0.23}`$​$`{} = 5.0`$.
2. Each stage gives $`g_0\,I_{\mathrm{sp}}\,\ln n`$​$`{} = 9.81 \times 280 \times \ln 5`$​$`{} = 4421\ \mathrm{m/s}`$.
3. Two stages: $`\Delta V = 8842\ \mathrm{m/s}`$.

### Q10 · NAT · 2 marks

**Answer: 4.848 MPa (range 4.80 to 4.89)**

1. Mass balance: $`\displaystyle \rho_{\mathrm{p}}\,A_{\mathrm{b}}\,a\,P_{\mathrm{c}}^{n} = \frac{P_{\mathrm{c}}\,A_{\mathrm{t}}}{c^{*}}`$, so $`P_{\mathrm{c}}^{1 - n}`$​$`\displaystyle {} = \rho_{\mathrm{p}}\,a\,c^{*}\,\left(\frac{A_{\mathrm{b}}}{A_{\mathrm{t}}}\right)`$ in consistent units.
2. With $`a = 5 \times 10^{-3}\ \mathrm{m/s}`$ per MPa^0.35 and $`P_{\mathrm{c}}`$ in MPa: $`\displaystyle P_{\mathrm{c}}^{0.65} = \frac{1800 \times 5 \times 10^{-3} \times 1550 \times 200}{10^{6}}`$​$`{} = 2.790`$.
3. $`\displaystyle P_{\mathrm{c}} = 2.790^{\frac{1}{0.65}}`$​$`{} = 4.85\ \mathrm{MPa}`$, and the burn rate is $`5 \times 4.85^{0.35} = 8.69\ \mathrm{mm/s}`$.

Sensitivity: a 10% rise in $`\displaystyle \frac{A_{\mathrm{b}}}{A_{\mathrm{t}}}`$ raises $`P_{\mathrm{c}}`$ by $`\displaystyle 1.1^{\frac{1}{0.65}} - 1 = 15.8\%`$, which is why grain cracks are dangerous.

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

With $`C_{\mathrm{i}} = 0`$ there is no ram drag: $`F = \dot m_{\mathrm{a}} (1 + f) C_{\mathrm{j}}`$​$`{} = 25 \times 1.02 \times 580`$​$`{} = 14{,}790\ \mathrm{N}`$​$`{} = 14.79\ \mathrm{kN}`$.

### Q2 · MCQ · 1 mark

**Answer: (C)**

Impulse blading has $`\beta_2 = \beta_3`$, so $`W_{\mathrm{t}2} = W_{\mathrm{t}3}`$. Axial exit gives $`W_{\mathrm{t}3} = U`$, while $`W_{\mathrm{t}2} = C_{\mathrm{t}2} - U`$, so $`C_{\mathrm{t}2} = 2 U`$. The work is $`U (C_{\mathrm{t}2} + C_{\mathrm{t}3}) = 2 U^{2}`$, giving $`\psi = 2`$. A 50% reaction stage with axial exit gives $`\psi = 1`$.

### Q3 · NAT · 1 mark

**Answer: 0.7222 (range 0.717 to 0.727)**

$`\displaystyle \varepsilon = \frac{T_{\mathrm{g}} - T_{\mathrm{b}}}{T_{\mathrm{g}} - T_{\mathrm{c}}}`$​$`\displaystyle {} = \frac{1800 - 1150}{1800 - 900}`$​$`\displaystyle {} = \frac{650}{900}`$​$`{} = 0.722`$.

### Q4 · NAT · 1 mark

**Answer: 0.05828 (range 0.0579 to 0.0587)**

$`\mathrm{CH_{4}} + 2 (\mathrm{O_{2}} + 3.76 \mathrm{N_{2}})`$​$`{} \to \mathrm{CO_{2}} + 2 \mathrm{H_{2}O} + 7.52 \mathrm{N_{2}}`$. Air mass $`= 2 \times 137.28 = 274.56\ \mathrm{g}`$ per 16 g of fuel, so $`\displaystyle f_{\mathrm{st}} = \frac{16}{274.56}`$​$`{} = 0.0583`$. The $`\mathrm{C}_n\mathrm{H}_{2n+2}`$ formula with $`n = 1`$ gives $`\displaystyle \frac{8}{34.32 \times 4}`$, the same value.

### Q5 · NAT · 1 mark

**Answer: 11757.6 rpm (range 11722 to 11793)**

$`\displaystyle \frac{N}{\sqrt{T_{01}}}`$ is held fixed, so $`N_{\mathrm{corr}} = 12{,}000 \times {}`$​$`\displaystyle \sqrt{\frac{288}{300}}`$​$`{} = 12{,}000 \times 0.97980`$​$`{} = 11{,}758\ \mathrm{rpm}`$.

### Q6 · MSQ · 1 mark

**Answer: (A), (C), (D)**

An air-breathing engine takes its oxidiser from the air, so its $`I_{\mathrm{sp}}`$ based on fuel flow (thousands of seconds) far exceeds a rocket's (A). A rocket's thrust does not depend on flight speed, so (B) is false. At subsonic speeds a ramjet has little ram compression, so its TSFC is far worse than a turbojet's (C). At the same thrust and flight speed a turbofan's lower jet speed gives a higher $`\eta_{\mathrm{p}}`$ (D).

### Q7 · NAT · 2 marks

**Answer: 597.4 N·s/kg (range 590 to 605)**

1. Compressor: $`\Delta T_{\mathrm{c}} = 288 \times {}`$​$`\displaystyle \frac{5^{0.2857} - 1}{0.85}`$​$`{} = 197.8\ \mathrm{K}`$, so $`T_{02} = 485.8\ \mathrm{K}`$; $`P_{02} = 506.5\ \mathrm{kPa}`$ and $`P_{03} = 0.96 \times 506.5`$​$`{} = 486.2\ \mathrm{kPa}`$.
2. Turbine: $`\Delta T_{\mathrm{t}} = 1.005 \times {}`$​$`\displaystyle \frac{197.8}{0.99 \times 1.148}`$​$`{} = 174.9\ \mathrm{K}`$, so $`T_{04} = 925.1\ \mathrm{K}`$. $`\displaystyle T_{04}' = 1100 - \frac{174.9}{0.88}`$​$`{} = 901.2\ \mathrm{K}`$, so $`\displaystyle \frac{P_{03}}{P_{04}} = \left(\frac{1100}{901.2}\right)^{4}`$​$`{} = 2.2194`$ and $`P_{04} = 219.1\ \mathrm{kPa}`$.
3. Nozzle: $`\displaystyle \frac{P_{04}}{P_{\mathrm{a}}} = 2.163`$, above the critical 1.919, so it is choked. $`\displaystyle T_{\mathrm{c}} = \frac{925.1 \times 6}{7}`$​$`{} = 792.9\ \mathrm{K}`$, $`C_{\mathrm{j}} = \sqrt{1.333 \times 287 \times 792.9}`$​$`{} = 550.8\ \mathrm{m/s}`$, $`\displaystyle P_{\mathrm{c}} = \frac{219.1}{1.919}`$​$`{} = 114.2\ \mathrm{kPa}`$.
4. $`\displaystyle \frac{A}{\dot m} = \frac{R T_{\mathrm{c}}}{P_{\mathrm{c}}\,C_{\mathrm{j}}}`$​$`\displaystyle {} = \frac{287 \times 792.9}{114{,}162 \times 550.8}`$​$`{} = 0.003619\ \mathrm{m^2{\cdot}s/kg}`$.
5. $`\displaystyle F_{\mathrm{s}} = C_{\mathrm{j}} + \frac{(P_{\mathrm{c}} - P_{\mathrm{a}})\,A}{\dot m}`$​$`{} = 550.8 + 12{,}862 \times {}`$​$`0.003619`$​$`{} = 550.8 + 46.5`$​$`{} = 597.4\ \mathrm{N{\cdot}s/kg}`$.

### Q8 · NAT · 2 marks

**Answer: 13**

1. With polytropic efficiency: $`\displaystyle \frac{T_{02}}{T_{01}} = 12^{\frac{0.2857}{0.90}}`$​$`{} = 12^{0.3175}`$​$`{} = 2.2009`$.
2. Overall $`\Delta T_0 = 288 \times 1.2009`$​$`{} = 345.9\ \mathrm{K}`$.
3. Stages $`\displaystyle = \frac{345.9}{28} = 12.35`$, so 13 stages are needed.

### Q9 · NAT · 2 marks

**Answer: 787.9 kW (range 781 to 795)**

1. Tip speed: $`\displaystyle U_2 = \frac{\pi \times 0.40 \times 22{,}000}{60}`$​$`{} = 460.8\ \mathrm{m/s}`$.
2. Slip factor: $`\displaystyle \sigma = 1 - \frac{0.63 \pi}{17}`$​$`{} = 0.8836`$.
3. Power $`= \dot m\,\psi\,\sigma\,U_2^{2}`$​$`{} = 4 \times 1.05 \times 0.8836 \times {}`$​$`460.8^{2}`$​$`{} = 787{,}872\ \mathrm{W}`$​$`{} = 787.9\ \mathrm{kW}`$.

### Q10 · NAT · 2 marks

**Answer: 61.7° (range 61.3 to 62.1)**

1. $`\psi = \phi (\tan\beta_2 + \tan\beta_3)`$ gives $`\displaystyle \tan\beta_2 + \tan\beta_3 = \frac{1.6}{0.7}`$​$`{} = 2.2857`$.
2. $`\displaystyle R = \left(\frac{\phi}{2}\right) (\tan\beta_3 - \tan\beta_2)`$​$`{} = 0.5`$ gives $`\displaystyle \tan\beta_3 - \tan\beta_2 = \frac{1}{0.7}`$​$`{} = 1.4286`$.
3. So $`\tan\beta_3 = 1.8571\quad (\beta_3 = 61.7^\circ)`$ and $`\tan\beta_2 = 0.4286\quad (\beta_2 = 23.2^\circ)`$.
4. For 50% reaction the triangles are symmetric, so $`\alpha_2 = \beta_3`$​$`{} = 61.7^\circ`$ and $`\alpha_3 = \beta_2`$​$`{} = 23.2^\circ`$.

### Q11 · NAT · 2 marks

**Answer: 1.555 (range 1.54 to 1.57)**

For optimum expansion the pressure term vanishes and $`\displaystyle C_{\mathrm{F}} = \sqrt{\left(\frac{2 \gamma^{2}}{\gamma - 1}\right)\,\left(\frac{2}{\gamma + 1}\right)^{\frac{\gamma + 1}{\gamma - 1}}\,\left[1 - \left(\frac{P_{\mathrm{e}}}{P_{\mathrm{c}}}\right)^{\frac{\gamma - 1}{\gamma}}\right]}`$.

1. $`\displaystyle \frac{2 \gamma^{2}}{\gamma - 1}`$​$`\displaystyle {} = \frac{2 \times 1.44}{0.2}`$​$`{} = 14.40`$.
2. $`\displaystyle \left(\frac{2}{2.2}\right)^{\frac{2.2}{0.2}}`$​$`{} = 0.9091^{11}`$​$`{} = 0.3505`$.
3. $`\displaystyle 1 - \left(\frac{1}{50}\right)^{\frac{0.2}{1.2}}`$​$`{} = 1 - 0.5210`$​$`{} = 0.4790`$.
4. $`C_{\mathrm{F}} = \sqrt{14.40 \times 0.3505 \times 0.4790}`$​$`{} = \sqrt{2.4176}`$​$`{} = 1.555`$.

Combined with $`c^{*}`$ this gives the effective exhaust velocity: $`c = c^{*}\,C_{\mathrm{F}}`$.

### Q12 · NAT · 2 marks

**Answer: 7826.9 km (range 7748 to 7906)**

1. Since $`\displaystyle \eta_{\mathrm{ov}} = \frac{F\,V}{\dot m_{\mathrm{f}}\,Q_{\mathrm{cv}}}`$ and $`F = D`$ in cruise, $`\displaystyle \frac{V}{g\,\mathrm{TSFC}} = \frac{\eta_{\mathrm{ov}}\,Q_{\mathrm{cv}}}{g}`$, so $`\displaystyle R = \eta_{\mathrm{ov}}\,\left(\frac{Q_{\mathrm{cv}}}{g}\right)\,\left(\frac{L}{D}\right)\,\ln \left(\frac{W_{\mathrm{i}}}{W_{\mathrm{f}}}\right)`$.
2. $`\displaystyle \frac{Q_{\mathrm{cv}}}{g} = \frac{43 \times 10^{6}}{9.81}`$​$`{} = 4{,}383{,}282\ \mathrm{m}`$.
3. $`R = 0.35 \times 4{,}383{,}282 \times {}`$​$`17 \times \ln 1.35`$​$`{} = 0.35 \times 4{,}383{,}282 \times 17 \times {}`$​$`0.3001`$​$`{} = 7{,}826{,}887\ \mathrm{m}`$, about 7,827 km.

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

No heat or work crosses the nozzle, so $`h_0`$, and with it $`T_0`$, stays constant. Friction lowers $`P_0`$ and raises entropy, and static temperature falls as the gas speeds up.

### Q2 · MCQ · 1 mark

**Answer: (A)**

$`\displaystyle \eta = 1 - \frac{1}{r^{\frac{\gamma - 1}{\gamma}}}`$ contains no temperature. Turbine inlet temperature changes the specific work, not the ideal efficiency.

### Q3 · MCQ · 1 mark

**Answer: (B)**

Maximum work occurs at $`\displaystyle c = \sqrt{\frac{T_3}{T_1}}`$, which makes $`T_2 = T_4`$​$`{} = \sqrt{T_1\,T_3}`$. Pushing the pressure ratio to its maximum $`(T_2 = T_3)`$ drives the work to zero.

### Q4 · NAT · 1 mark

**Answer: 1.667 (range 1.66 to 1.67)**

$`\displaystyle \gamma = 1 + \frac{2}{f}`$​$`\displaystyle {} = 1 + \frac{2}{3}`$​$`\displaystyle {} = \frac{5}{3}`$​$`{} = 1.667`$. A diatomic gas with 5 degrees of freedom gives the familiar 1.4.

### Q5 · NAT · 1 mark

**Answer: 0.5 (range 0.490 to 0.510)**

$`\displaystyle \eta_{\mathrm{p}} = \frac{2}{1 + \frac{C_{\mathrm{j}}}{C_{\mathrm{i}}}}`$​$`\displaystyle {} = \frac{2}{1 + 3}`$​$`{} = 0.5`$.

### Q6 · MCQ · 1 mark

**Answer: (B)**

$`\displaystyle \eta_{\mathrm{p}} = \frac{2}{1 + \frac{C_{\mathrm{j}}}{C_{\mathrm{i}}}}`$ equals 1 when $`C_{\mathrm{j}} = C_{\mathrm{i}}`$. But thrust $`\dot m (C_{\mathrm{j}} - C_{\mathrm{i}})`$ is then zero, so no practical engine runs there.

### Q7 · MCQ · 1 mark

**Answer: (D)**

A high-bypass turbofan moves the most air at the lowest jet speed for a given thrust, so its jet speed is closest to the flight speed. A ramjet barely works at Mach 0.8.

### Q8 · MSQ · 1 mark

**Answer: (A), (C), (D)**

TSFC is fuel flow per unit thrust, so lower is better (C), and kg/(N·h) is a common unit (A). Turbofans beat turbojets at subsonic cruise (D). A ramjet has almost no compression at subsonic speed, so its TSFC is the worst, not the best.

### Q9 · MCQ · 1 mark

**Answer: (B)**

The engine must take free-stream air moving at $`C_{\mathrm{i}}`$ and bring it along, which costs momentum $`\dot m_{\mathrm{a}}\,C_{\mathrm{i}}`$. That is the negative term in $`F = (\dot m_{\mathrm{a}} + \dot m_{\mathrm{f}}) C_{\mathrm{j}} - \dot m_{\mathrm{a}}\,C_{\mathrm{i}} + {}`$​$`(P_{\mathrm{e}} - P_{\mathrm{a}}) A_{\mathrm{e}}`$.

### Q10 · MCQ · 1 mark

**Answer: (C)**

Each stage's losses heat the air entering the next stage, which then needs more work. So the overall isentropic efficiency falls below the stage (polytropic) value, and the gap grows with pressure ratio.

### Q11 · MCQ · 1 mark

**Answer: (A)**

With losses, turbine work grows with $`T_3`$ while compressor work stays fixed, so both net work and efficiency rise. Option (C) is true only for the ideal cycle, which is the trap here.

### Q12 · MSQ · 1 mark

**Answer: (A), (C), (D)**

A propeller moves a huge mass of air slowly, so $`\eta_{\mathrm{p}}`$ is high at low speed (A), but its tips go transonic as flight speed rises (D). A turboprop gets most of its thrust from the propeller, not the jet, so (B) is false. A turboshaft drives a rotor or generator (C).

### Q13 · MCQ · 1 mark

**Answer: (D)**

A ramjet has no rotating parts. It slows the incoming air in its diffuser, converting kinetic energy into pressure, which is why it needs forward speed to work.

### Q14 · MCQ · 1 mark

**Answer: (C)**

The turbine extracts just enough work to drive the compressor and accessories. The remaining energy expands in the nozzle to produce thrust.

### Q15 · MSQ · 1 mark

**Answer: (A), (D)**

Thrust scales with mass flow, which falls with density (A, D). Ram drag $`\dot m_{\mathrm{a}}\,C_{\mathrm{i}}`$ actually falls with mass flow. A colder intake raises $`\displaystyle \frac{T_{03}}{T_{01}}`$ and helps the cycle, partly offsetting the loss, so (C) is wrong.

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

The intake is adiabatic with no work, so $`T_0`$ is unchanged. Friction lowers $`P_0`$, while static pressure rises and Mach number falls as the air slows.

### Q2 · MCQ · 1 mark

**Answer: (C)**

From $`\displaystyle \frac{\mathrm{d}A}{A} = \frac{(M^{2} - 1) \mathrm{d}u}{u}`$, subsonic flow $`(M < 1)`$ slows down when the area increases.

### Q3 · MCQ · 1 mark

**Answer: (C)**

With $`M > 1`$, the factor $`(M^{2} - 1)`$ is positive, so $`\mathrm{d}u < 0`$ needs $`\mathrm{d}A < 0`$. A supersonic diffuser therefore converges, the reverse of the subsonic case.

### Q4 · MCQ · 1 mark

**Answer: (B)**

Shock loss rises steeply with the normal Mach number. Several weak shocks compress the air with far less $`P_0`$ loss than one strong normal shock.

### Q5 · MSQ · 1 mark

**Answer: (B), (C)**

Choking fixes $`M = 1`$ at the exit (C) and the flow per unit area at a value set by $`P_{04}`$ and $`T_{04}`$ (B). Exit pressure then exceeds ambient, giving pressure thrust, and downstream changes cannot raise the flow.

### Q6 · MCQ · 1 mark

**Answer: (A)**

Under-expanded means $`P_{\mathrm{e}} > P_{\mathrm{a}}`$, so the jet keeps expanding outside the nozzle through expansion fans. Shocks and separation belong to over-expanded nozzles.

### Q7 · MCQ · 1 mark

**Answer: (D)**

With losses, a larger pressure ratio is needed to reach sonic speed. For $`\displaystyle \gamma = \frac{4}{3}`$ it rises from 1.853 to 1.919 at $`\eta_{\mathrm{nz}} = 0.95`$.

### Q8 · MCQ · 1 mark

**Answer: (C)**

The primary zone burns near stoichiometric to give a stable, fast-burning flame. The overall mixture is much leaner $`(\phi \approx 0.3)`$ once secondary and dilution air are added.

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

Burning extra fuel in the jet pipe raises $`T_0`$, and jet velocity scales with $`\sqrt{T_0}`$ at a given nozzle pressure ratio. Mass flow and $`P_0`$ do not rise; $`P_0`$ actually falls slightly.

### Q13 · MSQ · 1 mark

**Answer: (A), (C), (D)**

The nozzle must open to pass the hotter, less dense gas (C), and flame holders stabilise the flame in the fast jet-pipe flow (D). Heat is added at low pressure, so efficiency falls and TSFC rises sharply.

### Q14 · MCQ · 1 mark

**Answer: (D)**

An annular liner wraps the whole engine, saving length, weight and loss. Cans are easier to develop, and separate flame tubes with crossfire tubes describe can or can-annular designs.

### Q15 · MCQ · 1 mark

**Answer: (B)**

Heat transfer rises with mass flux $`\rho u`$, which peaks at the throat where the area is smallest. That is why throats get the most intense cooling.

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

A stator does no work, so $`h_0`$ is constant. It turns and slows the absolute flow, converting kinetic energy into static pressure.

### Q2 · MCQ · 1 mark

**Answer: (A)**

Equal enthalpy rise in rotor and stator makes the velocity triangles symmetric, so rotor and stator blades are mirror images.

### Q3 · MCQ · 1 mark

**Answer: (D)**

As the annulus boundary layers thicken, mid-span axial velocity rises and the blades there do less work. The average stage work drops, which $`\Omega`$ accounts for.

### Q4 · MCQ · 1 mark

**Answer: (C)**

$`\displaystyle \frac{W_2}{W_1}`$ measures how much the rotor slows the relative flow. Too much deceleration against the adverse pressure gradient separates the boundary layer.

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

The relative eddy in the passage means the air does not leave at the blade angle, so $`C_{\mathrm{t}2} < U_2`$ and $`\displaystyle \sigma = \frac{C_{\mathrm{t}2}}{U_2}`$​$`{} < 1`$. Slip reduces the work the impeller can do.

### Q9 · MCQ · 1 mark

**Answer: (A)**

Extra work is spent on disc friction and windage, so the work input is $`\psi\sigma U_2^{2}`$ with $`\psi`$ slightly above 1, typically 1.03 to 1.05.

### Q10 · MCQ · 1 mark

**Answer: (A)**

$`W = U_2^{2} - U_2\,C_{\mathrm{r}2}\,\cot\beta_2`$ falls with flow for backward vanes, which is stabilising. Radial vanes give constant work and forward vanes a rising, unstable curve.

### Q11 · MCQ · 1 mark

**Answer: (B)**

The rotor does work, so $`h_0`$ changes. Rothalpy is the rotating-frame equivalent that stays constant; for an axial rotor with constant U it reduces to $`\displaystyle h + \frac{W^{2}}{2}`$.

### Q12 · MCQ · 1 mark

**Answer: (B)**

All the expansion happens in the nozzles. The rotor only turns the flow at constant relative speed, so static pressure and enthalpy stay the same across it.

### Q13 · MCQ · 1 mark

**Answer: (C)**

Negative reaction means static enthalpy rises in the rotor, so $`W_3 < W_2`$ and the rotor acts as a diffuser. Designers avoid it because diffusing passages lose more.

### Q14 · MSQ · 1 mark

**Answer: (A), (C), (D)**

Film, impingement and convection cooling keep the metal below the gas temperature, and ceramic thermal barrier coatings insulate it (A, C, D). Hot turbine blades are nickel-based superalloys; aluminium would melt.

### Q15 · MCQ · 1 mark

**Answer: (C)**

$`\displaystyle \frac{\dot m \sqrt{T_{01}}}{P_{01}}`$ is fixed, so $`\dot m`$ is proportional to $`\displaystyle \frac{P_{01}}{\sqrt{T_{01}}}`$. $`P_{01}`$ falls much faster than $`\sqrt{T_{01}}`$ with altitude, so the actual mass flow drops.

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

A rocket takes in no air, so there is no ram drag and $`F = \dot m v_{\mathrm{e}} + (P_{\mathrm{e}} - P_{\mathrm{a}}) A_{\mathrm{e}}`$ does not contain flight speed. Thrust changes with altitude through $`P_{\mathrm{a}}`$, not with speed.

### Q2 · MCQ · 1 mark

**Answer: (A)**

In vacuum $`P_{\mathrm{a}} = 0`$, so the pressure term $`(P_{\mathrm{e}} - P_{\mathrm{a}}) A_{\mathrm{e}}`$ is largest. More thrust for the same propellant flow means higher $`I_{\mathrm{sp}}`$.

### Q3 · MCQ · 1 mark

**Answer: (A)**

$`\displaystyle c^{*} = \frac{P_{\mathrm{c}}\,A_{\mathrm{t}}}{\dot m}`$ depends on $`T_0`$, molar mass and $`\gamma`$ of the combustion products, not on the nozzle's expansion. $`C_{\mathrm{F}}`$ measures the nozzle.

### Q4 · MCQ · 1 mark

**Answer: (C)**

$`\displaystyle C_{\mathrm{F}} = \frac{F}{P_{\mathrm{c}}\,A_{\mathrm{t}}}`$ captures how well the nozzle turns chamber pressure into thrust, so it depends on expansion and back pressure. Chamber temperature enters through $`c^{*}`$, not $`C_{\mathrm{F}}`$.

### Q5 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Dropping empty tanks and engines is the core benefit (B, D), and upper stages can use large-area-ratio nozzles for vacuum (A). Staging does not change an engine's own $`I_{\mathrm{sp}}`$, so (C) is false.

### Q6 · MCQ · 1 mark

**Answer: (C)**

With $`n < 1`$, a pressure rise increases nozzle outflow (proportional to $`P_{\mathrm{c}}`$) faster than gas generation (proportional to $`P_{\mathrm{c}}^{n}`$), so the pressure returns to equilibrium. With $`n > 1`$ it runs away.

### Q7 · MCQ · 1 mark

**Answer: (B)**

High cross-flow velocity in the port thins the boundary layer and raises heat transfer to the propellant, so it burns faster. It matters most early in the burn, when the port is narrow.

### Q8 · MCQ · 1 mark

**Answer: (B)**

Exhaust velocity scales roughly with $`\displaystyle \sqrt{\frac{T_0}{M}}`$. LOX/LH2 exhaust is mostly water and excess hydrogen, with a very low molar mass. Its flame temperature is not unusually high, and its density is very low.

### Q9 · MCQ · 1 mark

**Answer: (A)**

$`\displaystyle \eta_{\mathrm{p}} = \frac{2 \left(\frac{u}{c}\right)}{1 + \left(\frac{u}{c}\right)^{2}}`$ peaks at 1 when $`u = c`$, because the exhaust is then left at rest relative to the ground. Unlike a jet engine, the rocket still has full thrust there.

### Q10 · MSQ · 1 mark

**Answer: (A), (D)**

A shock is adiabatic and does no work, so $`T_0`$ is constant (D), and continuity keeps $`\rho u`$ constant (A). It is irreversible, so $`P_0`$ falls and entropy rises; that is the trap.

### Q11 · MCQ · 1 mark

**Answer: (B)**

An air-breathing engine carries only fuel and takes its oxidiser free from the air, so its thrust per unit of carried propellant is much higher. A rocket must carry its oxidiser too.

### Q12 · MCQ · 1 mark

**Answer: (D)**

Gravity loss is roughly the integral of $`g\,\cos\theta`$ over the burn, so finishing the burn sooner and turning toward horizontal both cut it. This is the impulsive launch idea in your notes.

### Q13 · MCQ · 1 mark

**Answer: (D)**

Flow accelerates to sonic speed at the throat and becomes supersonic in the diverging section. That needs $`M = 1`$ exactly at the minimum area.

### Q14 · MSQ · 1 mark

**Answer: (A), (B), (D)**

Compressors divide ideal by actual work (A); turbines and nozzles divide actual by ideal (B, D). $`\displaystyle \frac{P_{01}}{P_{0\mathrm{a}}}`$ is the pressure recovery factor, not the isentropic efficiency, so (C) is the trap.

### Q15 · MCQ · 1 mark

**Answer: (D)**

Hypergolic pairs such as $`\mathrm{N_{2}O_{4}}`$ with MMH ignite on contact, so they suit spacecraft thrusters that restart many times. They are toxic, storable at room temperature, and have moderate $`I_{\mathrm{sp}}`$.
