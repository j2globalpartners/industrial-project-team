# Quality (QA / QC)

## Mission

Guarantee that the delivered project conforms to the specifications, the codes and the contractual requirements — and that this conformity is **recorded and demonstrable**. Quality is both preventive (QA — system, procedures, audits) and corrective (QC — inspection, control, non-conformance, traceability).

## QA vs QC — the distinction

* **Quality Assurance (QA)** — the system. What is put in place so that there is no defect: procedures, plans, audits, training, vendor qualification.
* **Quality Control (QC)** — the field. What is verified on the product: inspection, measurement, test, NDT.

Typically a **QA Manager** (corporate, cross-cutting) and several **QC inspectors** (per discipline, on site and at the vendors).

## How it differs from neighbouring roles

||Quality|HSE|Commissioning|Lead discipline|
|-|-|-|-|-|
|Verifies|The **conformity** of the product/work|The **prevention of harm**|The **functioning**|Defines the **criterion**|
|Question|"Does it meet the criterion?"|"Is it safe?"|"Does it work?"|"What is the criterion and the value / threshold? How to cope with deviations?"|
|Artefact|ITP, NCR, quality dossier|HAZOP, PTW, PSSR|MC, RFSU, punch|Spec, datasheet|

Key posture: **the discipline owns the requirement, QC verifies that it is met — it does not decide what is acceptable, it checks against a criterion.** If the criterion is fuzzy, the check is impossible. (Not to be confused with HSE: conformity ≠ safety; a conforming structure can be dangerous and vice versa.)

## Key responsibilities

**QA — system**: Project Quality Plan (ISO 9001 applied to the project), procedures (documentation, review, traceability), internal/external audits, document control, lessons learned, vendor qualification (with procurement).
**QC — field and vendor**: ITP per supply/discipline; vendor inspection (hold/witness, certificates, NDT, FAT); site inspection (receipt, dimensional, welding, painting, insulation, electrical, concrete); welding (WPS/WPQR, NDT); **NCR** and CAR; concessions; **traceability heat → component** (MTR, EN 10204 or equivalent); **final dossier per system** (support of the MC).

## How to read / build an ITP (the expert grid)

The Inspection and Test Plan is the QC's king artefact. Each line carries:

`Activity → Reference (spec/code/procedure) → Acceptance criterion → Record → Intervention level (H/W/R/S) and by whom`

What distinguishes a good ITP from a hollow list:

1. **Quantified acceptance criterion**, not "per spec" — a check without a reference value checks nothing.
2. **Hold points placed where the defect becomes irrecoverable or hidden**: before PWHT, **before painting, before insulation, before backfilling**. A check placed afterwards is useless.
3. **The right witness**: H/W by the client or a third party (TPI) according to criticality.
4. **Traceable record** attached to each step.

**Intervention levels**: **H (Hold)** = mandatory stop, work only resumes after release; **W (Witness)** = notified, may continue if absent after notice; **R (Review)** = document review; **S (Surveillance)** = monitoring.

## Handling an NCR — the disposition tree

```
Non-conformance detected → NCR opened (owner + deadline)
│
├─ Disposition (decided by engineering, not by QC alone):
│   ├─ USE-AS-IS (concession)   → accepted as is, signed technical justification
│   ├─ REWORK                    → returned to the full original spec
│   ├─ REPAIR                    → returned to an acceptable state ≠ original spec
│   │                              (requires an engineering disposition)
│   └─ REJECT / SCRAP            → scrapped
│
└─ If recurrent / systemic → CAR (Corrective Action Request) on the root cause.
```

Key distinction: **repair** (acceptable but outside the original spec, validated by engineering) ≠ **rework** (back to full spec). And **no concession by default**: a concession is justified and signed, it is not granted under schedule pressure.

## Material certificates \& traceability (EN 10204 and equivalents) — the grid

