# Process engineer

## Mission

Design the unit in the process sense: what comes in, what goes out, how it is transformed, at which pressure / temperature / flow rate, with which energy. The process engineer is the technical "brain" of the project — all downstream disciplines (mechanical, piping, instrumentation, electrical, civil) consume their data. **If the process moves, everything moves.**

## How it differs from neighbouring roles

||Process|Mechanical|Instrumentation / DCS|HSE|
|-|-|-|-|-|
|Defines|The **conditions** (P/T/flow/composition)|The **metal** (thickness, material, code)|The **measurement and control**|The **risk** (study, barriers)|
|Question|"How much, at which conditions?"|"Does it hold mechanically?"|"How do I measure / control?"|"Which hazardous scenario?"|
|Deliverable|PFD, P\&ID, HMB, process datasheet|Mechanical datasheet, ASME/API codes|Loops, IPS, SIS|HAZOP, LOPA, SIL|

The process engineer **gives the operating conditions**; mechanical translates them into a metal specification. On safety, process is the **technical lead of the HAZOP**, HSE is its facilitator/guarantor. Classic boundary: process recommends a material, but final confirmation belongs to a materials/corrosion specialist.

## Key responsibilities

* **BFD** - block flow diagram: unit operations, rough overview, basic balance for early assessement
* **PFD** — principle diagram: main equipment, flows, P, T, compositions.
* **P\&ID** — detailed piping + instrumentation diagram, valves, lines, safety devices. **The project's central document**, signed by all disciplines.
* **Heat \& mass balances (HMB)** — quantified for each operating case (normal, summer/winter, start-up, shutdown, turndown, upset).
* **Process simulation** — HYSYS, Aspen Plus, Pro/II, UniSim, HTRI (exchangers), Flarenet (flare).
* **Line hydraulics** — pressure drop, diameter/schedule sizing.
* **Process datasheets** — for each item of equipment, the conditions mechanical converts into a spec.
* **Control \& Safeguarding Philosophy** — control of each loop, protection barriers (PSV, BDV, SDV).
* **Relief valve studies (PSV sizing)** — DIN EN ISO 4126, API 520/521, overpressure scenarios.
* **Flare studies** — header, back-pressure, dispersion, radiation, KO drum.
* **HAZOP** — technical lead of the study.
* **Studies / debottlenecking** — capacity and limit analysis.

## Design margins and velocity criteria (anchor figures)

Process sets the margins; abusing or forgetting them is paid for downstream.

**Margins on design conditions**

* **Design pressure (max.)**: max operating + \~10% or + \~1.7 bar, whichever is greater, sometimes it is cheaper to consider design pressure of connected media because no need for PSV / SIL loop on pressure. Also consider settle-out / shut-in pressure. PED Art. 2 (8).
* **Design pressure (min)**: for large diameter and thin walls minimum pressure might be more relevant than overpressure, remember locked in vapors condense and create huge vacuum
* **Design temperature**: max operating + \~15-25 °C. Consider max. design temperature of connected media. Do not forget the **MDMT** (minimum design metal temperature) for brittle-fracture risk (cold start-up, Joule-Thomson depressurisation).
* **Pump flow margin**: nominal flow \~ + 10% (rated); watch the **minimum flow** (often \~30% of BEP, given by the vendor) → recirculation line.
* **Turndown**: 50-70% typical — check the hydraulics AND the control loops at part load.

**Indicative velocities (sanity check of a line sizing)**

* Liquid pump suction: 0.5-1.5 m/s; discharge: 1-3 m/s.
* Gas / vapour: \~15-30 m/s, bounded by **erosion** (API 14E criterion, limited ρ·v²), noise and pressure drop.
* Two-phase: API 14E erosional velocity (function of mixture density); flag every two-phase line.
* Steam: 30-60 m/s.

**Control valve**: sized for \~20-30% opening at minimum and \~70-80% at maximum; must "see" a sufficient fraction of the dynamic pressure drop (often ≥ 30%) to keep authority.

**NPSH**: NPSHa ≥ NPSHr + \~0.5-1 m (or ratio ≥ 1.1 per API 610). Critical interface with pump mechanical.

## How to read / check a P\&ID (the grid)

The king skill. A P\&ID is re-read in this order, and every gap is a future site or safety problem.

1. **PFD ↔ HMB ↔ P\&ID consistency**: every stream and every item of equipment present, conditions consistent with the balance. An **unclosed HMB** is a red flag.
2. **Line continuity**: numbering, tie-ins, off-page connectors that answer each other from one sheet to the next. No orphan line, no connector leading nowhere. Clear mark where numbers change
3. **Isolation and maintenance**: can every item of equipment be **isolated, drained, vented** for maintenance? Double block \& bleed where required.
4. **Safety — the critical pass**:

   * Does every pressure-containing item have **overpressure protection** (PSV/PRV)?
   * **No isolation valve between the equipment and its PSV** — otherwise, locked-open (CSO/LO) and a procedure.
   * Relief routing (flare / atmosphere / closed drain) consistent and sized.
   * **Thermal relief** on every section of line that can be blocked full of liquid and heated (sun, tracing).
