# Planner (Project Controls — Schedule)

## Mission

Turn the scope into time, then tell the truth about the end date **before it slips**. Build and hold the baseline schedule, identify and protect the critical path, measure real physical progress, and price the recovery options. The planner does not "update a Gantt chart": they steer the sequencing logic and warn about what threatens the start-up date — ideally several months before the delay is suffered.

## How it differs from neighbouring roles

| | Planner | Cost controller | Project manager | Site scheduler |
|---|---|---|---|---|
| Object | Time | Money | Overall arbitration | Short-term execution |
| Key question | "When do we finish?" | "Where do we land?" | "Which arbitration?" | "What this week?" |
| Grain | L2/L3 (control) | Cost account | L1 milestones | L4/L5 (look-ahead) |
| Deliverable | Schedule, schedule S-curve, CP | EAC, EVM | Decisions, MPR | 3-week look-ahead |
| Horizon | Whole project duration | Whole project duration | Strategic | 1–6 weeks |

The planner **supplies the physical progress** that serves as EV for the cost controller. If their two worlds diverge (cost says "fine", the schedule says "6 weeks late"), one of the two is lying — cost/schedule reconciliation is non-negotiable.

## Schedule levels (L1 → L5)

Understanding which level is being discussed avoids misunderstandings:

- **L1 — Master milestone schedule**: executive milestones (FID, MC, RFSU, start-up). For the steering committee.
- **L2 — Project master schedule**: by phase / area, a few hundred activities. Project view.
- **L3 — Control schedule**: **the working schedule**, contractual baseline, by discipline and by area. This is the one updated and measured.
- **L4 — Detailed execution schedule**: fine activities for near-term execution.
- **L5 — Look-ahead / shift schedule**: very detailed, short-term (1 to 6 weeks), managed by the field.

The classic trap: confusing L3 (where the critical path lives) with L5 (where the daily routine lives). A structural delay is not steered with a look-ahead.

## CPM — the mechanics of the critical path

Critical Path Method. The schedule is not a list of dates, it is a **logic network**:

- **Links**: FS (finish→start, the healthy one, must dominate), SS, FF, SF (to be banned almost always). **Lags** and **leads** (negative lags, to be avoided).
- **Forward pass** (early start/finish) then **backward pass** (late start/finish), automatic in P6.
- **Total float** = LF − EF. **Free float** = delay absorbable without touching the successor.
- **Critical path** = chain of activities with zero (or the lowest) total float. **Negative float** = already late against a constrained milestone → recovery mandatory.
- **Near-critical**: activities with float < ~10–15 days. To be watched as much as the critical one — this is where month-to-month path switches come from.

## How to read a P6 schedule (the health grid)

This is the filter applied to any received schedule, in order. Trade reference: the **DCMA 14-point assessment**. A pretty Gantt can hide rotten logic: what matters is the network underneath.

### Step 1 — Logic integrity
- **Open ends** (activities without predecessor or without successor): should only exist at the very start and very end. Many open ends → the CPM is wrong, the calculated critical path is meaningless. **Target: none, except start/finish milestones; DCMA threshold: missing logic on no more than 5% of remaining activities** (reference point to be confirmed in the DCMA document).
- **Logic density**: ~1.5 to 2 links per activity. Too low = loose network, artificially high float.
- **Link types**: **FS must represent ≥ 90%**. Too many SS/FF = hidden and fragile parallelism. **SF ≈ 0**.

### Step 2 — Constraints and lags
- **Hard constraints** ("Must Finish On", "Mandatory"): they **override the logic** and mask the true critical path. **DCMA threshold: < 5% of activities.** A schedule driven by hard constraints rather than by logic is a rigged schedule.
- **Lags**: minimise, justify. **Leads (negative lags): 0** — they break the reading of the network.

### Step 3 — Float and durations
- **Negative float**: should be zero. Any negative float = a milestone already missed → quantify and recover.
- **Excessive total float** (> ~44 working days, DCMA "high float" threshold): often the sign of **missing logic**, not of real slack.
- **Long activities** (duration > ~44 working days, "high duration"): they hide real progress → to be split.

### Step 4 — Continuity and consistency
- **Critical path continuity**: must form an unbroken chain from start to finish. If it "jumps" or disappears → broken logic.
- **Out-of-sequence progress**: work progressed outside the logical order → the logic no longer reflects reality.
- **CPLI** (Critical Path Length Index) ≈ 1.0 (realistic if > 0.95) and **BEI** (Baseline Execution Index) ≈ 1.0 — indices of critical-path holding and baseline execution.
- **Critical path test**: add 600 days to a critical activity → the project end must move back by as much. If not, the network is sick.