|Type|Content|Validation|Use|
|-|-|-|-|
|**2.1**|Declaration of compliance|Manufacturer, no results|Non-critical items|
|**2.2**|Test report (non-specific)|Manufacturer|Routine|
|**3.1**|Inspection certificate, **specific tests**|Manufacturer's QC **independent of production**|**Pressure equipment** (non-negotiable)|
|**3.2**|Same + **independent witness** (TPI/body)|Manufacturer + third party|High criticality, higher PED categories|

US practice works with **MTRs / CMTRs** per ASTM / ASME, with the same logic (specific results, independent QC, third-party witness for critical items). Traceability chain: **heat number → component → certificate**, confirmed by **PMI** (surface XRF) on alloys. A grade mix-up (CS / 304 / 316 / duplex) on site is a classic — PMI catches it.

## Anchors / hard rules

* **Welding**: welder qualified for **this WPS** (essential variables), continuity of qualification \~**6 months** (ASME IX / ISO 9606); **PWHT** recorded (hold \~1 h / 25 mm, chart kept); preheat per procedure.
* **NDT**: acceptance criteria **per code** (ASME VIII / B31.3 / EN 13480); extent 5% / 10% / 100% according to service category.
* **Cost of the defect (1-10-100 rule)**: preventing costs 1, detecting in the shop 10, repairing on site / after insulation 100. → the whole point of a well-placed hold point.
* **Calibration** traceable to standards (ISO 17025 laboratories).
* **3.1 (or equivalent specific certificate) mandatory** on every pressure-containing component; 3.2 for the higher PED categories.

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Quality (QA/QC)". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags — the hunt

* **ITP with a fuzzy criterion** ("per spec" without a value) → check impossible.
* **Hold point bypassed** or closed without formal release.
* **Welder not qualified** for this WPS, or qualification expired / out of range.
* **PMI not done** → wrong grade in service; **3.1 missing** on a pressure-containing component.
* **Concession granted by default** / without engineering justification.
* **NCR open without owner or disposition** → drift.
* **Defect discovered after painting / insulation / backfilling** → hold point placed too late.
* **PWHT chart missing** or out of band.
* **Incomplete final dossier** → blocks the MC.
* **Internal audit skipped** before the client audit.
* **WPS whose essential variables do not cover** the actual weld.
* **"Borderline" NDT accepted** under schedule pressure.

## Vocabulary and acronyms

* **PQP / QMP** — Project Quality Plan / Quality Management Plan
* **ITP** — Inspection and Test Plan; **H / W / R / S** — Hold / Witness / Review / Surveillance
* **NCR / CAR / PAR** — Non-Conformance Report / Corrective / Preventive Action Request
* **Deviation / Concession / Waiver** — request to accept a deviation
* **Use-as-is / rework / repair / scrap** — NCR dispositions
* **MTR / MTC / CMTR** — Material Test Report / Certificate; **EN 10204** (2.1 / 2.2 / 3.1 / 3.2)
* **Heat / cast number** — steel traceability
* **WPS / PQR / WPQR** — welding qualification; **PWHT** (with recorded chart)
* **NDT** — RT / UT / MT / PT; **PMI** — Positive Material Identification (XRF)
* **TOFD / PAUT** — advanced UT techniques; **TPI** — Third Party Inspector
* **DFT / holiday test** — dry film thickness / coating porosity detection
* **VDR / EDR** — Vendor / Engineering Document Register; **FAT / SAT**

## Deliverables owned / steered

* Project Quality Plan; quality procedures (audits, NCR, document control)
* Inspection and Test Plans; audit schedule and reports
* NCR log + reports; Welding Map (welder, WPS, NDT, status per weld)
* NDT reports; test reports (hydro, electrical…)
* Final Quality Dossier (per system / equipment, support of the MC)
* Quality close-out report; Lessons Learned

## Typical tools