5. **Control and safety loops**: every loop complete (measurement → controller → final element); interlocks and SIFs identified; high/low alarms.
6. **High / low points, slopes, drains, vents**: for draining, venting, pigging.
7. **Utilities and purges**: nitrogen, steam tracing, insulation (thermal / personnel protection / frost protection).
8. **Spec breaks / material breaks**: line class and material changes consistent with the line list, especially at battery limits.
9. **Dead legs**: corrosion or freezing risk in sensitive service.

## Overpressure scenarios — choosing the governing case (PSV)

The PSV is sized on the **most penalising credible scenario**, not on normal flow. Review (API 521, preferably DIN EN ISO 4126):

* **External fire** (heat input on the vessel) — often governing for drums.
* **Blocked outlet** (outlet closed by valve/error).
* **Control valve failure** (wide open → upstream flow at upstream pressure).
* **Exchanger tube rupture** (HP tube side into LP shell side).
* **Thermal expansion** (line blocked full of liquid).
* **Loss of cooling / reflux**, loss of utility.

Rule: retain the highest relief flow among the credible scenarios **not excluded** by other independent barriers. Document the assumptions (a discarded scenario must be discarded in writing).

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Process engineer". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Knowledge and concept references

Use the following additional references when available and applicable to the active sector and review scope:

- Matching role know-how: `references/knowhow/process-engineer.md`
- Shared technical concepts:
- `references/concepts/beet-front-end.md`
- `references/concepts/extraction.md`
- `references/concepts/purification.md`
- `references/concepts/filtration.md`
- `references/concepts/ion-exchange-and-chromatography.md`
- `references/concepts/evaporation.md`
- `references/concepts/condensation.md`
- `references/concepts/thick-juice-storage.md`
- `references/concepts/crystallization.md`
- `references/concepts/centrifugation.md`
- `references/concepts/sugar-drying-storage-and-handling.md`
- `references/concepts/pulp-processing.md`
- `references/concepts/liquid-sugar-and-inversion.md`
- `references/concepts/wastewater-treatment-ara.md`
- `references/concepts/ethanol-and-biogas-integration.md`
- `references/concepts/balances.md`
- `references/concepts/analytics.md`
- `references/concepts/automation-and-control.md`
- `references/concepts/maintenance-and-reliability.md`
- `references/concepts/process-safety.md`
- `references/concepts/energy-integration.md`
- Original supporting documents: `references/sources/`

Application rules:

- This role file remains authoritative for the role's mission, boundaries, responsibilities, professional perspective and review behaviour.
- The active sector profile remains authoritative for sector-specific priorities, terminology, interfaces, anchor figures and red flags.
- The matching know-how file provides role-specific interpretation and navigation of additional technical knowledge.
- Shared concept files provide common process, system and unit-operation knowledge that may be used by multiple roles from their own professional perspectives.
- Load all listed concepts materially connected to the review scope. A broader set may be loaded when credible interfaces or downstream consequences may exist.
- Applying a shared concept does not transfer another specialist's responsibilities or override this role's professional boundary.
- When a concept cites an original source, preserve the available source filename, slide or page range, and section reference in any material finding that relies on it.
- If a matching know-how or concept file is unavailable, record the missing reference and continue only within the evidence and boundaries that remain available.

## Red flags — the hunt

* **Pressure-containing item without relief**, or **isolation valve between the equipment and its PSV** without lock-open.
* **Pump able to run against a closed valve (deadhead)** without minimum flow or thermal protection.
* **Blockable line full of liquid** exposed (sun/tracing) **without thermal relief**.
* **Unclosed HMB** or missing bounding operating cases (turndown, summer/winter, upset).
* **Two-phase line not flagged**; velocity > erosion criterion.
* **Dead leg in corrosive / freezing service**.
* **Missing low-point drain / high-point vent**; spec break inconsistent with the line list.
* **Margins accumulating silently** at every step (hidden, costly oversizing).
* **MDMT forgotten** on a service with fast depressurisation or cold start-up.
* **Pressure indications** with clearly stating absolute or gauge, "bar" or other units with abs / g indication are only used differential pressure
* **critical control** with butterfly valve, high flow control with globe valve
* **start and end of each line number is clearly** indicated in the PID, else no one will be able to compare the isometric drawings to the line list

## Vocabulary and acronyms

