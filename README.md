# GATE AE Propulsion: Solved Examples, Test Series and Online Mock Tests

A complete practice set for **Section 5 (Propulsion) of the GATE 2027 Aerospace Engineering (AE) paper**, ordered from basic to advanced.

- **79 solved examples** cover all 12 syllabus topics and every GATE question type (MCQ, MSQ, NAT).
- **10 timed tests (122 questions)** come in two series:
  - 6 numerical tests in GATE style (calculator allowed)
  - 4 conceptual tests you answer in your head, without pen and paper
- **Full solutions** are kept in a separate document from the question papers, so you can attempt a test before you see the answers.
- **An online mock test** runs in the browser. It has a countdown timer, a question palette and GATE marking with negatives, and it shows the solutions after you submit.

## Start here

| What | Read online | Download |
| --- | --- | --- |
| Online mock tests (timed, scored automatically) | [Open the mock test](https://abhishek4650.github.io/gate-ae-propulsion-test-series/) | [index.html](index.html) |
| Solved examples (79, topic-wise) | [solved-examples.md](markdown/solved-examples.md) | [PDF](pdf/solved-examples.pdf) |
| Question papers (10 tests, no answers) | [question-papers.md](markdown/question-papers.md) | [PDF](pdf/question-papers.pdf) |
| Solutions (answer keys and worked solutions) | [solutions.md](markdown/solutions.md) | [PDF](pdf/solutions.pdf) |

The mock test link works once GitHub Pages is turned on for this repository (see [Hosting the mock test](#hosting-the-mock-test)).

## Suggested study plan

1. Work through a topic in the solved examples. Cover each solution, attempt the question yourself, then check it.
2. Take the topic test for that block under time, either online or on paper.
3. Check your answers against the solutions document and redo every question you got wrong.
4. Finish with Test N6 (full-syllabus mock) and Test C4 (conceptual traps).

## The tests

| Test | Level | Topics | Questions | Marks | Time |
| --- | --- | --- | --- | --- | --- |
| N1 | Basic | Thermodynamics, Brayton cycle, thrust, efficiencies | 10 | 15 | 30 min |
| N2 | Basic–intermediate | Intakes, nozzles, combustors | 10 | 15 | 30 min |
| N3 | Intermediate | Turbojet, turbofan, turboprop, ramjet, afterburner, range | 10 | 15 | 30 min |
| N4 | Intermediate–advanced | Axial and centrifugal compressors, axial turbines, matching | 10 | 15 | 30 min |
| N5 | Intermediate–advanced | Rockets | 10 | 15 | 30 min |
| N6 | Advanced | Full-syllabus GATE-level mock | 12 | 18 | 40 min |
| C1 | Basic | Cycles, thrust, efficiencies, engine types | 15 | 15 | 20 min |
| C2 | Intermediate | Intakes, nozzles, combustors, afterburners | 15 | 15 | 20 min |
| C3 | Intermediate–advanced | Turbomachinery, blade cooling, surge, matching | 15 | 15 | 20 min |
| C4 | Advanced | Rockets and cross-topic traps | 15 | 15 | 20 min |

## Syllabus coverage (GATE 2027, Section 5: Propulsion)

| Syllabus item | Solved examples topic |
| --- | --- |
| Basics of thermodynamics | 1 |
| Brayton cycle | 2 |
| Thrust, efficiency and range | 3 |
| Intakes and nozzles | 4, 5 |
| Combustors and afterburners; stoichiometric fuel–air ratio | 6 |
| Ramjet, turbojet, turbofan, turboprop and turboshaft performance | 7 |
| Axial compressors | 8 |
| Centrifugal compressors | 9 |
| Axial turbines; turbine blade cooling (special topic) | 10 |
| Compressor–turbine matching (special topic) | 11 |
| Rockets: thrust, specific impulse, multistaging, solid and liquid propellants | 12 |

## Marking scheme and standard data

- **MCQ:** +1 or +2 if correct. A wrong answer costs $`1/3`$ mark (1-mark question) or $`2/3`$ mark (2-mark question).
- **MSQ:** full marks only for exactly the correct set of options. There is no negative marking.
- **NAT:** full marks if your value is inside the accepted range. There is no negative marking.
- **Standard data** (unless a question says otherwise):
  - Air: $`\gamma = 1.4`$, $`C_p = 1.005\ \mathrm{kJ/kg{\cdot}K}`$, $`R = 287\ \mathrm{J/kg{\cdot}K}`$
  - Hot gas: $`\gamma = 4/3`$, $`C_{p\mathrm{g}} = 1.148\ \mathrm{kJ/kg{\cdot}K}`$
  - $`g_0 = 9.81\ \mathrm{m/s^2}`$
- **Angles** in axial machines are measured from the axial direction.

Formulas are typeset as in textbooks and the GATE paper, with stacked fractions such as $`\displaystyle \frac{P_0}{P} = \left(\frac{T_0}{T}\right)^{\frac{\gamma}{\gamma - 1}}`$, in the markdown files, the PDFs and the online mock. Symbols follow the handwritten notes the set was built from: $`C_p`$ and $`C_{p\mathrm{g}}`$ for specific heats, $`C_{\mathrm{i}}`$ and $`C_{\mathrm{j}}`$ for flight and jet speed, $`P_{\mathrm{a}}`$ and $`P_{\mathrm{e}}`$ for ambient and exit pressure, $`\beta`$ for bypass ratio, $`\eta_{\mathrm{in}}`$ and $`\eta_{\mathrm{nz}}`$ for intake and nozzle efficiency, and $`\Omega`$ for the work-done factor.

## Hosting the mock test

`index.html` is a single page with all the test data inside it, and it needs no server. It loads MathJax from the jsDelivr CDN to typeset the formulas, and shows plain-text notation if MathJax cannot load. To publish it:

1. Open **Settings → Pages** in this repository.
2. Under "Build and deployment", set **Source** to "Deploy from a branch".
3. Choose the **main** branch and the **/ (root)** folder, then click Save.

After a minute the mock test is live at `https://abhishek4650.github.io/gate-ae-propulsion-test-series/`. Your last score on each test is stored in your own browser only.

## Notes

- This is an unofficial practice series. It is not affiliated with GATE or with IIT Madras, the organising institute for GATE 2027.
- Every numerical answer was computed in code, and NAT ranges sit within about 1% of the exact value.
- If you find a mistake, please open an issue with the test and question number.