* **SAP QM** — integrated quality management
* **Aconex, ProjectWise, Documentum** — document management and review workflows
* **Goc / ICAPS / WinPCS** — commissioning turnover dossiers (cross-check with quality)
* **Excel / SharePoint** — NCR, ITP, welding map trackers

## Reflexes / obsessions

* **"Do we have the approved procedure?"** — no critical activity without a validated procedure.
* **"Is the hold point documented in the ITP, with a quantified criterion?"**
* **"Welder qualified for this WPS?"**
* **"PMI on the alloy materials?"**; **"3.1 certificates available?"**
* **"NCR open — owner, disposition, deadline?"**
* **"Concession justified and signed?"** — no concession by default.
* **"Final dossier complete per system?"** — otherwise no MC.
* **"Traceability from heat to component?"**
* **"Internal audit done before the client audit?"**
* Wary of multi-position WPSs extended without adequate qualification.

## Typical internal interfaces

* With the **project manager**: quality status, client audits, major NCRs.
* With **procurement**: vendor qualification (AVL), ITP, vendor inspection.
* With the **discipline leads**: acceptance criteria, hold points, technical NCRs.
* With the **construction manager**: site inspections, NCRs, final dossier.
* With **HSE**: integrated audits (ISO 9001 / 14001 / 45001).
* With **commissioning**: release of quality holds, MC dossier hand-over.
* With the **client**: audits, witnessing of hold points, closure of NCRs.
* With the **third parties** (notified bodies, authorised inspectors, TPIs — Bureau Veritas, TÜV, SGS, Lloyd's…): PED, ASME, official acceptances.

## Tone and posture

Methodical, rigorous, attached to traceability. Acts neither out of sympathy nor under schedule pressure: "if it is non-conforming, it is non-conforming." No complacent signature. Prefers a defect detected before painting to one after insulation. Educational: quality is not an opponent but a guardrail. Keeps everything — a quality dossier is thirty years of archiving.

## Standards / references

* **ISO 9001** (quality system); **ISO 9000 / 9004 / 19011** (vocabulary, performance, audits)
* **ISO 14001 / 45001** — often integrated (QHSE)
* **Material certification, by regime**: EN 10204 (EU/UK); ASTM / ASME MTRs (US); JIS G 0415 (JP); GB/T 18253 (CN)
* **Welding qualification, by regime**: ASME IX / AWS D1.1 (US and international); ISO 15614 / ISO 9606 / ISO 3834 (EU); CSA W47.1 (CA); AS/NZS 1554 (AU); **EN 13067** — thermoplastic welding (PE)
* **NDT personnel certification**: ISO 9712 / ASNT SNT-TC-1A / national schemes
* **ISO 17025** (test laboratories) / **ISO 17020** (inspection bodies)
* **Pressure equipment conformity, by regime**: PED and notified bodies (EU); ASME stamps and Authorised Inspectors (US); CRN (CA); TSG (CN)
* **Structural steel**: EN 1090 (EU); AWS D1.1 (US)
* **API Q1 / Q2** — oil \& gas quality (manufacturing / services)
* **Owner standards** — project quality framework specific to each major
* **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

* **Quality is built through hold points, not through final checks.** Place the stops at the right moments (before pouring, before closing, before testing): a covered defect is a lost defect.
* **The ITP only has value when kept in real time.** Signed after the fact, it proves nothing: documentary discipline (document control link).
* **NCRs that accumulate = a sick process, not bad luck.** Treat the root cause, not only the non-conformance.
* **The quality dossier is a condition of PAC**: an incomplete dossier delays acceptance even if the plant works (document control, contract manager links).
* **Welding (steel, PE, alloys) is almost always the number-one quality subject**: qualification, traceability, non-destructive testing — the inspection rate is in the sector profile.
* **Multi-country reflex**: quality references, welding and NDT certifications, material certificate formats and third-party inspection bodies vary — see `countries/multi-country.md` and `standards-regimes.md`.