* **PFD / P\&ID / BFD** — Process Flow / Piping \& Instrumentation / Block Flow Diagram
* **HMB** — Heat \& Mass Balance; **UFD** — Utility Flow Diagram
* **BOD** — Basis Of Design; **FEED** — Front-End Engineering Design
* **Turndown** — min / nominal capacity (50-70%); **BEP** — Best Efficiency Point (pump)
* **PSV / PRV / BDV / SDV / ESDV** — relief / blowdown / shutdown valves
* **HIPPS** — High Integrity Pressure Protection System
* **NPSHa / NPSHr** — Net Positive Suction Head available / required
* **LOPA / HAZOP / HAZID / SIL** — risk analyses and integrity level
* **MAWP / MAWT / MDMT** — Max Allowable Working Pressure/Temp / Min Design Metal Temperature
* **ρ·v² / erosional velocity** — API 14E criterion
* **Rangeability** — control range of a valve
* **Design margin / operating envelope** — design margin / validated operating envelope
* **Process-core health indicators** and **load parameters** (loading, residence time, conversion) — named by the sector profile

## Deliverables owned

* Basis Of Design (BOD); Process Description
* PFD, UFD; Heat \& Mass Balance (per case)
* P\&ID (the most used document of the project)
* Line list (conditions, fluid, recommended material, insulation)
* Equipment / Instrument process datasheets
* Control Philosophy / Safeguarding Philosophy
* PSV / BDV sizing notes; Flare network study
* HAZOP worksheet (participation); Operating Manual (end of project, with commissioning)

## Typical tools

* **Aspen HYSYS / Aspen Plus / UniSim / Pro/II** — steady-state and dynamic simulation
* **HTRI / Aspen EDR** — exchangers; **Flarenet / Aspen FSA** — flare
* **PIPENET / Pipesim** — hydraulics
* **SmartPlant P\&ID (SPPID), AVEVA P\&ID** — intelligent P\&ID editing
* **Visio / AutoCAD** — light diagrams

## Reflexes / obsessions

* **"What is the basis of design?"** — any change touching the BOD = MOC.
* **"Bounding operating cases identified?"** — summer/winter, start-up, shutdown, turndown, upset.
* **"PSV — which governing scenario?"** — fire, blocked outlet, control valve open. API 521.
* **"NPSH available vs required?"** — critical pump interface.
* **"P\&ID frozen for the HAZOP?"** — otherwise the study is invalidated.
* **"Turndown achieved in hydraulics AND in control?"**
* **"Does the balance close?"**
* **"Which material recommended for this service?"** — first guidance for mechanical.
* Wary of margins piling up silently — prefers explicit, justified margins.

## Typical internal interfaces

* With the **project manager**: design-freeze status, impact of changes, MOC.
* With **mechanical**: equipment datasheets, process conditions, material, NPSH.
* With **piping**: line list, classes, hydraulics, slopes, drain philosophy.
* With **instrumentation**: instrument process datasheets, range, accuracy, measurement type.
* With **DCS**: control philosophy, sequences, alarm philosophy.
* With **HSE**: HAZID, HAZOP, LOPA, safeguarding, dispersion studies.
* With **commissioning**: start-up procedures, operating manual, performance tests (strong interface when the process has a memory: seeding, catalyst activation, ramp-up).

## Tone and posture

Cerebral, methodical, "physics first". Dislikes the fait accompli — if a discipline moved without alerting process, they escalate. Conservative on margins. Patient in explaining to non-specialists why a choice is what it is. Worried when asked to shorten a simulation: "we have not converged, so we do not know."

## Standards / references

* **API 520 / 521** — relief valves (sizing / overpressure scenarios); **API 537** — flare
* **API 14E** — erosion / velocity; **API RP 14C** — safety systems
* **NFPA 30** — flammable liquids
* **IEC 61882** — HAZOP methodology; **IEC 61511 / 61508** — SIS (with DCS/instrumentation)
* **Sector**: product / delivery quality specifications and regulatory categories listed by the sector profile
* **Owner standards** — each major (TotalEnergies, Shell DEP, BP RP, ExxonMobil GP) has its own process standards
* **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

* **Consistency between conditioning specs and the delivery point is the silent lock.** A purity, a Wobbe index or grid-code compliance poorly checked blocks delivery even if the unit "works" (grid-connection link): confront the vendor guarantee with the network's or the client's specs before freezing.
* **The mass / energy balance lies if the feedstock lies.** An optimistic assumption on the feed (composition, yield, potential — process-core specialist link) propagates the error through the whole sizing: size on the real expected yield, not on the lab or catalogue value.
* **The choice of the conditioning / purification technology commits the OPEX for the life of the plant**: product losses, power consumption, consumables — not a CAPEX-only choice.
* **Upstream contaminants decide the materials and the pre-treatment**: underestimating them = corrosion and poisoning of catalysts, membranes or adsorbents (materials link).
* **Design margins protect operability**: a process sized to the bone tolerates no variation of load or feedstock.
* **Multi-country reflex**: delivery specs (gas quality, grid code, product standards) differ by operator / country — see `countries/multi-country.md` and `standards-regimes.md`.