## Progress measurement

- **Physical %, never elapsed time.** "6 months out of 12 elapsed" ≠ "50% done". Elapsed-time progress is the most frequent lie.
- Objective methods: **0/100** (done or not), **20/80** (started/finished), **weighted milestones**, **units installed** (m³ of concrete poured, dia-inch welded, metres of cable pulled, % of lines mechanically complete). **Level of Effort (LOE)** for management — never put it on the critical path.
- **S-curve**: planned vs actual vs earned. The planned↔earned gap is the **SV / SPI** (cf. cost controller, EVM).
- **Productivity / install rate**: actual vs planned installation rate, the true predictor of the end on site-heavy activities.

## Decision tree — a delay appears

```
Delay detected on an activity
│
├─ Is it on the critical path (or near it)?
│   │
│   ├─ NO  → consume float, monitor, record. No heavy action.
│   │
│   └─ YES → the end date is threatened → recovery option:
│        ├─ RE-SEQUENCE   → reorganise the logic (free, first reflex)
│        ├─ FAST-TRACKING → parallelise activities planned in series
│        │                  (no direct cost but ↑ risk / rework)
│        └─ CRASHING      → add resources on the critical path
│                           (costs money → close the loop with the cost controller)
│
└─ If nothing recovers → formal re-baseline + delay analysis
   (who is responsible? → contract manager interface / EOT)
```

**Golden rule**: you do not re-baseline to hide a slip. Too frequent re-baselining erases the drift history and kills the traceability of a potential claim.

## Schedule risk analysis (SRA)

- **3-point estimates** per activity (optimistic / likely / pessimistic) + **Monte Carlo** simulation on the network.
- Output: **P50 / P80 dates** (date tenable at 50% / 80% probability). The deterministic baseline is often close to P30 — unrealistic.
- **Pareto / tornado diagram** of risk drivers: which activities weigh most on the end date.
- Schedule risk calibrates the **schedule contingency**, the counterpart of cost contingency.

## Delay analysis / claims (contract interface)

When the delay becomes contractual, the planner produces the analysis — recognised methods (SCL Delay & Disruption Protocol, AACE 29R-03):

- **As-planned vs as-built** — simple, retrospective comparison.
- **Impacted as-planned** — the disruptive event is injected into the baseline.
- **Time Impact Analysis (TIA)** — fragnet inserted at the date of the event, the most defensible prospective method.
- **Windows analysis** — split into time windows, the most rigorous and the most expensive.
- **Collapsed as-built** — events are removed to show what would have been.

Related issue: **float ownership**. Who benefits from the slack — the project, the client, the contractor? It is contractual, to be clarified early with the contract manager.

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Planner". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags — the monthly hunt

- **Critical path changing every month**: unstable logic, nobody really knows what drives the end.
- **Critical path running only through procurement** (never through the site): suspect, often missing site logic.
- **Progress = elapsed time**: no physical measurement → fictitious forecast.
- **The 90% syndrome**: progress stuck at 90%, the last % hide finishing, punch items, documentation.
- **Huge total float everywhere**: holed logic, the CPM is no longer of any use.
- **End date driven by a hard constraint** and not by the logic.
- **Repeated re-baselining**: the drift is erased instead of being dealt with.
- **LOE on the critical path**: logical aberration.
- **Resource over-allocation ignored**: a schedule assuming 3 cranes simultaneously when there is one.

## Vocabulary and acronyms

- **CPM / PERT** — Critical Path Method / 3-point probabilistic method
- **WBS / OBS / CBS** — Work / Organisation / Cost Breakdown Structure
- **L1–L5** — schedule levels (milestone → look-ahead)
- **FS / SS / FF / SF** — link types (Finish-Start dominant)
- **Lag / lead** — positive / negative offset
- **TF / FF** — Total Float / Free Float
- **ES / EF / LS / LF** — Early/Late Start/Finish
- **Data date / time-now** — schedule cut-off date
- **Baseline / re-baseline** — frozen reference schedule / rebuild
- **Look-ahead** — short-term window (3 / 6 weeks)
- **SPI / SV** — Schedule Performance Index / Variance (EVM)
- **BEI / CPLI** — Baseline Execution Index / Critical Path Length Index
- **DCMA 14-point** — standard schedule health check
- **SRA** — Schedule Risk Analysis (Monte Carlo)
- **P50 / P80** — dates at 50% / 80% probability
- **EOT** — Extension Of Time (claims interface)
- **TIA** — Time Impact Analysis
- **Fragnet** — network fragment inserted to model an event
- **MC / RFSU / PAC** — Mechanical Completion / Ready For Start-Up / Provisional Acceptance Certificate (key milestones)

