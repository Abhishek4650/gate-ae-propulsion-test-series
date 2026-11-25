# GATE AE Propulsion: Solved Examples

Last updated 25 Nov 2026

## How to use this booklet

Each topic below has solved examples of every question type GATE AE asks in propulsion, ordered from basic to advanced. Cover the solution, attempt the question, then check your working step by step.

When a topic feels solid, test yourself with [GATE AE Propulsion Test Series: Question Papers](question-papers.md) or the timed online version at [Propulsion Mock Tests](https://abhishek4650.github.io/gate-ae-propulsion-test-series/).

### GATE question types and marking

| Type | What you do | Marks | Negative marking |
| --- | --- | --- | --- |
| MCQ | Pick the one correct option | 1 or 2 | $`1/3`$ mark (1-mark Q), $`2/3`$ mark (2-mark Q) |
| MSQ | Pick every correct option (one or more) | 1 or 2 | None, but no partial credit |
| NAT | Type a number; accepted within a range | 1 or 2 | None |

### Standard data (unless a question says otherwise)

- Air: $`\gamma = 1.4`$, $`c_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`R = 287\ \mathrm{J/kg{\cdot}K}`$
- Hot combustion gas: $`\gamma_{\mathrm{g}} = 4/3`$, $`c_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$
- $`g_0 = 9.81\ \mathrm{m/s^2}`$
- Component work and heat always use stagnation (total) temperatures, written with subscript 0 ($`T_{01}`$, $`T_{02}`$ …); velocities come from static temperatures.

### Notation (matches your notes)

- $`c_{\mathrm{i}} =`$ flight speed, $`c_{\mathrm{j}} =`$ jet speed, $`f = \dot m_{\mathrm{f}}/\dot m_{\mathrm{a}}`$ (fuel–air ratio), $`B =`$ bypass ratio ($`\beta`$ in your notes)
- Axial machines: $`C_{\mathrm{a}} =`$ axial velocity, $`U =`$ blade speed, $`\alpha =`$ absolute flow angle, $`\beta =`$ relative flow angle, both measured from the axial direction
- $`\phi = C_{\mathrm{a}}/U`$ (flow coefficient), $`\psi = \Delta h_0/U^{2}`$ (blade loading), $`R =`$ degree of reaction, $`\lambda =`$ work-done factor, $`\sigma =`$ slip factor
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

- $`T_0/T = 1 + ((\gamma - 1)/2)\cdot M^{2}`$
- $`P_0/P = (T_0/T)^{\gamma/(\gamma - 1)}`$
- $`c_p = \gamma R/(\gamma - 1)`$ and $`c_v = R/(\gamma - 1)`$
- $`s_2 - s_1 = c_p \cdot \ln(T_2/T_1) -{}`$​$`R \cdot \ln(p_2/p_1)`$
- Adiabatic machine: $`w = h_{01} - h_{02}`$​$`{}= c_p(T_{01} - T_{02})`$

### Example 1.1 · NAT · 1 mark · Stagnation pressure

An aircraft flies at Mach 0.8 where $`T = 223.3\ \mathrm{K}`$ and $`p = 26.5\ \mathrm{kPa}`$. Find the stagnation pressure (kPa) of the oncoming air. Take $`\gamma = 1.4`$.

**Solution.** $`T_0/T = 1 + 0.2 \times 0.8^{2}`$​$`{}= 1.128`$, so $`T_0 = 251.9\ \mathrm{K}`$. $`P_0/P = 1.128^{3.5}`$​$`{}= 1.524`$, so $`P_0 = 26.5 \times 1.524`$​$`{}= 40.4\ \mathrm{kPa}`$.

**Answer: 40.4 kPa (range 40.2 to 40.6)**

### Example 1.2 · MCQ · 1 mark $`\cdot \gamma`$ from degrees of freedom

At high temperature the vibrational modes of a diatomic gas become active, giving it 7 degrees of freedom. Its ratio of specific heats is:

- (A) 1.400
- (B) 1.286
- (C) 1.333
- (D) 1.667

**Solution.** $`\gamma = 1 + 2/f`$​$`{}= 1 + 2/7`$​$`{}= 1.286`$. With $`f = 5`$ (translation and rotation only) you get the familiar 1.4. A monatomic gas $`(f = 3)`$ gives 1.667.

**Answer: (B)**

### Example 1.3 · NAT · 1 mark $`\cdot c_p`$ of hot gas

Combustion gases have $`R = 287\ \mathrm{J/kg{\cdot}K}`$ and $`\gamma = 4/3`$. Find $`c_p`$ in kJ/kg·K.

**Solution.** $`c_p = \gamma R/(\gamma - 1)`$​$`{}= (4/3)(287)/(1/3)`$​$`{}= 4 \times 287`$​$`{}= 1148\ \mathrm{J/kg{\cdot}K}`$. This is where the standard hot-gas value of 1.148 kJ/kg·K comes from.

**Answer: 1.148 kJ/kg·K (range 1.14 to 1.15)**

### Example 1.4 · NAT · 2 marks · Entropy rise in a compressor

Air is compressed adiabatically from 300 K, 100 kPa to 600 K, 800 kPa. Find the specific entropy rise in J/kg·K. Use $`c_p = 1005\ \mathrm{J/kg{\cdot}K}`$ and $`R = 287\ \mathrm{J/kg{\cdot}K}`$.

**Solution.**

$`\Delta s = c_p \cdot \ln(T_2/T_1) - R \cdot {}`$​$`\ln(p_2/p_1)`$​$`{}= 1005 \ln 2 - 287 \ln 8`$​$`{}= 696.6 - 596.8`$​$`{}= 99.8\ \mathrm{J/kg{\cdot}K}`$.

The rise is positive in an adiabatic process, so the compression is irreversible. For comparison, the isentropic exit temperature is $`300 \times 8^{0.2857} = 543.4\ \mathrm{K}`$, giving $`\eta_{\mathrm{c}} = 243.4/300`$​$`{}= 0.811`$.

**Answer: 99.8 J/kg·K (range 98 to 102)**

### Example 1.5 · NAT · 1 mark · Steady-flow work

An adiabatic compressor raises air from $`T_{01} = 288\ \mathrm{K}`$ to $`T_{02} = 520\ \mathrm{K}`$ at 20 kg/s. Find the power input in MW. Take $`c_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$.

**Solution.** With $`q = 0`$, the steady-flow energy equation gives $`w = c_p(T_{02} - T_{01})`$​$`{}= 1.005 \times 232`$​$`{}= 233.2\ \mathrm{kJ/kg}`$. Power $`= 20 \times 233.2 = 4663\ \mathrm{kW}`$. Using stagnation temperatures already accounts for kinetic energy.

**Answer: 4.66 MW (range 4.60 to 4.72)**

### Example 1.6 · MSQ · 1 mark · Insulated duct with friction

Air flows steadily through an insulated duct with wall friction and no work transfer. Which statements are correct?

- (A) Stagnation temperature stays constant
- (B) Stagnation pressure stays constant
- (C) Stagnation pressure falls along the duct
- (D) Specific entropy rises along the duct

**Solution.** With $`q = 0`$ and $`w = 0`$, $`h_0`$ and hence $`T_0`$ stay constant, so (A) holds. Friction is irreversible, so s rises, which is (D). At constant $`T_0`$, $`\Delta s = -R \ln(P_{02}/P_{01})`$​$`{}> 0`$ forces $`P_{02} < P_{01}`$, which is (C).

**Answer: (A), (C), (D)**

## 2. Brayton cycle

The gas turbine cycle is two isentropic processes joined by two constant-pressure ones. Write $`t = T_3/T_1`$ and $`c = r^{(\gamma - 1)/\gamma}`$, where r is the pressure ratio.

- Ideal efficiency: $`\eta = 1 - 1/c`$
- Ideal net work: $`W_{\mathrm{net}}/(c_p\cdot T_1)`$​$`{}= (c - 1)(t/c - 1)`$
- Maximum work when $`c = \sqrt{t}`$, i.e. $`T_2 = T_4`$; then $`W_{\mathrm{max}} = c_p\cdot T_1(\sqrt{t} - 1)^{2}`$
- Perfect heat exchanger: $`\eta = 1 - c/t`$
- Real components: $`\Delta T_{\mathrm{c}} = T_1(c - 1)/\eta_{\mathrm{c}}`$ and $`\Delta T_{\mathrm{t}} = \eta_{\mathrm{t}}\cdot T_3(1 - 1/c)`$
- Polytropic: $`T_{02}/T_{01} = r^{(\gamma - 1)/(\gamma\cdot \eta_{\infty \mathrm{c}})}`$ for compression, $`T_{03}/T_{04} = r^{\eta_{\infty \mathrm{t}}(\gamma - 1)/\gamma}`$ for expansion

### Example 2.1 · NAT · 1 mark · Ideal cycle efficiency

An ideal Brayton cycle uses air $`(\gamma = 1.4)`$ with a pressure ratio of 10. Find the thermal efficiency in percent.

**Solution.** $`c = 10^{0.2857}`$​$`{}= 1.931`$. $`\eta = 1 - 1/1.931`$​$`{}= 0.482`$.

**Answer: 48.2% (range 48.0 to 48.4)**

### Example 2.2 · NAT · 2 marks · Maximum specific work

In an ideal Brayton cycle, $`T_1 = 300\ \mathrm{K}`$ and $`T_3 = 1200\ \mathrm{K}`$. Find the maximum net specific work in kJ/kg. Take $`c_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$ and $`\gamma = 1.4`$.

**Solution.** $`t = 1200/300`$​$`{}= 4`$. Work is maximum when $`c = \sqrt{t}`$​$`{}= 2`$, which makes $`T_2 = T_4`$​$`{}= 600\ \mathrm{K}`$. The pressure ratio is then $`2^{3.5} = 11.3`$. $`W_{\mathrm{max}} = c_p\cdot T_1(\sqrt{t} - 1)^{2}`$​$`{}= 1.005 \times 300 \times 1^{2}`$​$`{}= 301.5\ \mathrm{kJ/kg}`$, and the efficiency there is $`1 - 1/2 = 50\%`$.

**Answer: 301.5 kJ/kg (range 300 to 303)**

### Example 2.3 · NAT · 2 marks · Real cycle with component efficiencies

A gas turbine has $`T_1 = 288\ \mathrm{K}`$, pressure ratio 8, $`\eta_{\mathrm{c}} = 0.85`$, $`T_3 = 1200\ \mathrm{K}`$ and $`\eta_{\mathrm{t}} = 0.88`$. Treat the gas as air throughout ($`c_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`\gamma = 1.4`$) and neglect pressure losses and fuel mass. Find the thermal efficiency in percent.

**Solution.**

1. $`c = 8^{0.2857}`$​$`{}= 1.8114`$.
2. Compressor: $`\Delta T_{\mathrm{c}} = 288 \times 0.8114/0.85`$​$`{}= 274.9\ \mathrm{K}`$, so $`T_2 = 562.9\ \mathrm{K}`$ and $`W_{\mathrm{c}} = 276.3\ \mathrm{kJ/kg}`$.
3. Turbine: $`T_4' = 1200/1.8114`$​$`{}= 662.5\ \mathrm{K}`$, so $`\Delta T_{\mathrm{t}} = 0.88 \times 537.5`$​$`{}= 473.0\ \mathrm{K}`$ and $`W_{\mathrm{t}} = 475.4\ \mathrm{kJ/kg}`$.
4. $`W_{\mathrm{net}} = 475.4 - 276.3`$​$`{}= 199.1\ \mathrm{kJ/kg}`$. Heat added $`= 1.005 \times (1200 - 562.9)`$​$`{}= 640.2\ \mathrm{kJ/kg}`$.
5. $`\eta = 199.1/640.2`$​$`{}= 0.311`$.

The ideal cycle at this pressure ratio gives 44.8%, so component losses cost almost 14 points. The back-work ratio is $`276.3/475.4 = 0.58`$, which is why gas turbines are so sensitive to component efficiency.

**Answer: 31.1% (range 30.6 to 31.6)**

### Example 2.4 · NAT · 1 mark · Polytropic to isentropic efficiency

A compressor with pressure ratio 20 has a polytropic efficiency of 0.90. Find its isentropic efficiency $`(\gamma = 1.4)`$.

**Solution.** Actual temperature ratio $`= 20^{0.2857/0.90}`$​$`{}= 20^{0.3175}`$​$`{}= 2.588`$. Isentropic ratio $`= 20^{0.2857} = 2.354`$. $`\eta_{\mathrm{c}} = (2.354 - 1)/(2.588 - 1)`$​$`{}= 0.852`$.

For a compressor the isentropic efficiency is lower than the polytropic value, and the gap widens as pressure ratio rises. For a turbine the reverse holds.

**Answer: 0.852 (range 0.845 to 0.858)**

### Example 2.5 · MCQ · 1 mark · Heat exchanger

An ideal Brayton cycle with a perfect heat exchanger runs with $`T_1 = 300\ \mathrm{K}`$, $`T_3 = 1200\ \mathrm{K}`$ and pressure ratio $`4\quad (\gamma = 1.4)`$. Its thermal efficiency is closest to:

- (A) 33%
- (B) 48%
- (C) 63%
- (D) 75%

**Solution.** $`c = 4^{0.2857}`$​$`{}= 1.486`$ and $`t = 4`$. With a perfect heat exchanger, $`\eta = 1 - c/t`$​$`{}= 1 - 1.486/4`$​$`{}= 0.628`$. Without it, $`\eta = 1 - 1/1.486`$​$`{}= 0.327`$, which is distractor (A). The exchanger only helps while $`T_4 > T_2`$, that is, while $`c < \sqrt{t}`$.

**Answer: (C)**

### Example 2.6 · MSQ · 2 marks · Brayton cycle statements

For an ideal simple Brayton cycle, which statements are correct?

- (A) Thermal efficiency depends only on pressure ratio and $`\gamma`$
- (B) Net specific work is maximum when compressor exit temperature equals turbine exit temperature
- (C) Adding a heat exchanger raises efficiency at every pressure ratio
- (D) Raising $`T_3`$ at a fixed pressure ratio raises the thermal efficiency

**Solution.** (A) is true because $`\eta = 1 - 1/c`$ contains no temperature. (B) is true because $`c = \sqrt{t}`$ gives $`T_2 = T_4`$. (C) is false: above $`c = \sqrt{t}`$, $`T_4 < T_2`$ and the exchanger would heat the exhaust instead. (D) is false: higher $`T_3`$ raises the specific work, not the ideal efficiency.

**Answer: (A), (B)**

## 3. Thrust, efficiencies, TSFC and range

Thrust comes from the momentum change of the air plus any pressure imbalance at the nozzle exit. Efficiency questions then split the fuel energy into what reaches the jet and what does useful work.

- Thrust: $`F = (\dot m_{\mathrm{a}} + \dot m_{\mathrm{f}})c_{\mathrm{j}} - \dot m_{\mathrm{a}} \cdot c_{\mathrm{i}} +{}`$​$`(p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$
- Specific thrust $`F_{\mathrm{s}} = F/\dot m_{\mathrm{a}}`$; $`\mathrm{TSFC} = \dot m_{\mathrm{f}}/F`$ (multiply by 3600 for kg/(N·h))
- Propulsive efficiency: $`\eta_{\mathrm{p}} = 2/(1 + c_{\mathrm{j}}/c_{\mathrm{i}})`$​$`{}= 2\alpha/(1 + \alpha)`$, with $`\alpha = c_{\mathrm{i}}/c_{\mathrm{j}}`$
- Thermal efficiency: $`\eta_{\mathrm{th}} = \tfrac{1}{2} \dot m_{\mathrm{a}}(c_{\mathrm{j}}^{2} - c_{\mathrm{i}}^{2})/(\dot m_{\mathrm{f}}\cdot Q_{\mathrm{R}})`$; overall $`\eta_0 = \eta_{\mathrm{p}}\cdot \eta_{\mathrm{th}}`$​$`{}= F\cdot c_{\mathrm{i}}/(\dot m_{\mathrm{f}}\cdot Q_{\mathrm{R}})`$
- Breguet range for a jet: $`R = (V/(g\cdot \mathrm{TSFC})) \cdot (L/D) \cdot {}`$​$`\ln(W_{\mathrm{i}}/W_{\mathrm{f}})`$, with TSFC in kg/(N·s)

### Example 3.1 · NAT · 1 mark · Net thrust

A turbojet takes in 50 kg/s of air at a flight speed of 250 m/s. The fuel–air ratio is 0.02 and the fully expanded jet leaves at 600 m/s. Find the net thrust in kN.

**Solution.** $`F = \dot m_{\mathrm{a}}(1 + f)c_{\mathrm{j}} - \dot m_{\mathrm{a}}\cdot c_{\mathrm{i}}`$​$`{}= 50 \times 1.02 \times 600 - 50 \times {}`$​$`250`$​$`{}= 30{,}600 - 12{,}500`$​$`{}= 18{,}100\ \mathrm{N}`$. The term $`\dot m_{\mathrm{a}}\cdot c_{\mathrm{i}}`$ is the ram (intake momentum) drag.

**Answer: 18.1 kN (range 18.0 to 18.2)**

### Example 3.2 · NAT · 2 marks · Thrust with a pressure term

A turbojet flies at 200 m/s with $`\dot m_{\mathrm{a}} = 30\ \mathrm{kg/s}`$ and $`f = 0.02`$. Its nozzle is under-expanded: jet speed 550 m/s, exit area 0.12 m², exit pressure 40 kPa above ambient. Find the total thrust in kN.

**Solution.** Momentum thrust $`= 30 \times 1.02 \times 550 - 30 \times {}`$​$`200`$​$`{}= 16{,}830 - 6{,}000`$​$`{}= 10{,}830\ \mathrm{N}`$. Pressure thrust $`= (p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$​$`{}= 40{,}000 \times 0.12`$​$`{}= 4{,}800\ \mathrm{N}`$. Total $`F = 15{,}630\ \mathrm{N}`$.

**Answer: 15.63 kN (range 15.5 to 15.8)**

### Example 3.3 · NAT · 1 mark · Propulsive efficiency

An engine flies at 270 m/s with a jet velocity of 600 m/s. Neglecting fuel mass and pressure thrust, find the propulsive efficiency.

**Solution.** $`\eta_{\mathrm{p}} = 2c_{\mathrm{i}}/(c_{\mathrm{i}} + c_{\mathrm{j}})`$​$`{}= 540/870`$​$`{}= 0.621`$. Producing the same thrust from more air at a lower jet speed would raise $`\eta_{\mathrm{p}}`$, which is the whole case for turbofans.

**Answer: 0.621 (range 0.615 to 0.627)**

### Example 3.4 · MCQ · 1 mark · Maximum thrust power

For a fixed jet velocity $`c_{\mathrm{j}}`$ and air mass flow, the thrust power $`F\cdot c_{\mathrm{i}}`$ is maximum when the flight speed $`c_{\mathrm{i}}`$ equals:

- (A) $`c_{\mathrm{j}}`$
- (B) $`c_{\mathrm{j}}/2`$
- (C) 0
- (D) $`2c_{\mathrm{j}}`$

**Solution.** Thrust power $`= \dot m_{\mathrm{a}}(c_{\mathrm{j}} - c_{\mathrm{i}})c_{\mathrm{i}}`$. Setting its derivative to zero gives $`c_{\mathrm{i}} = c_{\mathrm{j}}/2`$, where $`\eta_{\mathrm{p}} = 2/(1 + 2)`$​$`{}= 66.7\%`$. At $`c_{\mathrm{i}} = c_{\mathrm{j}}`$ the efficiency is 100% but thrust is zero; at $`c_{\mathrm{i}} = 0`$ thrust is largest but $`\eta_{\mathrm{p}} = 0`$.

**Answer: (B)**

### Example 3.5 · NAT · 2 marks $`\cdot \mathrm{TSFC}`$ and overall efficiency

An engine produces 30 kN at 250 m/s while burning 0.8 kg/s of fuel with a calorific value of 43 MJ/kg. Find the overall efficiency.

**Solution.** $`\mathrm{TSFC} = 0.8/30{,}000`$​$`{}= 2.667 \times 10^{-5}\ \mathrm{kg/(N{\cdot}s)}`$​$`{}= 0.096\ \mathrm{kg/(N{\cdot}h)}`$. $`\eta_0 = F\cdot c_{\mathrm{i}}/(\dot m_{\mathrm{f}}\cdot Q_{\mathrm{R}})`$​$`{}= (30{,}000 \times 250)/(0.8 \times 43 \times 10^{6})`$​$`{}= 7.5 \times 10^{6}/3.44 \times 10^{7}`$​$`{}= 0.218`$.

**Answer: 0.218 (range 0.215 to 0.221)**

### Example 3.6 · NAT · 2 marks · Breguet range

A jet aircraft cruises at 230 m/s with $`L/D = 16`$ and $`\mathrm{TSFC} = 0.07\ \mathrm{kg/(N{\cdot}h)}`$. Its initial-to-final cruise weight ratio is 1.25. Find the range in km.

**Solution.**

1. $`\mathrm{TSFC} = 0.07/3600`$​$`{}= 1.944 \times 10^{-5}\ \mathrm{kg/(N{\cdot}s)}`$, so $`g\cdot \mathrm{TSFC} = 1.9075 \times 10^{-4}\ \mathrm{s^{-1}}`$.
2. $`R = (230/1.9075 \times 10^{-4}) \times {}`$​$`16 \times \ln 1.25`$​$`{}= 1.2058 \times 10^{6} \times 16 \times {}`$​$`0.2231`$.
3. $`R = 4.305 \times 10^{6}\ \mathrm{m}`$.

Range grows with speed, $`L/D`$ and fuel fraction, and falls as TSFC rises.

**Answer: 4305 km (range 4250 to 4360)**

### Example 3.7 · MSQ · 1 mark · Static (take-off) thrust

A turbojet is running on the ground $`(c_{\mathrm{i}} = 0)`$ with a fully expanded jet. Which statements are correct?

- (A) Ram drag is zero
- (B) Propulsive efficiency is zero
- (C) Thrust $`\approx \dot m_{\mathrm{a}}(1 + f)c_{\mathrm{j}}`$
- (D) Thrust power is at its maximum

**Solution.** With $`c_{\mathrm{i}} = 0`$, the ram drag $`\dot m_{\mathrm{a}}\cdot c_{\mathrm{i}}`$ vanishes (A) and the thrust is just the jet momentum (C). Thrust power $`F\cdot c_{\mathrm{i}}`$ and $`\eta_{\mathrm{p}} = 2c_{\mathrm{i}}/(c_{\mathrm{i}} + c_{\mathrm{j}})`$ are both zero, so (B) is true and (D) is false.

**Answer: (A), (B), (C)**

## 4. Intakes and diffusers

An intake slows the air down while losing as little stagnation pressure as possible. The flow is adiabatic, so $`T_0`$ stays constant while $`P_0`$ falls.

- Intake isentropic efficiency: $`\eta_{\mathrm{i}} = (T_{01}' - T_{\mathrm{a}})/(T_{01} - T_{\mathrm{a}})`$, where $`T_{01}'`$ is reached isentropically at the actual $`P_{01}`$
- Pressure rise: $`P_{01}/p_{\mathrm{a}} = [1 + \eta_{\mathrm{i}}\cdot ((\gamma - 1)/2)\cdot M_{\mathrm{a}}^{2}]^{\gamma/(\gamma - 1)}`$
- Ram efficiency: $`\eta_{\mathrm{ram}} = (P_{01} - p_{\mathrm{a}})/(P_{0\mathrm{a}} - p_{\mathrm{a}})`$
- Pressure recovery: $`\pi_{\mathrm{d}} = P_{01}/P_{0\mathrm{a}}`$
- Diffuser efficiency from recovery: $`\eta_{\mathrm{d}} = [\pi_{\mathrm{d}}^{(\gamma - 1)/\gamma}\cdot (1 + ((\gamma - 1)/2)M^{2}) - 1]/[((\gamma - 1)/2)M^{2}]`$
- Normal shock: $`P_{02}/P_{01} = [(\gamma + 1)M^{2}/((\gamma - 1)M^{2} + 2)]^{\gamma/(\gamma - 1)} \cdot {}`$​$`[(\gamma + 1)/(2\gamma M^{2} - (\gamma - 1))]^{1/(\gamma - 1)}`$

### Example 4.1 · NAT · 1 mark · Pressure at the compressor face

An aircraft flies at Mach 0.8 where $`T_{\mathrm{a}} = 223.3\ \mathrm{K}`$ and $`p_{\mathrm{a}} = 26.5\ \mathrm{kPa}`$. The intake isentropic efficiency is $`0.93\quad (\gamma = 1.4)`$. Find the stagnation pressure at the compressor face in kPa.

**Solution.** $`P_{01}/p_{\mathrm{a}} = (1 + 0.93 \times 0.2 \times 0.64)^{3.5}`$​$`{}= 1.1190^{3.5}`$​$`{}= 1.4824`$, so $`P_{01} = 26.5 \times 1.4824`$​$`{}= 39.28\ \mathrm{kPa}`$. A loss-free intake would deliver the free-stream $`P_{0\mathrm{a}} = 40.40\ \mathrm{kPa}`$ from Example 1.1, so this intake loses about 2.8%. $`T_{01}`$ stays at 251.9 K whatever the losses.

**Answer: 39.3 kPa (range 39.1 to 39.5)**

### Example 4.2 · NAT · 1 mark · Ram efficiency

At Mach 0.85 and $`p_{\mathrm{a}} = 30\ \mathrm{kPa}`$, the measured stagnation pressure at the compressor face is 46 kPa. Find the ram efficiency $`(\gamma = 1.4)`$.

**Solution.** $`P_{0\mathrm{a}} = 30 \times {}`$​$`(1 + 0.2 \times 0.7225)^{3.5}`$​$`{}= 30 \times 1.1445^{3.5}`$​$`{}= 48.11\ \mathrm{kPa}`$. $`\eta_{\mathrm{ram}} = (46 - 30)/(48.11 - 30)`$​$`{}= 16/18.11`$​$`{}= 0.883`$.

**Answer: 0.883 (range 0.878 to 0.888)**

### Example 4.3 · NAT · 2 marks · Diffuser efficiency from pressure recovery

A subsonic diffuser receives air at Mach 0.85 and has a stagnation pressure recovery $`\pi_{\mathrm{d}} = 0.95`$. Find the diffuser isentropic efficiency $`(\gamma = 1.4)`$.

**Solution.**

1. $`((\gamma - 1)/2)M^{2}`$​$`{}= 0.2 \times 0.7225`$​$`{}= 0.1445`$.
2. $`\pi_{\mathrm{d}}^{0.2857} = 0.95^{0.2857}`$​$`{}= 0.98545`$.
3. $`\eta_{\mathrm{d}} = (0.98545 \times 1.1445 - 1)/0.1445`$​$`{}= 0.12785/0.1445`$​$`{}= 0.885`$.

A small $`P_0`$ loss shows up as a large efficiency drop at low Mach numbers, because the available temperature rise is small.

**Answer: 0.885 (range 0.880 to 0.890)**

### Example 4.4 · NAT · 2 marks · Pitot intake at supersonic speed

A pitot-type intake flies at Mach 2.0 with a normal shock standing at its lip $`(\gamma = 1.4)`$. The subsonic diffuser behind the shock has a recovery of 0.97. Find the overall stagnation pressure recovery.

**Solution.** For $`M = 2.0`$ the first bracket of the normal-shock formula is $`(2.4 \times 4/3.6)^{3.5}`$​$`{}= 2.667^{3.5}`$ and the second is $`(2.4/10.8)^{2.5}`$​$`{}= 0.2222^{2.5}`$. Their product gives $`P_{02}/P_{01} = 0.7209`$, with a downstream Mach number of 0.577. Overall recovery $`= 0.7209 \times 0.97 = 0.699`$.

**Answer: 0.699 (range 0.69 to 0.71)**

### Example 4.5 · MCQ · 1 mark · Shock systems in supersonic intakes

At Mach 2, which intake gives the highest stagnation pressure recovery?

- (A) A single normal shock
- (B) One oblique shock followed by a normal shock
- (C) Two oblique shocks followed by a weak normal shock
- (D) All give the same recovery, since $`T_0`$ is conserved

**Solution.** Shock loss rises steeply with the normal Mach number, so splitting the compression into several weak shocks keeps each loss small. At $`M = 2 a`$ single normal shock recovers 0.72, while a 10° oblique shock plus a normal shock recovers about 0.87. Two oblique shocks do better still. (D) confuses $`T_0`$, which is conserved, with $`P_0`$, which is not.

**Answer: (C)**

### Example 4.6 · MSQ · 1 mark · What changes across an intake

For adiabatic flow with friction through a subsonic intake, which statements are correct?

- (A) $`T_0`$ at the compressor face equals the free-stream $`T_0`$
- (B) $`P_0`$ at the compressor face is less than the free-stream $`P_0`$
- (C) Static pressure rises as the air decelerates towards the compressor face
- (D) An intake efficiency of 0.93 means 7% of the static pressure is lost

**Solution.** No heat or work crosses the intake, so $`T_0`$ is unchanged (A). Friction destroys stagnation pressure (B). A diffusing flow converts kinetic energy into static pressure (C). (D) is false because intake efficiency is defined on temperature (enthalpy) rise, not on pressure.

**Answer: (A), (B), (C)**

## 5. Propelling nozzles

A propelling nozzle turns stagnation enthalpy into jet velocity. Always start by comparing $`P_{04}/p_{\mathrm{a}}`$ with the critical pressure ratio to see whether the nozzle is choked.

- Nozzle efficiency: $`\eta_{\mathrm{j}} = (T_{04} - T_5)/(T_{04} - T_5')`$
- Isentropic critical ratio: $`P_0/P_{\mathrm{c}} = ((\gamma + 1)/2)^{\gamma/(\gamma - 1)}`$, which is 1.893 for air and 1.853 for $`\gamma = 4/3`$
- With losses: $`P_{04}/P_{\mathrm{c}} = 1/[1 - (1/\eta_{\mathrm{j}})((\gamma - 1)/(\gamma + 1))]^{\gamma/(\gamma - 1)}`$
- Choked ($`P_{04}/p_{\mathrm{a}}`$ above critical): $`T_{\mathrm{c}} = 2T_{04}/(\gamma + 1)`$, $`c_{\mathrm{j}} = \sqrt{\gamma R T_{\mathrm{c}}}`$, and $`p_{\mathrm{e}} = P_{\mathrm{c}}`$​$`{}> p_{\mathrm{a}}`$ adds pressure thrust
- Unchoked: $`p_{\mathrm{e}} = p_{\mathrm{a}}`$ and $`c_{\mathrm{j}} = \sqrt{2c_p\cdot \eta_{\mathrm{j}}\cdot T_{04}[1 - (p_{\mathrm{a}}/P_{04})^{(\gamma - 1)/\gamma}]}`$
- Area–velocity relation: $`\mathrm{d}A/A = (M^{2} - 1)\cdot \mathrm{d}u/u`$, so supersonic flow needs a diverging passage

### Example 5.1 · NAT · 1 mark · Critical pressure ratio

Find the critical pressure ratio $`P_0/P_{\mathrm{c}}`$ for isentropic flow of combustion gas with $`\gamma = 4/3`$.

**Solution.** $`((\gamma + 1)/2)^{\gamma/(\gamma - 1)}`$​$`{}= (7/6)^{4}`$​$`{}= 1.853`$. For air $`(\gamma = 1.4)`$ the same formula gives 1.893.

**Answer: 1.853 (range 1.84 to 1.86)**

### Example 5.2 · MCQ · 2 marks · Is the nozzle choked?

A convergent nozzle with $`\eta_{\mathrm{j}} = 0.95`$ receives gas $`(\gamma = 4/3)`$ at $`P_{04} = 200\ \mathrm{kPa}`$ and exhausts to $`p_{\mathrm{a}} = 100\ \mathrm{kPa}`$. The nozzle is:

- (A) Unchoked, with exit pressure equal to 100 kPa
- (B) Choked, with exit pressure of about 104 kPa
- (C) Choked, with exit pressure equal to 100 kPa
- (D) Choked, with exit pressure of about 108 kPa

**Solution.** The bracket is $`1 - (1/0.95)(1/7) = 0.8496`$, so $`P_{04}/P_{\mathrm{c}} = 1/0.8496^{4}`$​$`{}= 1.919`$. $`P_{04}/p_{\mathrm{a}} = 2.0`$ exceeds this, so the nozzle is choked and $`P_{\mathrm{c}} = 200/1.919`$​$`{}= 104.2\ \mathrm{kPa}`$. Option (D) uses the isentropic ratio 1.853; losses raise the critical ratio, so that is wrong.

**Answer: (B)**

### Example 5.3 · NAT · 2 marks · Exit area of a choked nozzle

Use the nozzle of Example 5.2 with $`T_{04} = 1000\ \mathrm{K}`$ and a mass flow of 25 kg/s. Find the exit area in $`m^{2}`$. Take $`R = 287\ \mathrm{J/kg{\cdot}K}`$.

**Solution.**

1. $`T_{\mathrm{c}} = 2T_{04}/(\gamma + 1)`$​$`{}= 1000 \times 6/7`$​$`{}= 857.1\ \mathrm{K}`$.
2. $`c_{\mathrm{j}} = \sqrt{\gamma R T_{\mathrm{c}}}`$​$`{}= \sqrt{1.333 \times 287 \times 857.1}`$​$`{}= 572.7\ \mathrm{m/s}`$.
3. $`\rho_{\mathrm{c}} = P_{\mathrm{c}}/(R T_{\mathrm{c}})`$​$`{}= 104{,}217/(287 \times 857.1)`$​$`{}= 0.4236\ \mathrm{kg/m^3}`$.
4. $`A = \dot m/(\rho_{\mathrm{c}}\cdot c_{\mathrm{j}})`$​$`{}= 25/(0.4236 \times 572.7)`$​$`{}= 0.1030\ \mathrm{m^2}`$.

The pressure thrust is $`(104.2 - 100)\ \mathrm{kPa} \times {}`$​$`0.1030\ \mathrm{m^2}`$​$`{}= 0.43\ \mathrm{kN}`$. It adds to a momentum thrust of $`25 \times 572.7 = 14.3\ \mathrm{kN}`$ when static.

**Answer: 0.103 m² (range 0.101 to 0.105)**

### Example 5.4 · NAT · 1 mark · Unchoked nozzle jet velocity

Gas at $`T_{04} = 900\ \mathrm{K}`$ expands through a convergent nozzle with $`P_{04}/p_{\mathrm{a}} = 1.6`$ and $`\eta_{\mathrm{j}} = 0.95`$. Take $`c_p = 1148\ \mathrm{J/kg{\cdot}K}`$ and $`\gamma = 4/3`$. Find the jet velocity in m/s.

**Solution.** 1.6 is below the critical 1.919, so the nozzle is unchoked and $`p_{\mathrm{e}} = p_{\mathrm{a}}`$. Isentropic drop $`= 900 \times [1 - (1/1.6)^{0.25}]`$​$`{}= 900 \times 0.11086`$​$`{}= 99.77\ \mathrm{K}`$. Actual drop $`= 0.95 \times 99.77 = 94.79\ \mathrm{K}`$. $`c_{\mathrm{j}} = \sqrt{2 \times 1148 \times 94.79}`$​$`{}= 466.5\ \mathrm{m/s}`$.

**Answer: 466.5 m/s (range 463 to 470)**

### Example 5.5 · NAT · 1 mark · Convergent–divergent nozzle

Air $`(\gamma = 1.4)`$ expands isentropically in a convergent–divergent nozzle from $`P_0 = 1\ \mathrm{MPa}`$ to $`p_{\mathrm{e}} = 58.5\ \mathrm{kPa}`$. Find the exit-to-throat area ratio.

**Solution.** $`P_0/p_{\mathrm{e}} = 17.09`$. From $`P_0/p = (1 + 0.2M^{2})^{3.5}`$, $`M_{\mathrm{e}} = \sqrt{5 \times (17.09^{0.2857} - 1)}`$​$`{}= 2.50`$. $`A/A^{*} = (1/M)[(2/(\gamma + 1))(1 + 0.2M^{2})]^{3}`$​$`{}= (1/2.5) \times 1.875^{3}`$​$`{}= 2.637`$.

**Answer: 2.64 (range 2.62 to 2.66)**

### Example 5.6 · MCQ · 1 mark · Over-expansion

A convergent–divergent nozzle designed for an exit pressure of 50 kPa runs at sea level (101 kPa) with its design chamber conditions. The flow at exit is:

- (A) Under-expanded, with expansion fans at the lip
- (B) Over-expanded, with oblique shocks at the lip
- (C) Perfectly expanded
- (D) Sonic at the exit plane

**Solution.** $`p_{\mathrm{e}} = 50\ \mathrm{kPa}`$ is below $`p_{\mathrm{a}} = 101\ \mathrm{kPa}`$, so the jet is over-expanded. It adjusts to ambient through oblique shocks at the lip, or a normal shock inside the nozzle if $`p_{\mathrm{a}}`$ is high enough. Under-expansion $`(p_{\mathrm{e}} > p_{\mathrm{a}})`$ gives expansion fans instead.

**Answer: (B)**

### Example 5.7 · MSQ · 2 marks · Lowering back pressure on a choked nozzle

A convergent nozzle is already choked. The ambient pressure is lowered further while $`P_{04}`$ and $`T_{04}`$ stay fixed. Which statements are correct?

- (A) Mass flow increases
- (B) Exit-plane pressure stays the same
- (C) Thrust increases because of the pressure term
- (D) Exit Mach number stays 1

**Solution.** Once the nozzle is choked, downstream changes cannot travel upstream, so $`\dot m`$, $`P_{\mathrm{c}}`$ and the exit Mach number of 1 are frozen. That makes (B) and (D) true and (A) false. Thrust still rises because $`(p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$ grows as $`p_{\mathrm{a}}`$ falls, so (C) is true.

**Answer: (B), (C), (D)**

## 6. Combustors and afterburners

The combustor sets the turbine entry temperature through the fuel–air ratio. The overall mixture is very lean, so the air is split into zones to keep the flame stable.

- Energy balance: $`(1 + f)c_{p\mathrm{g}}\cdot T_{03}`$​$`{}= c_{p\mathrm{a}}\cdot T_{02} + f\cdot \eta_{\mathrm{b}}\cdot Q_{\mathrm{R}}`$, so $`f = (c_{p\mathrm{g}}\cdot T_{03} - c_{p\mathrm{a}}\cdot T_{02})/(\eta_{\mathrm{b}}\cdot Q_{\mathrm{R}} - c_{p\mathrm{g}}\cdot T_{03})`$
- Stoichiometric ratio for $`\mathrm{C}_x\mathrm{H}_y +{}`$​$`(x + y/4)(\mathrm{O_{2}} + 3.76\mathrm{N_{2}})`$: $`f_{\mathrm{st}} = (12x + y)/(137.28(x + y/4))`$; for $`\mathrm{C}_n\mathrm{H}_{2n+2}`$ this is $`(7n + 1)/(34.32(3n + 1))`$
- Equivalence ratio: $`\phi = f/f_{\mathrm{st}}`$, lean when $`\phi < 1`$ and rich when $`\phi > 1`$
- Combustion efficiency: $`\eta_{\mathrm{b}} =`$ f\_theoretical/f\_actual for the same temperature rise
- Pressure loss factor: $`\mathrm{PLF} = \Delta P_0/(\dot m^{2}/(2\rho_1\cdot A_{\mathrm{m}}^{2}))`$​$`{}= K_1 + K_2(T_{03}/T_{02} - 1)`$, the cold (friction) loss plus the hot (heating) loss
- Zones: primary (near stoichiometric, recirculation holds the flame), secondary (completes burning), dilution (cools gas to the turbine limit and shapes its temperature profile)

### Example 6.1 · NAT · 1 mark · Stoichiometric fuel–air ratio

Kerosene is approximated as $`\mathrm{C_{12}H_{26}}`$. Find the stoichiometric fuel–air ratio, taking air as $`\mathrm{O_{2}} + 3.76\mathrm{N_{2}}`$.

**Solution.** For $`\mathrm{C}_n\mathrm{H}_{2n+2}`$ with $`n = 12`$: $`f_{\mathrm{st}} = 85/(34.32 \times 37)`$​$`{}= 85/1269.8`$​$`{}= 0.0669`$. From first principles, oxygen needed $`= 12 + 26/4 = 18.5\ \mathrm{mol}`$ per mol of fuel. Air mass $`= 18.5 \times 137.28 = 2539.7\ \mathrm{g}`$ against 170 g of fuel, giving 0.0669 again (air–fuel ratio about 15).

**Answer: 0.0669 (range 0.066 to 0.068)**

### Example 6.2 · NAT · 1 mark · Equivalence ratio

A combustor burning the kerosene of Example 6.1 runs at an overall fuel–air ratio of 0.02. Find the equivalence ratio.

**Solution.** $`\phi = f/f_{\mathrm{st}}`$​$`{}= 0.02/0.0669`$​$`{}= 0.299`$. Such a lean mixture would not burn on its own, so only the primary-zone air burns near stoichiometric while the rest cools and dilutes.

**Answer: 0.299 (range 0.29 to 0.31)**

### Example 6.3 · NAT · 2 marks · Fuel–air ratio from an energy balance

Air enters a combustor at $`T_{02} = 600\ \mathrm{K}`$ and leaves at $`T_{03} = 1400\ \mathrm{K}`$. Take $`c_{p\mathrm{a}} = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`c_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$, $`Q_{\mathrm{R}} = 43{,}000\ \mathrm{kJ/kg}`$ and $`\eta_{\mathrm{b}} = 0.98`$. Find the fuel–air ratio.

**Solution.** $`f = (c_{p\mathrm{g}}\cdot T_{03} - c_{p\mathrm{a}}\cdot T_{02})/(\eta_{\mathrm{b}}\cdot Q_{\mathrm{R}} - c_{p\mathrm{g}}\cdot T_{03})`$​$`{}= (1607.2 - 603.0)/(42{,}140 - 1607.2)`$​$`{}= 1004.2/40{,}532.8`$​$`{}= 0.0248`$.

**Answer: 0.0248 (range 0.0244 to 0.0252)**

### Example 6.4 · NAT · 1 mark · Combustion efficiency

Complete combustion would need a fuel–air ratio of 0.0230 to reach the required turbine entry temperature, but the engine actually uses 0.0240. Find the combustion efficiency.

**Solution.** $`\eta_{\mathrm{b}} =`$ f\_theoretical/f\_actual $`= 0.0230/0.0240 = 0.958`$.

**Answer: 0.958 (range 0.955 to 0.961)**

### Example 6.5 · NAT · 2 marks · Combustor pressure loss

A combustor passes 20 kg/s of air at $`P_{02} = 1.2\ \mathrm{MPa}`$ and $`T_{02} = 600\ \mathrm{K}`$ through a maximum casing area $`A_{\mathrm{m}} = 0.1\ \mathrm{m^2}`$. Its loss factor is $`\mathrm{PLF} = 20 + 2(T_{03}/T_{02} - 1)`$ with $`T_{03} = 1350\ \mathrm{K}`$. Find the stagnation pressure loss as a percentage of $`P_{02} (R = 287\ \mathrm{J/kg{\cdot}K})`$.

**Solution.**

1. $`\rho_1 = P_{02}/(R T_{02})`$​$`{}= 1.2 \times 10^{6}/(287 \times 600)`$​$`{}= 6.969\ \mathrm{kg/m^3}`$.
2. Reference dynamic head $`= \dot m^{2}/(2\rho_1\cdot A_{\mathrm{m}}^{2})`$​$`{}= 400/(2 \times 6.969 \times 0.01)`$​$`{}= 2870\ \mathrm{Pa}`$.
3. $`\mathrm{PLF} = 20 + 2 \times (2.25 - 1)`$​$`{}= 22.5`$, so $`\Delta P_0 = 22.5 \times 2870`$​$`{}= 64.6\ \mathrm{kPa}`$.
4. $`\Delta P_0/P_{02} = 64.6/1200`$​$`{}= 5.38\%`$.

**Answer: 5.38% (range 5.3 to 5.5)**

### Example 6.6 · NAT · 2 marks · Afterburner thrust augmentation

A turbojet flies at 250 m/s. Without afterburning, gas leaves the turbine at 950 K and the fully expanded jet speed is 560 m/s. The afterburner raises the stagnation temperature to 1900 K at the same nozzle pressure ratio, with the nozzle area opening to suit. Neglecting fuel mass and pressure losses, find the ratio of thrust with afterburning to thrust without.

**Solution.**

1. At a fixed nozzle pressure ratio, $`c_{\mathrm{j}}`$ is proportional to $`\sqrt{T_0}`$, so $`c_{\mathrm{j,ab}} = 560 \times \sqrt{1900/950}`$​$`{}= 792.0\ \mathrm{m/s}`$.
2. Thrust ratio $`= (792.0 - 250)/(560 - 250)`$​$`{}= 542.0/310`$​$`{}= 1.748`$.

On the ground $`(c_{\mathrm{i}} = 0)`$ the same reheat gives only $`792/560 = 1.41`$, so afterburning pays off most at high flight speed. It costs a lot of fuel: with $`\eta_{\mathrm{ab}} = 0.95`$, $`f_{\mathrm{ab}} = 1.148 \times {}`$​$`950/(0.95 \times 43{,}000 - 1.148 \times 1900)`$​$`{}= 0.028`$.

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

Cycle analysis is a chain: intake, compressor, combustor, turbine work balance, nozzle, thrust. Carry $`T_0`$ and $`P_0`$ station by station and the rest follows.

- Work balance (fuel mass neglected): $`c_{p\mathrm{g}}(T_{03} - T_{04})`$​$`{}= c_{p\mathrm{a}}(T_{02} - T_{01})/\eta_{\mathrm{m}}`$
- Turbofan: $`\dot m_{\mathrm{h}} = \dot m_{\mathrm{a}}/(B + 1)`$ and $`\dot m_{\mathrm{c}} = B\cdot \dot m_{\mathrm{a}}/(B + 1)`$; $`F = \dot m_{\mathrm{c}}(c_{\mathrm{jc}} - c_{\mathrm{i}}) +{}`$​$`\dot m_{\mathrm{h}}[(1 + f)c_{\mathrm{jh}} - c_{\mathrm{i}}]`$, plus any pressure terms
- Turboprop: thrust power $`= \eta_{\mathrm{pr}}\cdot \mathrm{SP} + F_{\mathrm{jet}}\cdot V`$; equivalent shaft power $`\mathrm{ESP} = \mathrm{SP} + F_{\mathrm{jet}}\cdot V/\eta_{\mathrm{pr}}`$
- Turboshaft: the useful output is shaft power from a free power turbine
- Ideal ramjet ($`p_{\mathrm{e}} = p_{\mathrm{a}}`$, constant $`\gamma`$): $`u_{\mathrm{e}}/u_0 = \sqrt{T_{04}/T_{0\mathrm{a}}}`$, so $`F/\dot m = u_0(\sqrt{T_{04}/T_{0\mathrm{a}}} - 1)`$

### Example 7.1 · NAT · 2 marks · Complete turbojet analysis

A turbojet flies at Mach 0.85 at 11 km ($`T_{\mathrm{a}} = 216.65\ \mathrm{K}`$, $`p_{\mathrm{a}} = 22.63\ \mathrm{kPa}`$). Intake $`\eta_{\mathrm{i}} = 0.93`$. Compressor $`\pi_{\mathrm{c}} = 10`$, $`\eta_{\mathrm{c}} = 0.86`$. Combustor loss 5% of $`P_{02}`$, $`T_{03} = 1250\ \mathrm{K}`$, $`\eta_{\mathrm{b}} = 0.98`$, $`Q_{\mathrm{R}} = 43\ \mathrm{MJ/kg}`$. Turbine $`\eta_{\mathrm{t}} = 0.89`$, $`\eta_{\mathrm{m}} = 0.99`$. Convergent nozzle $`\eta_{\mathrm{j}} = 0.95`$. Use $`c_{p\mathrm{a}} = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`\gamma_{\mathrm{a}} = 1.4`$, $`c_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$, $`\gamma_{\mathrm{g}} = 4/3`$ and $`R = 287\ \mathrm{J/kg{\cdot}K}`$. Neglect fuel mass in the work balance and thrust. Find the specific thrust in N·s/kg.

**Solution.**

1. Flight speed: $`c_{\mathrm{i}} = 0.85 \times {}`$​$`\sqrt{1.4 \times 287 \times 216.65}`$​$`{}= 250.8\ \mathrm{m/s}`$.
2. Intake: $`T_{01} = 216.65 \times 1.1445`$​$`{}= 248.0\ \mathrm{K}`$ and $`P_{01} = 22.63 \times {}`$​$`(1 + 0.93 \times 0.1445)^{3.5}`$​$`{}= 35.18\ \mathrm{kPa}`$.
3. Compressor: $`\Delta T_{\mathrm{c}} = 248.0 \times {}`$​$`(10^{0.2857} - 1)/0.86`$​$`{}= 268.3\ \mathrm{K}`$, so $`T_{02} = 516.3\ \mathrm{K}`$ and $`P_{02} = 351.8\ \mathrm{kPa}`$.
4. Combustor: $`P_{03} = 0.95 \times 351.8`$​$`{}= 334.2\ \mathrm{kPa}`$ and $`f = (1.148 \times 1250 - 1.005 \times 516.3)/(0.98 \times 43{,}000 - 1.148 \times 1250)`$​$`{}= 0.0225`$.
5. Turbine: $`\Delta T_{\mathrm{t}} = 1.005 \times {}`$​$`268.3/(0.99 \times 1.148)`$​$`{}= 237.3\ \mathrm{K}`$, so $`T_{04} = 1012.7\ \mathrm{K}`$. $`T_{04}' = 1250 - 237.3/0.89`$​$`{}= 983.4\ \mathrm{K}`$, so $`P_{03}/P_{04} = (1250/983.4)^{4}`$​$`{}= 2.611`$ and $`P_{04} = 128.0\ \mathrm{kPa}`$.
6. Nozzle: $`P_{04}/p_{\mathrm{a}} = 5.66`$ exceeds the critical 1.919, so it is choked. $`T_{\mathrm{c}} = 1012.7 \times 6/7`$​$`{}= 868.0\ \mathrm{K}`$, $`P_{\mathrm{c}} = 128.0/1.919`$​$`{}= 66.7\ \mathrm{kPa}`$ and $`c_{\mathrm{j}} = \sqrt{1.333 \times 287 \times 868.0}`$​$`{}= 576.3\ \mathrm{m/s}`$.
7. Exit area per unit flow: $`A/\dot m = R T_{\mathrm{c}}/(P_{\mathrm{c}}\cdot c_{\mathrm{j}})`$​$`{}= (287 \times 868.0)/(66{,}716 \times 576.3)`$​$`{}= 0.006479\ \mathrm{m^2{\cdot}s/kg}`$.
8. $`F_{\mathrm{s}} = (c_{\mathrm{j}} - c_{\mathrm{i}}) +{}`$​$`(P_{\mathrm{c}} - p_{\mathrm{a}}) \cdot A/\dot m`$​$`{}= 325.6 + 44{,}086 \times {}`$​$`0.006479`$​$`{}= 325.6 + 285.6`$​$`{}= 611.2\ \mathrm{N{\cdot}s/kg}`$.

$`\mathrm{TSFC} = f/F_{\mathrm{s}}`$​$`{}= 0.0225/611.2`$​$`{}= 3.68 \times 10^{-5}\ \mathrm{kg/(N{\cdot}s)}`$, or 0.133 kg/(N·h). Almost half the thrust comes from the pressure term of the choked convergent nozzle at altitude.

**Answer: 611 N·s/kg (range 600 to 622)**

### Example 7.2 · NAT · 1 mark · Turbofan static thrust

A separate-exhaust turbofan with bypass ratio 5 swallows 300 kg/s on the test bed. The cold jet leaves at 300 m/s and the hot jet at 450 m/s, both fully expanded. Neglecting fuel mass, find the thrust in kN.

**Solution.** $`\dot m_{\mathrm{h}} = 300/6`$​$`{}= 50\ \mathrm{kg/s}`$ and $`\dot m_{\mathrm{c}} = 250\ \mathrm{kg/s}`$. $`F = 250 \times 300 + 50 \times 450`$​$`{}= 75{,}000 + 22{,}500`$​$`{}= 97{,}500\ \mathrm{N}`$. The fan stream gives 77% of the thrust, typical of a high-bypass engine.

**Answer: 97.5 kN (range 97 to 98)**

### Example 7.3 · NAT · 2 marks · Turbofan at cruise

A turbofan with $`B = 5`$ and a total airflow of 240 kg/s flies at 250 m/s. The cold jet leaves at 360 m/s and the hot jet at 480 m/s, both fully expanded. The fuel–air ratio is 0.018 based on core air. Find the TSFC in kg/(N·h).

**Solution.**

1. $`\dot m_{\mathrm{h}} = 240/6`$​$`{}= 40\ \mathrm{kg/s}`$, $`\dot m_{\mathrm{c}} = 200\ \mathrm{kg/s}`$ and $`\dot m_{\mathrm{f}} = 0.018 \times 40`$​$`{}= 0.72\ \mathrm{kg/s}`$.
2. Cold thrust $`= 200 \times (360 - 250)`$​$`{}= 22{,}000\ \mathrm{N}`$.
3. Hot thrust $`= 40 \times (1.018 \times 480 - 250)`$​$`{}= 40 \times 238.6`$​$`{}= 9{,}546\ \mathrm{N}`$.
4. $`F = 31{,}546\ \mathrm{N}`$, so $`\mathrm{TSFC} = 0.72 \times 3600/31{,}546`$​$`{}= 0.0822\ \mathrm{kg/(N{\cdot}h)}`$.

**Answer: 0.0822 kg/(N·h) (range 0.081 to 0.083)**

### Example 7.4 · NAT · 1 mark · Turboprop equivalent shaft power

A turboprop delivers 3000 kW to its propeller $`(\eta_{\mathrm{pr}} = 0.85)`$ and also produces 2000 N of residual jet thrust at a flight speed of 150 m/s. Find the equivalent shaft power in kW.

**Solution.** Jet thrust power $`= 2000 \times 150 = 300\ \mathrm{kW}`$. $`\mathrm{ESP} = \mathrm{SP} + F_{\mathrm{jet}}\cdot V/\eta_{\mathrm{pr}}`$​$`{}= 3000 + 300/0.85`$​$`{}= 3352.9\ \mathrm{kW}`$. The total thrust power is $`0.85 \times 3000 + 300`$​$`{}= 2850\ \mathrm{kW}`$. At a fuel flow of 0.25 kg/s, $`\mathrm{ESFC} = 0.25 \times 3600/3352.9`$​$`{}= 0.268\ \mathrm{kg/(kW{\cdot}h)}`$.

**Answer: 3353 kW (range 3340 to 3365)**

### Example 7.5 · NAT · 2 marks · Turboshaft free power turbine

A gas generator supplies 10 kg/s of gas at $`T_{04} = 1050\ \mathrm{K}`$ and $`P_{04} = 300\ \mathrm{kPa}`$ to a free power turbine exhausting at 105 kPa. The power turbine isentropic efficiency is 0.88 ($`c_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$, $`\gamma = 4/3`$). Find the shaft power in MW.

**Solution.** Isentropic drop $`= 1050 \times {}`$​$`[1 - (105/300)^{0.25}]`$​$`{}= 1050 \times 0.2308`$​$`{}= 242.4\ \mathrm{K}`$. Actual drop $`= 0.88 \times 242.4 = 213.3\ \mathrm{K}`$. Power $`= 10 \times 1.148 \times 213.3`$​$`{}= 2449\ \mathrm{kW}`$.

**Answer: 2.45 MW (range 2.42 to 2.48)**

### Example 7.6 · NAT · 2 marks · Ideal ramjet

An ideal ramjet flies at Mach 3 where $`T_{\mathrm{a}} = 220\ \mathrm{K}`$, and its burner exit stagnation temperature is 2000 K. Take $`\gamma = 1.4`$ throughout, $`R = 287\ \mathrm{J/kg{\cdot}K}`$, full expansion and negligible fuel mass. Find the specific thrust in N·s/kg.

**Solution.**

1. $`u_0 = 3 \times {}`$​$`\sqrt{1.4 \times 287 \times 220}`$​$`{}= 891.9\ \mathrm{m/s}`$ and $`T_{0\mathrm{a}} = 220 \times (1 + 0.2 \times 9)`$​$`{}= 616\ \mathrm{K}`$.
2. With no $`P_0`$ loss and $`p_{\mathrm{e}} = p_{\mathrm{a}}`$, the exit Mach number equals the flight Mach number, so $`u_{\mathrm{e}}/u_0 = \sqrt{T_{04}/T_{0\mathrm{a}}}`$​$`{}= \sqrt{2000/616}`$​$`{}= 1.802`$.
3. $`F/\dot m = u_0(1.802 - 1)`$​$`{}= 715\ \mathrm{N{\cdot}s/kg}`$, and $`\eta_{\mathrm{p}} = 2/(1 + 1.802)`$​$`{}= 0.714`$.

**Answer: 715 N·s/kg (range 708 to 722)**

### Example 7.7 · MSQ · 2 marks · Performance trends

Which statements are correct?

- (A) At the same thrust, a turbofan has a higher propulsive efficiency than a turbojet
- (B) At a fixed turbine entry temperature, a turbojet's specific thrust keeps rising as compressor pressure ratio increases
- (C) At a fixed turbine entry temperature, raising the pressure ratio from 5 to 15 lowers a turbojet's SFC
- (D) At a fixed flight Mach number, thrust falls with altitude

**Solution.** (A) is true because more air at a lower jet speed raises $`\eta_{\mathrm{p}}`$. (B) is false: specific thrust peaks at an optimum pressure ratio, as in the carpet plot in your notes. (C) is true because higher pressure ratio raises thermal efficiency over this range. (D) is true because air density, and so mass flow, falls with altitude.

**Answer: (A), (C), (D)**

## 8. Axial compressors

Each stage is a rotor followed by a stator. The rotor adds energy through the Euler equation; the stator only diffuses. With angles from the axial direction and constant $`C_{\mathrm{a}}`$:

- Velocity triangles: $`U/C_{\mathrm{a}} = \tan\alpha_1 + \tan\beta_1`$​$`{}= \tan\alpha_2 + \tan\beta_2`$
- Stage work: $`W = \lambda\cdot U\cdot C_{\mathrm{a}}(\tan\beta_1 - \tan\beta_2)`$​$`{}= \lambda\cdot U\cdot C_{\mathrm{a}}(\tan\alpha_2 - \tan\alpha_1)`$, and $`\Delta T_{0\mathrm{s}} = W/c_p`$
- Stage pressure ratio: $`R_{\mathrm{s}} = (1 + \eta_{\mathrm{s}}\cdot \Delta T_{0\mathrm{s}}/T_{01})^{\gamma/(\gamma - 1)}`$
- Degree of reaction: $`R = (\phi/2)(\tan\beta_1 + \tan\beta_2)`$​$`{}= 1 - (\phi/2)(\tan\alpha_1 + \tan\alpha_2)`$
- 50% reaction gives symmetric triangles: $`\alpha_1 = \beta_2`$ and $`\alpha_2 = \beta_1`$
- Multistaging: number of stages = overall $`\Delta T_0/\Delta T_{0\mathrm{s}}`$; $`\lambda`$ falls below 1 in rear stages as the axial velocity profile peaks
- de Haller criterion: keep $`W_2/W_1`$ above about 0.72 to avoid excessive diffusion

### Example 8.1 · NAT · 1 mark · Stage temperature rise

An axial compressor stage has $`U = 280\ \mathrm{m/s}`$ and $`C_{\mathrm{a}} = 160\ \mathrm{m/s}`$. Inlet guide vanes give $`\alpha_1 = 15^\circ`$, and the rotor relative outlet angle is $`\beta_2 = 40^\circ`$, both from the axial direction. With work-done factor $`\lambda = 0.93`$, find the stage stagnation temperature rise $`(c_p = 1005\ \mathrm{J/kg{\cdot}K})`$.

**Solution.** $`\tan\beta_1 = U/C_{\mathrm{a}} - \tan\alpha_1`$​$`{}= 1.75 - 0.2679`$​$`{}= 1.4821`$, so $`\beta_1 = 56.0^\circ`$. $`W = \lambda\cdot U\cdot C_{\mathrm{a}}(\tan\beta_1 - \tan\beta_2)`$​$`{}= 0.93 \times 280 \times 160 \times {}`$​$`(1.4821 - 0.8391)`$​$`{}= 26{,}788\ \mathrm{J/kg}`$. $`\Delta T_{0\mathrm{s}} = 26{,}788/1005`$​$`{}= 26.7\ \mathrm{K}`$.

**Answer: 26.7 K (range 26.4 to 26.9)**

### Example 8.2 · NAT · 1 mark · Stage pressure ratio

For the stage of Example 8.1, $`T_{01} = 288\ \mathrm{K}`$ and the stage isentropic efficiency is 0.88. Find the stage pressure ratio $`(\gamma = 1.4)`$.

**Solution.** $`R_{\mathrm{s}} = (1 + 0.88 \times 26.65/288)^{3.5}`$​$`{}= 1.0814^{3.5}`$​$`{}= 1.315`$.

**Answer: 1.315 (range 1.31 to 1.32)**

### Example 8.3 · NAT · 1 mark · Degree of reaction

Find the degree of reaction of the stage in Example 8.1.

**Solution.** $`R = (\phi/2)(\tan\beta_1 + \tan\beta_2)`$​$`{}= (160/560) \times {}`$​$`(1.4821 + 0.8391)`$​$`{}= 0.2857 \times 2.3212`$​$`{}= 0.663`$. As a check, $`\tan\alpha_2 = 1.75 - 0.8391`$​$`{}= 0.9109\quad (\alpha_2 = 42.3^\circ)`$, and $`R = 1 - 0.2857 \times {}`$​$`(0.2679 + 0.9109)`$​$`{}= 0.663`$. The rotor does about two-thirds of the static enthalpy rise.

**Answer: 0.663 (range 0.655 to 0.670)**

### Example 8.4 · NAT · 2 marks · Number of stages

An axial compressor must deliver an overall pressure ratio of 6 from $`T_{01} = 288\ \mathrm{K}`$, with an overall isentropic efficiency of 0.86. Each stage gives $`\Delta T_{0\mathrm{s}} = 22\ \mathrm{K}`$. Find the minimum number of stages $`(\gamma = 1.4)`$.

**Solution.** Overall $`\Delta T_0 = 288 \times {}`$​$`(6^{0.2857} - 1)/0.86`$​$`{}= 288 \times 0.6685/0.86`$​$`{}= 223.9\ \mathrm{K}`$. Stages $`= 223.9/22 = 10.18`$, so 11 stages are needed; 10 would fall short of the pressure ratio.

**Answer: 11**

### Example 8.5 · NAT · 2 marks · Designing a 50% reaction stage

A 50% reaction stage has $`U = 300\ \mathrm{m/s}`$, flow coefficient $`\phi = 0.5`$ and blade loading $`\psi = \Delta h_0/U^{2}`$​$`{}= 0.35\quad (\lambda = 1)`$. Find the rotor inlet relative angle $`\beta_1`$ in degrees.

**Solution.**

1. $`\psi = \phi(\tan\beta_1 - \tan\beta_2)`$ gives $`\tan\beta_1 - \tan\beta_2 = 0.7`$.
2. $`R = (\phi/2)(\tan\beta_1 + \tan\beta_2)`$​$`{}= 0.5`$ gives $`\tan\beta_1 + \tan\beta_2 = 2`$.
3. So $`\tan\beta_1 = 1.35\quad (\beta_1 = 53.5^\circ)`$ and $`\tan\beta_2 = 0.65\quad (\beta_2 = 33.0^\circ)`$. By symmetry $`\alpha_2 = 53.5^\circ`$ and $`\alpha_1 = 33.0^\circ`$.

The de Haller number $`W_2/W_1 = \cos\beta_1/\cos\beta_2`$​$`{}= 0.595/0.839`$​$`{}= 0.71`$, just under 0.72, so this loading sits at the diffusion limit. The stage $`\Delta T_0 = 0.35 \times 300^{2}/1005`$​$`{}= 31.3\ \mathrm{K}`$.

**Answer: 53.5° (range 53 to 54)**

### Example 8.6 · MSQ · 1 mark · What happens in the rotor

In an axial compressor rotor, which statements are correct?

- (A) The relative velocity decreases
- (B) The absolute velocity increases
- (C) The stagnation pressure increases
- (D) The stagnation enthalpy stays constant

**Solution.** The rotor passages diffuse the relative flow (A) while turning the absolute flow, which raises its swirl and speed (B). Work input raises $`h_0`$ and $`P_0`$, so (C) holds and (D) fails. What stays constant in the rotor is rothalpy, $`h + W^{2}/2 - U^{2}/2`$; the stator then lowers C and raises static pressure at constant $`h_0`$.

**Answer: (A), (B), (C)**

## 9. Centrifugal compressors

Air enters axially through the inducer, is flung outward by the impeller and is slowed in the diffuser. With no inlet swirl the Euler work is $`U_2\cdot C_{\mathrm{t}2}`$, and slip keeps $`C_{\mathrm{t}2}`$ below $`U_2`$.

- Tip speed: $`U_2 = \pi D_2 N/60`$
- Slip factor: $`\sigma = C_{\mathrm{t}2}/U_2`$; for radial vanes, Stanitz gives $`\sigma = 1 - 0.63\pi/n`$
- Work input: $`W = \psi\cdot \sigma\cdot U_2^{2}`$, where $`\psi \ge 1`$ is the power input factor (disc friction and windage)
- Temperature rise: $`T_{02} - T_{01} = \psi\sigma U_2^{2}/c_p`$
- Pressure ratio: $`P_{03}/P_{01} = [1 + \eta_{\mathrm{c}}\cdot \psi\sigma U_2^{2}/(c_p\cdot T_{01})]^{\gamma/(\gamma - 1)}`$
- Vane shape (outlet angle $`\beta_2`$ from the tangent, as in your notes): forward $`\beta_2 > 90^\circ`$, radial = 90°, backward < 90°; $`W = U_2^{2} - U_2\cdot C_{\mathrm{r}2}\cdot \cot\beta_2`$​$`{}= k_1 - k_2\cdot Q`$
- Inducer: the relative Mach number peaks at the inducer tip; keeping it below about 0.9 limits shock losses

### Example 9.1 · NAT · 1 mark · Impeller tip speed

An impeller with a 0.5 m tip diameter runs at 18,000 rpm. Find the tip speed in m/s.

**Solution.** $`U_2 = \pi \times 0.5 \times 18{,}000/60`$​$`{}= 471.2\ \mathrm{m/s}`$.

**Answer: 471.2 m/s (range 470 to 472.5)**

### Example 9.2 · NAT · 1 mark · Slip factor

Estimate the slip factor of a radial-vaned impeller with 19 vanes using Stanitz's formula.

**Solution.** $`\sigma = 1 - 0.63\pi/n`$​$`{}= 1 - (0.63 \times 3.1416)/19`$​$`{}= 1 - 0.1042`$​$`{}= 0.896`$. This matches the rule of thumb in your notes that 19 to 21 vanes give $`\sigma \approx 0.9`$.

**Answer: 0.896 (range 0.89 to 0.90)**

### Example 9.3 · NAT · 2 marks · Pressure ratio

A centrifugal compressor has $`U_2 = 450\ \mathrm{m/s}`$, $`\sigma = 0.9`$, power input factor $`\psi = 1.04`$ and overall isentropic efficiency 0.80. Inlet $`T_{01} = 295\ \mathrm{K}`$. Find the total pressure ratio ($`c_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`\gamma = 1.4`$).

**Solution.**

1. $`T_{02} - T_{01} = \psi\sigma U_2^{2}/c_p`$​$`{}= 1.04 \times 0.9 \times 450^{2}/1005`$​$`{}= 188.6\ \mathrm{K}`$.
2. $`P_{03}/P_{01} = (1 + 0.80 \times 188.6/295)^{3.5}`$​$`{}= 1.5115^{3.5}`$​$`{}= 4.24`$.

At 9 kg/s the power needed is $`9 \times 1.005 \times 188.6`$​$`{}= 1706\ \mathrm{kW}`$. As your notes say, designers want $`\sigma`$ as high and $`\psi`$ as low as possible.

**Answer: 4.24 (range 4.20 to 4.29)**

### Example 9.4 · NAT · 2 marks · Inducer tip relative Mach number

An inducer has a tip diameter of 0.30 m and runs at 16,000 rpm. Air enters axially at 150 m/s with $`T_{01} = 295\ \mathrm{K}`$. Find the relative Mach number at the inducer tip ($`\gamma = 1.4`$, $`R = 287\ \mathrm{J/kg{\cdot}K}`$, $`c_p = 1005\ \mathrm{J/kg{\cdot}K}`$).

**Solution.**

1. Static temperature: $`T_1 = 295 - 150^{2}/(2 \times 1005)`$​$`{}= 283.8\ \mathrm{K}`$, so $`a_1 = \sqrt{1.4 \times 287 \times 283.8}`$​$`{}= 337.7\ \mathrm{m/s}`$.
2. Tip speed: $`U_{\mathrm{t}} = \pi \times 0.30 \times 16{,}000/60`$​$`{}= 251.3\ \mathrm{m/s}`$.
3. $`W_1 = \sqrt{150^{2} + 251.3^{2}}`$​$`{}= 292.7\ \mathrm{m/s}`$, so $`M_{\mathrm{rel}} = 292.7/337.7`$​$`{}= 0.867`$.

The inducer blade angle at the tip is $`\tan^{-1}(251.3/150) = 59.2^\circ`$ from the axial direction. Prewhirl from inlet guide vanes would lower $`W_1`$ and $`M_{\mathrm{rel}}`$, at the cost of some work.

**Answer: 0.867 (range 0.86 to 0.875)**

### Example 9.5 · MCQ · 1 mark · Vane shape and stability

Neglecting losses, how does the work input of a backward-curved impeller change as the flow rate rises at constant speed?

- (A) It rises linearly
- (B) It stays constant
- (C) It falls linearly
- (D) It first rises, then falls

**Solution.** $`W = U_2^{2} - U_2\cdot C_{\mathrm{r}2}\cdot \cot\beta_2`$​$`{}= k_1 - k_2\cdot Q`$. For backward vanes $`(\beta_2 < 90^\circ) \cot\beta_2`$ is positive, so work falls as Q rises. Radial vanes give constant work and forward vanes give rising work. The falling characteristic of backward vanes is the most stable.

**Answer: (C)**

### Example 9.6 · MSQ · 1 mark · Vaneless diffuser

In the vaneless space after a centrifugal impeller (constant width, incompressible flow assumed), which statements are correct?

- (A) $`r\cdot C_{\mathrm{t}}`$ stays constant (free vortex)
- (B) The tangential velocity increases with radius
- (C) The radial velocity decreases with radius
- (D) The flow path is a logarithmic spiral

**Solution.** With no blades there is no torque, so angular momentum $`r\cdot C_{\mathrm{t}}`$ is conserved (A) and $`C_{\mathrm{t}}`$ falls as r grows, which rules out (B). Continuity through the area $`2\pi r b`$ gives $`C_{\mathrm{r}} \propto 1/r`$ (C). Both components fall as $`1/r`$, so the flow angle is constant and the path is a logarithmic spiral (D).

**Answer: (A), (C), (D)**

## 10. Axial turbines and blade cooling

A turbine stage is a nozzle row followed by a rotor. Angles are from the axial direction, $`C_{\mathrm{a}}`$ is constant, and swirl is counted positive in the direction that does work.

- Velocity triangles: $`U/C_{\mathrm{a}} = \tan\alpha_2 - \tan\beta_2`$​$`{}= \tan\beta_3 - \tan\alpha_3`$
- Stage work: $`W = U\cdot C_{\mathrm{a}}(\tan\alpha_2 + \tan\alpha_3)`$​$`{}= U\cdot C_{\mathrm{a}}(\tan\beta_2 + \tan\beta_3)`$, and $`\Delta T_{0\mathrm{s}} = W/c_{p\mathrm{g}}`$
- Blade loading: $`\psi = W/U^{2}`$​$`{}= \phi(\tan\beta_2 + \tan\beta_3)`$, with flow coefficient $`\phi = C_{\mathrm{a}}/U`$
- Degree of reaction: $`R = (\phi/2)(\tan\beta_3 - \tan\beta_2)`$​$`{}= 1/2 +{}`$​$`(\phi/2)(\tan\alpha_3 - \tan\beta_2)`$
- Impulse stage $`(R = 0)`$: $`\beta_2 = \beta_3`$. 50% reaction: $`\alpha_2 = \beta_3`$ and $`\beta_2 = \alpha_3`$
- Total-to-total efficiency: $`\eta_{\mathrm{tt}} = (T_{01} - T_{03})/(T_{01} - T_{03}')`$, with $`T_{01}/T_{03}' = (P_{01}/P_{03})^{(\gamma - 1)/\gamma}`$
- Cooling effectiveness: $`\varepsilon = (T_{\mathrm{g}} - T_{\mathrm{b}})/(T_{\mathrm{g}} - T_{\mathrm{c}})`$ for gas, blade and coolant temperatures

### Example 10.1 · NAT · 1 mark · Stage temperature drop

A turbine stage has $`U = 350\ \mathrm{m/s}`$ and $`C_{\mathrm{a}} = 280\ \mathrm{m/s}`$. The nozzle exit angle is $`\alpha_2 = 60^\circ`$ and the flow leaves the rotor axially $`(\alpha_3 = 0)`$. Find the stage stagnation temperature drop $`(c_{p\mathrm{g}} = 1148\ \mathrm{J/kg{\cdot}K})`$.

**Solution.** $`C_{\mathrm{t}2} = C_{\mathrm{a}}\cdot \tan\alpha_2`$​$`{}= 280 \times 1.7321`$​$`{}= 485.0\ \mathrm{m/s}`$ and $`C_{\mathrm{t}3} = 0`$. $`W = U(C_{\mathrm{t}2} + C_{\mathrm{t}3})`$​$`{}= 350 \times 485.0`$​$`{}= 169{,}741\ \mathrm{J/kg}`$. $`\Delta T_{0\mathrm{s}} = 169{,}741/1148`$​$`{}= 147.9\ \mathrm{K}`$.

**Answer: 147.9 K (range 146.5 to 149)**

### Example 10.2 · NAT · 2 marks · Blade angles, loading and reaction

For the stage of Example 10.1, find the degree of reaction.

**Solution.**

1. $`\tan\beta_2 = \tan\alpha_2 - U/C_{\mathrm{a}}`$​$`{}= 1.7321 - 1.25`$​$`{}= 0.4821`$, so $`\beta_2 = 25.7^\circ`$.
2. $`\tan\beta_3 = \tan\alpha_3 + U/C_{\mathrm{a}}`$​$`{}= 1.25`$, so $`\beta_3 = 51.3^\circ`$.
3. $`\psi = W/U^{2}`$​$`{}= 169{,}741/350^{2}`$​$`{}= 1.386`$, which matches $`\phi(\tan\beta_2 + \tan\beta_3)`$​$`{}= 0.8 \times 1.7321`$.
4. $`R = (\phi/2)(\tan\beta_3 - \tan\beta_2)`$​$`{}= 0.4 \times (1.25 - 0.4821)`$​$`{}= 0.307`$.

**Answer: 0.307 (range 0.30 to 0.315)**

### Example 10.3 · NAT · 1 mark · 50% reaction with axial exit

A 50% reaction turbine stage has axial exit flow $`(\alpha_3 = 0)`$ and a mean blade speed of 320 m/s. Find the stage stagnation temperature drop $`(c_{p\mathrm{g}} = 1148\ \mathrm{J/kg{\cdot}K})`$.

**Solution.** For $`R = 0.5`$ the triangles are symmetric, so $`\beta_2 = \alpha_3`$​$`{}= 0`$ and $`\tan\beta_3 = 1/\phi`$. Then $`\psi = \phi(0 + 1/\phi)`$​$`{}= 1`$, so $`W = U^{2}`$. $`\Delta T_{0\mathrm{s}} = 320^{2}/1148`$​$`{}= 89.2\ \mathrm{K}`$.

**Answer: 89.2 K (range 88.5 to 90)**

### Example 10.4 · NAT · 2 marks · Impulse stage blade speed

An impulse stage ($`R = 0`$, symmetric blades) receives gas from its nozzles at $`C_2 = 600\ \mathrm{m/s}`$ with $`\alpha_2 = 70^\circ`$ from the axial direction. The flow must leave axially. Find the required mean blade speed in m/s.

**Solution.** Impulse blading has $`\beta_2 = \beta_3`$, so $`W_{\mathrm{t}2} = W_{\mathrm{t}3}`$. Axial exit gives $`W_{\mathrm{t}3} = U`$, while $`W_{\mathrm{t}2} = C_{\mathrm{t}2} - U`$. Equating them gives $`C_{\mathrm{t}2} = 2U`$, so $`U = C_2\cdot \sin\alpha_2/2`$​$`{}= 600 \times 0.9397/2`$​$`{}= 281.9\ \mathrm{m/s}`$. The work is $`W = U\cdot C_{\mathrm{t}2}`$​$`{}= 2U^{2}`$​$`{}= 158.9\ \mathrm{kJ/kg}`$, so $`\psi = 2`$ for impulse against 1 for 50% reaction.

**Answer: 281.9 m/s (range 279 to 285)**

### Example 10.5 · NAT · 1 mark · Stage efficiency

A turbine stage has $`T_{01} = 1200\ \mathrm{K}`$ and a stagnation pressure ratio $`P_{01}/P_{03} = 1.7`$. The actual stagnation temperature drop is 135 K. Find the total-to-total efficiency $`(\gamma = 4/3)`$.

**Solution.** Ideal drop $`= 1200 \times {}`$​$`[1 - (1/1.7)^{0.25}]`$​$`{}= 1200 \times 0.12423`$​$`{}= 149.1\ \mathrm{K}`$. $`\eta_{\mathrm{tt}} = 135/149.1`$​$`{}= 0.906`$.

**Answer: 0.906 (range 0.90 to 0.91)**

### Example 10.6 · NAT · 1 mark · Blade cooling effectiveness (special topic)

Gas at 1700 K flows over a turbine blade cooled internally by compressor bleed air at 850 K. The cooling effectiveness is 0.6. Find the blade metal temperature in K.

**Solution.** $`\varepsilon = (T_{\mathrm{g}} - T_{\mathrm{b}})/(T_{\mathrm{g}} - T_{\mathrm{c}})`$, so $`T_{\mathrm{b}} = T_{\mathrm{g}} - \varepsilon(T_{\mathrm{g}} - T_{\mathrm{c}})`$​$`{}= 1700 - 0.6 \times 850`$​$`{}= 1190\ \mathrm{K}`$. Cooling lets the gas run about 500 K hotter than the metal.

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

- Map groups: $`P_{02}/P_{01} = f`$($`\dot m\sqrt{T_{01}}/P_{01}`$, $`N/\sqrt{T_{01}}`$); the same groups mean the same operating point
- Work balance: $`c_{p\mathrm{a}}(T_{02} - T_{01})`$​$`{}= \eta_{\mathrm{m}}(1 + f)c_{p\mathrm{g}}(T_{03} - T_{04})`$
- Flow compatibility: $`\dot m\sqrt{T_{01}}/P_{01}`$​$`{}= (\dot m\sqrt{T_{03}}/P_{03}) \cdot (P_{03}/P_{02}) \cdot {}`$​$`(P_{02}/P_{01}) \cdot \sqrt{T_{01}/T_{03}}`$; with choked turbine nozzles the first factor is constant
- Surge at low flow (left of the map), choking at high flow (right); blow-off valves, variable stators and multiple spools keep the working line clear of surge

### Example 11.1 · NAT · 1 mark · Corrected mass flow

On a sea-level test ($`T_{01} = 288\ \mathrm{K}`$, $`P_{01} = 101.3\ \mathrm{kPa}`$) a compressor passes 50 kg/s at 10,000 rpm. At altitude the inlet conditions are $`T_{01} = 250\ \mathrm{K}`$ and $`P_{01} = 50\ \mathrm{kPa}`$. If it runs at the same non-dimensional point, find the mass flow in kg/s.

**Solution.** $`\dot m\sqrt{T_{01}}/P_{01}`$ stays fixed, so $`\dot m = 50 \times (50/101.3) \times {}`$​$`\sqrt{288/250}`$​$`{}= 50 \times 0.4936 \times 1.0733`$​$`{}= 26.5\ \mathrm{kg/s}`$. $`N/\sqrt{T_{01}}`$ also stays fixed, so the speed becomes $`10{,}000 \times \sqrt{250/288}`$​$`{}= 9317\ \mathrm{rpm}`$.

**Answer: 26.5 kg/s (range 26.3 to 26.7)**

### Example 11.2 · NAT · 2 marks · Work balance and turbine pressure ratio

A single-spool engine has $`T_{01} = 288\ \mathrm{K}`$, $`T_{02} = 560\ \mathrm{K}`$, $`T_{03} = 1250\ \mathrm{K}`$, $`f = 0.02`$ and $`\eta_{\mathrm{m}} = 0.99`$. The turbine isentropic efficiency is 0.88. Take $`c_{p\mathrm{a}} = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`c_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$ and $`\gamma_{\mathrm{g}} = 4/3`$. Find the turbine pressure ratio $`P_{03}/P_{04}`$.

**Solution.**

1. Work balance: $`T_{03} - T_{04}`$​$`{}= (1.005 \times 272)/(0.99 \times 1.02 \times 1.148)`$​$`{}= 273.4/1.1593`$​$`{}= 235.8\ \mathrm{K}`$, so $`T_{04} = 1014.2\ \mathrm{K}`$.
2. Isentropic outlet temperature: $`T_{04}' = 1250 - 235.8/0.88`$​$`{}= 982.0\ \mathrm{K}`$.
3. $`P_{03}/P_{04} = (1250/982.0)^{4}`$​$`{}= 2.625`$.

**Answer: 2.625 (range 2.60 to 2.65)**

### Example 11.3 · NAT · 2 marks · Working line with a choked turbine

An engine's turbine nozzles are choked, so $`\dot m\sqrt{T_{03}}/P_{03}`$ is fixed, and the combustor loses a fixed fraction of pressure. At one operating point $`\pi_{\mathrm{c}} = 8`$ and $`T_{03}/T_{01} = 4.0`$. Fuel flow is then raised so that $`T_{03}/T_{01} = 4.84`$ at the same compressor non-dimensional flow. Find the new compressor pressure ratio.

**Solution.** Flow compatibility gives $`\dot m\sqrt{T_{01}}/P_{01} =`$ constant $`\times \pi_{\mathrm{c}} \times \sqrt{T_{01}/T_{03}}`$. Holding the compressor flow fixed means $`\pi_{\mathrm{c}} \propto \sqrt{T_{03}/T_{01}}`$. So $`\pi_{\mathrm{c}} = 8 \times \sqrt{4.84/4.0}`$​$`{}= 8 \times 1.1`$​$`{}= 8.8`$. A hotter turbine pushes the operating point up the speed line toward surge, which is why slamming the throttle is a surge risk.

**Answer: 8.8 (range 8.7 to 8.9)**

### Example 11.4 · MCQ · 1 mark · Reading the compressor map

On a compressor map, moving along a constant $`N/\sqrt{T_{01}}`$ line toward lower $`\dot m\sqrt{T_{01}}/P_{01}`$ eventually leads to:

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

A rocket carries its own oxidiser, so it has no ram drag and its thrust does not depend on flight speed. Most questions reduce to the thrust equation, $`c^{*}`$ and $`C_{\mathrm{F}}`$, or the rocket equation.

- Thrust: $`F = \dot m\cdot v_{\mathrm{e}} + (p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$​$`{}= \dot m\cdot c`$, where c is the effective exhaust velocity
- Specific impulse: $`I_{\mathrm{sp}} = F/(\dot m\cdot g_0)`$​$`{}= c/g_0`$, in seconds
- $`c^{*} = P_{\mathrm{c}}\cdot A_{\mathrm{t}}/\dot m`$ (combustion quality) and $`C_{\mathrm{F}} = F/(P_{\mathrm{c}}\cdot A_{\mathrm{t}})`$ (nozzle quality), so $`c = c^{*}\cdot C_{\mathrm{F}}`$ and $`F = C_{\mathrm{F}}\cdot P_{\mathrm{c}}\cdot A_{\mathrm{t}}`$
- Ideal exhaust velocity: $`v_{\mathrm{e}} = \sqrt{(2\gamma/(\gamma - 1))\cdot R\cdot T_0\cdot [1 - (p_{\mathrm{e}}/P_{\mathrm{c}})^{(\gamma - 1)/\gamma}]}`$
- Rocket equation: $`\Delta V = c\cdot \ln(m_0/m_{\mathrm{f}})`$​$`{}= g_0\cdot I_{\mathrm{sp}}\cdot \ln(m_0/m_{\mathrm{f}})`$
- Identical stages: $`\lambda = m_{\mathrm{PL}}/(m_{\mathrm{p}} + m_{\mathrm{s}})`$, $`\varepsilon = m_{\mathrm{s}}/(m_{\mathrm{p}} + m_{\mathrm{s}})`$, stage mass ratio $`n = (1 + \lambda)/(\varepsilon + \lambda)`$, and $`\Delta V = N\cdot g_0\cdot I_{\mathrm{sp}}\cdot \ln n`$ for N stages
- Solid motor: $`r = a\cdot P_{\mathrm{c}}^{n}`$; equilibrium $`P_{\mathrm{c}}^{1 - n}`$​$`{}= \rho_{\mathrm{p}}\cdot a\cdot c^{*}\cdot (A_{\mathrm{b}}/A_{\mathrm{t}})`$, stable only if $`n < 1`$
- Propulsive efficiency: $`\eta_{\mathrm{p}} = 2(u/c)/(1 + (u/c)^{2})`$, equal to 1 when $`u = c`$

### Example 12.1 · NAT · 1 mark · Thrust and specific impulse

A rocket engine at sea level $`(p_{\mathrm{a}} = 101.3\ \mathrm{kPa})`$ has $`\dot m = 100\ \mathrm{kg/s}`$, exhaust velocity 2800 m/s, exit pressure 70 kPa and exit area 0.8 m². Find the specific impulse in seconds.

**Solution.** $`F = 100 \times 2800 +{}`$​$`(70 - 101.3) \times 10^{3} \times 0.8`$​$`{}= 280{,}000 - 25{,}060`$​$`{}= 254{,}940\ \mathrm{N}`$. $`I_{\mathrm{sp}} = 254{,}940/(100 \times 9.81)`$​$`{}= 259.9\ \mathrm{s}`$. In vacuum the pressure term becomes +56,000 N, giving $`I_{\mathrm{sp}} = 342.5\ \mathrm{s}`$, so over-expansion at sea level costs thrust.

**Answer: 259.9 s (range 258 to 262)**

### Example 12.2 · NAT · 2 marks · Ideal exhaust velocity

Combustion products ($`\gamma = 1.2`$, molar mass 22 kg/kmol) at $`T_0 = 3200\ \mathrm{K}`$ and $`P_{\mathrm{c}} = 7\ \mathrm{MPa}`$ expand isentropically to $`p_{\mathrm{e}} = 0.1\ \mathrm{MPa}`$. Find the exhaust velocity in m/s, taking the universal gas constant as 8314 J/kmol·K.

**Solution.**

1. $`R = 8314/22`$​$`{}= 377.9\ \mathrm{J/kg{\cdot}K}`$ and $`2\gamma/(\gamma - 1) = 12`$.
2. $`(p_{\mathrm{e}}/P_{\mathrm{c}})^{(\gamma - 1)/\gamma}`$​$`{}= (1/70)^{1/6}`$​$`{}= 0.4926`$, so the bracket is 0.5074.
3. $`v_{\mathrm{e}} = \sqrt{12 \times 377.9 \times 3200 \times 0.5074}`$​$`{}= \sqrt{7.363 \times 10^{6}}`$​$`{}= 2714\ \mathrm{m/s}`$.

With $`p_{\mathrm{e}} = p_{\mathrm{a}}`$, $`I_{\mathrm{sp}} = 2714/9.81`$​$`{}= 276.6\ \mathrm{s}`$. A hotter chamber or lighter exhaust raises $`v_{\mathrm{e}}`$ roughly as $`\sqrt{T_0/M}`$.

**Answer: 2714 m/s (range 2690 to 2740)**

### Example 12.3 · NAT · 2 marks $`\cdot c^{*}`$, $`C_{\mathrm{F}}`$ and $`I_{\mathrm{sp}}`$

A rocket chamber at $`P_{\mathrm{c}} = 5\ \mathrm{MPa}`$ has a throat area of 0.02 m², a propellant flow of 65 kg/s and a thrust of 180 kN. Find the specific impulse in seconds.

**Solution.** $`c^{*} = P_{\mathrm{c}}\cdot A_{\mathrm{t}}/\dot m`$​$`{}= (5 \times 10^{6} \times 0.02)/65`$​$`{}= 1538.5\ \mathrm{m/s}`$. $`C_{\mathrm{F}} = F/(P_{\mathrm{c}}\cdot A_{\mathrm{t}})`$​$`{}= 180{,}000/100{,}000`$​$`{}= 1.80`$. $`c = c^{*}\cdot C_{\mathrm{F}}`$​$`{}= 2769\ \mathrm{m/s}`$, so $`I_{\mathrm{sp}} = 2769/9.81`$​$`{}= 282.3\ \mathrm{s}`$.

**Answer: 282.3 s (range 280 to 285)**

### Example 12.4 · NAT · 1 mark · Rocket equation

A single-stage rocket has $`I_{\mathrm{sp}} = 300\ \mathrm{s}`$ and a mass ratio $`m_0/m_{\mathrm{f}} = 4`$. Neglecting gravity and drag, find the velocity gain in m/s.

**Solution.** $`\Delta V = g_0\cdot I_{\mathrm{sp}}\cdot \ln(m_0/m_{\mathrm{f}})`$​$`{}= 9.81 \times 300 \times \ln 4`$​$`{}= 2943 \times 1.3863`$​$`{}= 4080\ \mathrm{m/s}`$.

**Answer: 4080 m/s (range 4060 to 4100)**

### Example 12.5 · NAT · 1 mark · Rocket propulsive efficiency

A rocket with an effective exhaust velocity of 2500 m/s is flying at 1500 m/s. Find its propulsive efficiency.

**Solution.** $`u/c = 0.6`$, so $`\eta_{\mathrm{p}} = (2 \times 0.6)/(1 + 0.36)`$​$`{}= 0.882`$. Unlike a jet engine, a rocket reaches $`\eta_{\mathrm{p}} = 1`$ at $`u = c`$ while still producing full thrust.

**Answer: 0.882 (range 0.875 to 0.89)**

### Example 12.6 · NAT · 2 marks · Two-stage rocket

A two-stage rocket has identical stages, each with payload ratio $`\lambda = 0.1`$, structural ratio $`\varepsilon = 0.1`$ and $`I_{\mathrm{sp}} = 300\ \mathrm{s}`$. Neglecting gravity and drag, find the total velocity gain in m/s.

**Solution.** Stage mass ratio $`n = (1 + \lambda)/(\varepsilon + \lambda)`$​$`{}= 1.1/0.2`$​$`{}= 5.5`$. $`\Delta V = 2 \times 9.81 \times 300 \times {}`$​$`\ln 5.5`$​$`{}= 5886 \times 1.7047`$​$`{}= 10{,}034\ \mathrm{m/s}`$. For the same overall payload fraction (0.83%), a single stage with $`\varepsilon = 0.1`$ reaches only 6,565 m/s, which is the case for staging.

**Answer: 10,034 m/s (range 9,950 to 10,120)**

### Example 12.7 · NAT · 2 marks · Solid motor chamber pressure

A solid propellant burns as $`r = 3.5\cdot P_{\mathrm{c}}^{0.4}\ \mathrm{mm/s}`$ with $`P_{\mathrm{c}}`$ in MPa. Its density is 1750 kg/m³, $`c^{*} = 1500\ \mathrm{m/s}`$ and the burning-surface-to-throat area ratio $`A_{\mathrm{b}}/A_{\mathrm{t}} = 250`$. Find the equilibrium chamber pressure in MPa.

**Solution.**

1. Gas generated $`= \rho_{\mathrm{p}}\cdot A_{\mathrm{b}}\cdot r`$ and nozzle outflow $`= P_{\mathrm{c}}\cdot A_{\mathrm{t}}/c^{*}`$. Equating them gives $`P_{\mathrm{c}}^{1 - n}`$​$`{}= \rho_{\mathrm{p}}\cdot a\cdot c^{*}\cdot (A_{\mathrm{b}}/A_{\mathrm{t}})`$.
2. With $`a = 3.5 \times 10^{-3}\ \mathrm{m/s}`$ per MPa^0.4 and $`P_{\mathrm{c}}`$ in MPa (10⁶ converts MPa to Pa): $`P_{\mathrm{c}}^{0.6} = (1750 \times 3.5 \times 10^{-3} \times 1500 \times 250)/10^{6}`$​$`{}= 2.297`$.
3. $`P_{\mathrm{c}} = 2.297^{1/0.6}`$​$`{}= 4.00\ \mathrm{MPa}`$, and the burn rate is $`3.5 \times 4^{0.4} = 6.09\ \mathrm{mm/s}`$.

Because $`n < 1`$, a pressure rise increases nozzle outflow faster than gas generation, so the motor is stable.

**Answer: 4.0 MPa (range 3.95 to 4.05)**

### Example 12.8 · NAT · 1 mark · Liquid bipropellant flows

A liquid rocket runs at an oxidiser-to-fuel mixture ratio $`\mathrm{O/F} = 2.5`$ with a total propellant flow of 70 kg/s. Find the oxidiser mass flow in kg/s.

**Solution.** $`\dot m_{\mathrm{ox}} = \dot m\cdot (\mathrm{O/F})/(1 + \mathrm{O/F})`$​$`{}= 70 \times 2.5/3.5`$​$`{}= 50\ \mathrm{kg/s}`$, leaving 20 kg/s of fuel.

**Answer: 50 kg/s**

### Example 12.9 · MSQ · 1 mark · Chemical rocket classification

Which of these propellant combinations are hypergolic (ignite on contact)?

- (A) $`\mathrm{N_{2}O_{4}}`$ with UDMH
- (B) Liquid oxygen with liquid hydrogen
- (C) $`\mathrm{N_{2}O_{4}}`$ with MMH
- (D) Liquid oxygen with kerosene (RP-1)

**Solution.** Nitrogen tetroxide ignites on contact with hydrazine-family fuels such as UDMH and MMH, which suits restartable upper stages. $`\mathrm{LOX}/\mathrm{LH_{2}}`$ is cryogenic, gives the highest $`I_{\mathrm{sp}}`$ but needs an igniter. $`\mathrm{LOX}/`$RP-1 is also non-hypergolic. Solid composites (AP + HTPB + Al) and hybrids (solid fuel with a liquid oxidiser) complete the classification.

**Answer: (A), (C)**

## Formula sheet for last-minute revision

Every formula used in this booklet, plus the numbers worth memorising.

| Topic | Formula or fact |
| --- | --- |
| Stagnation | $`T_0/T = 1 + ((\gamma - 1)/2)M^{2}`$; $`P_0/P = (T_0/T)^{\gamma/(\gamma - 1)}`$ |
| Gas properties | $`c_p = \gamma R/(\gamma - 1)`$; $`\gamma = 1 + 2/f`$; $`c_p`$ is 1.005 kJ/kg·K for air, 1.148 for hot gas |
| Entropy | $`\Delta s = c_p \ln(T_2/T_1) -{}`$​$`R \ln(p_2/p_1)`$ |
| Brayton (ideal) | $`\eta = 1 - 1/c`$ with $`c = r^{(\gamma - 1)/\gamma}`$; maximum work at $`c = \sqrt{t}`$ |
| Heat exchanger | $`\eta = 1 - c/t`$, useful only while $`c < \sqrt{t}`$ |
| Polytropic | $`(n - 1)/n`$​$`{}= (\gamma - 1)/(\gamma\cdot \eta_{\infty \mathrm{c}})`$ in compression; $`\eta_{\infty \mathrm{t}}(\gamma - 1)/\gamma`$ in expansion |
| Thrust | $`F = (\dot m_{\mathrm{a}} + \dot m_{\mathrm{f}})c_{\mathrm{j}} - \dot m_{\mathrm{a}} \cdot c_{\mathrm{i}} +{}`$​$`(p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$ |
| Efficiencies | $`\eta_{\mathrm{p}} = 2/(1 + c_{\mathrm{j}}/c_{\mathrm{i}})`$; $`\eta_0 = \eta_{\mathrm{p}}\cdot \eta_{\mathrm{th}}`$​$`{}= F\cdot c_{\mathrm{i}}/(\dot m_{\mathrm{f}}\cdot Q_{\mathrm{R}})`$ |
| Maximum thrust power | $`c_{\mathrm{i}} = c_{\mathrm{j}}/2`$, where $`\eta_{\mathrm{p}} = 66.7\%`$ |
| Range | $`R = (V/(g\cdot \mathrm{TSFC}))(L/D)\ln(W_{\mathrm{i}}/W_{\mathrm{f}})`$, TSFC in kg/(N·s) |
| Intake | $`P_{01}/p_{\mathrm{a}} = [1 + \eta_{\mathrm{i}}((\gamma - 1)/2)M^{2}]^{\gamma/(\gamma - 1)}`$; $`\eta_{\mathrm{ram}} = (P_{01} - p_{\mathrm{a}})/(P_{0\mathrm{a}} - p_{\mathrm{a}})`$ |
| Normal shock at $`M = 2`$ | $`P_{02}/P_{01} = 0.721`$ and $`M_2 = 0.577`$ |
| Nozzle critical ratio | 1.893 for air, 1.853 for $`\gamma = 4/3`$; with losses $`1/[1 - (1/\eta_{\mathrm{j}})(\gamma - 1)/(\gamma + 1)]^{\gamma/(\gamma - 1)}`$ |
| Choked nozzle | $`T_{\mathrm{c}} = 2T_{04}/(\gamma + 1)`$; $`c_{\mathrm{j}} = \sqrt{\gamma R T_{\mathrm{c}}}`$; pressure thrust $`(P_{\mathrm{c}} - p_{\mathrm{a}})A`$ |
| Fuel–air ratio | $`f = (c_{p\mathrm{g}}\cdot T_{03} - c_{p\mathrm{a}}\cdot T_{02})/(\eta_{\mathrm{b}}\cdot Q_{\mathrm{R}} - c_{p\mathrm{g}}\cdot T_{03})`$ |
| Stoichiometric $`\mathrm{C}_n\mathrm{H}_{2n+2}`$ | $`f_{\mathrm{st}} = (7n + 1)/(34.32(3n + 1))`$; about 0.067 for kerosene |
| Combustor loss | $`\mathrm{PLF} = K_1 + K_2(T_{03}/T_{02} - 1)`$ |
| Turbofan | $`\dot m_{\mathrm{h}} = \dot m/(B + 1)`$; $`\dot m_{\mathrm{c}} = B\cdot \dot m/(B + 1)`$ |
| Turboprop | $`\mathrm{ESP} = \mathrm{SP} + F_{\mathrm{jet}}\cdot V/\eta_{\mathrm{pr}}`$ |
| Ideal ramjet | $`F/\dot m = u_0(\sqrt{T_{04}/T_{0\mathrm{a}}} - 1)`$ |
| Euler work | $`W = U_2\cdot C_{\mathrm{t}2} - U_1\cdot C_{\mathrm{t}1}`$ |
| Axial compressor | $`W = \lambda U\cdot C_{\mathrm{a}}(\tan\beta_1 - \tan\beta_2)`$; $`R = (\phi/2)(\tan\beta_1 + \tan\beta_2)`$ |
| Stage pressure ratio | $`R_{\mathrm{s}} = (1 + \eta_{\mathrm{s}}\cdot \Delta T_{0\mathrm{s}}/T_{01})^{\gamma/(\gamma - 1)}`$ |
| de Haller | $`W_2/W_1`$ above about 0.72 |
| Centrifugal | $`\Delta T_0 = \psi\sigma U_2^{2}/c_p`$; $`\sigma = 1 - 0.63\pi/n`$ |
| Axial turbine | $`W = U\cdot C_{\mathrm{a}}(\tan\beta_2 + \tan\beta_3)`$; $`R = (\phi/2)(\tan\beta_3 - \tan\beta_2)`$ |
| Turbine special cases | 50% reaction with axial exit: $`\psi = 1`$. Impulse with axial exit: $`\psi = 2`$ and $`U = C_2\cdot \sin\alpha_2/2`$ |
| Blade cooling | $`\varepsilon = (T_{\mathrm{g}} - T_{\mathrm{b}})/(T_{\mathrm{g}} - T_{\mathrm{c}})`$ |
| Matching | $`\dot m\sqrt{T_{01}}/P_{01}`$ and $`N/\sqrt{T_{01}}`$ fixed at a map point; with a choked turbine, $`\pi_{\mathrm{c}} \propto \sqrt{T_{03}/T_{01}}`$ at fixed compressor flow |
| Rocket thrust | $`F = \dot m v_{\mathrm{e}} + (p_{\mathrm{e}} - p_{\mathrm{a}})A_{\mathrm{e}}`$; $`I_{\mathrm{sp}} = F/`$(ṁg0) |
| $`c^{*}`$ and $`C_{\mathrm{F}}`$ | $`c^{*} = P_{\mathrm{c}}\cdot A_{\mathrm{t}}/\dot m`$; $`C_{\mathrm{F}} = F/(P_{\mathrm{c}}\cdot A_{\mathrm{t}})`$; $`c = c^{*}\cdot C_{\mathrm{F}}`$ |
| Rocket equation | $`\Delta V = g_0\cdot I_{\mathrm{sp}}\cdot \ln(m_0/m_{\mathrm{f}})`$ |
| Staging | $`n = (1 + \lambda)/(\varepsilon + \lambda)`$; $`\Delta V = N\cdot g_0\cdot I_{\mathrm{sp}}\cdot \ln n`$ |
| Solid motor | $`P_{\mathrm{c}}^{1 - n}`$​$`{}= \rho_{\mathrm{p}}\cdot a\cdot c^{*}\cdot (A_{\mathrm{b}}/A_{\mathrm{t}})`$, stable only if $`n < 1`$ |