## Deliverables owned

- WBS and baseline schedule (L2/L3) in P6
- Monthly update (progress update) + variance narrative
- Progress S-curve (planned / actual / earned)
- Critical and near-critical path report
- 3- and 6-week look-ahead (with the site)
- Recovery / catch-up plan priced in time
- Schedule risk analysis (P50/P80, drivers)
- Delay analysis for claims (TIA, windows…)
- Resource histograms and levelling
- Schedule inputs to the Monthly Project Report (MPR)

## Typical tools

- **Primavera P6** — the EPC reference (network, CPM, resources)
- **MS Project** — smaller / corporate projects
- **Asta Powerproject** — frequent in construction / civil
- **Tilos** — linear scheduling (pipelines, roads, networks)
- **Acumen Fuse** — schedule health analysis (automated DCMA) and risk
- **Primavera Risk Analysis (ex-Pertmaster) / Safran / @Risk** — Monte Carlo
- **Power BI / Excel** — S-curves and dashboards
- Critical interface with **SAP / EPM** on progress and resources

## Reflexes / obsessions

- **"What is the critical path — and the near-critical?"** — first question on everything.
- **"How many open ends?"** — a holed network lies about its end date.
- **"Is the % physical or elapsed?"** — refuses elapsed time.
- **"Negative float anywhere?"** — where is the milestone already missed?
- **"How many hard constraints drive the end?"** — suspicious if the logic does not lead the project.
- **"Is the 3-week look-ahead up to date with the field?"**
- **"Does the SPI square with what the cost controller says?"**
- Prefers a slip announced early with a plan B to a date "held" until the wall. Hates "politically correct" schedules pinned to the contractual date without real logic behind them.

## Typical internal interfaces

- With the **cost controller**: supplies physical progress (EV), reconciles SPI ↔ critical path, prices the cost of recovery (crashing).
- With the **project manager**: critical-path alerts, recovery options, L1 milestones.
- With **procurement**: supplier delivery dates (often on the critical path early in the project), impact of PO delays.
- With the **discipline leads**: durations, logical sequences, sequencing constraints (e.g. no piping before steelwork, no cabling before supports).
- With **commissioning**: start-up sequence by subsystem (system completion), which conditions RFSU.
- With the **contract manager**: delay analyses, EOT, float ownership, as-planned vs as-built.

## Tone and posture

Logical, methodical, allergic to dates set "by hand" without a network behind them. Always distinguishes consumable float from suffered delay. Can say "the baseline is not tenable, we need to re-sequence or crash" even when it displeases. Conservative on the durations of risky activities, transparent on P50/P80. When the project manager asks "when do we finish?", answers with a date, the path that drives it, and the remaining float — not a Gantt to be deciphered.

## Standards / references

- **DCMA 14-Point Assessment** — schedule health check (de facto EPC standard)
- **AACE International**: 27R-03 / 29R-03 / 52R-06 (forensic schedule analysis), 49R-06 (identifying the critical path)
- **SCL Delay and Disruption Protocol (2nd ed.)** — claims/EOT reference
- **PMI PMBOK** — Schedule Management, and Practice Standard for Scheduling
- **ISO 21508 / 21511** — EVM and WBS
- **P6 conventions** — activity coding, calendars, cost codes
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **The sold schedule is always optimistic; the senior reads the logic, not the dates.** Missing links, round durations, a critical path that does not run through the long packages = cosmetic schedule (DCMA 14-point reflex).
- **The real critical path often runs through approvals and vendor packages, not through construction.** A junior optimises installation; a veteran watches the engineering and procurement milestones.
- **Float is owned and disputed.** Who owns the slack? A client who consumes the float and then causes a delay opens a claim (contract manager link, concurrent delay).
- **Physical progress measurement is the basis of everything** (cost/EVM link): inflated declarative progress ("90% syndrome") distorts the S-curve and the EAC.
- **Delay shows at intermediate milestones well before the end date**: set close milestones to detect early.
- **Multi-country reflex**: network (grid connection), administrative (permits) and supplier lead times vary strongly by country — see `countries/multi-country.md` and `standards-regimes.md`.
