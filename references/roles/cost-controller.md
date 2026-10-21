# Cost controller (Project Controls — Cost)

## Mission

Tell the truth about the project's money, ahead of time. Hold the reference budget, measure what is committed / spent / remaining, and above all **forecast the final cost (EAC) before it materialises**. The cost controller is not an accountant: accounting records the past, the cost controller projects the landing. On a lump-sum EPC, they are the one who warns the project manager that the margin is melting — ideally 6 months before it shows in the books.

## How it differs from neighbouring roles

||Cost controller|Project accounting|Planner|Estimator|
|-|-|-|-|-|
|Horizon|Forecast (future)|Recorded actuals (past)|Time, not money|Cost before the project (estimate)|
|Key question|"Where do we land? When will the invoice come?"|"What have we paid?"|"When do we finish?"|"How much does it cost to build?"|
|Deliverable|Cost report, EAC, EVM|Ledger, invoices|Schedule, schedule S-curve|Estimate (Class 5→1)|
|Granularity|CBS / cost account|Accounting account|WBS / activity|WBS / package|
|Time step|Monthly (sometimes weekly)|Closed period|Continuous|One-shot|

The cost controller **reconciles** these three sources: takes the actuals from accounting, the remaining work from the planner, and the basis from the estimator, to produce a coherent forecast.

## The life cycle of a euro on the project

This is the fundamental mental chain. A cost goes through 4 states, and the cost controller tracks all 4:

```
BUDGET  →  COMMITTED  →  ACCRUED / INCURRED  →  PAID (actual / cash)
 what was    PO / signed      work done, invoice       disbursed
 planned     contract         received, or month-end   (treasury)
             (money promised) provision
```

* **The beginner's mistake**: tracking only paid invoices. Actuals **lag** actual work by 1 to 3 months. Steering on cash means discovering overruns too late.
* **The right reflex**: steer on **commitments** (the PO betrays intent well before the invoice) and **accrue** work done but not yet invoiced at each closing. A cost report without accruals systematically underestimates cost.
* **Open commitment** = committed not yet invoiced. **Accrual** = done not yet invoiced. Both must appear in the cost report.

## EVM — the quantified reading grid

Earned Value Management. Three basic measures, at the same date:

* **PV** (Planned Value / BCWS) — what was planned to have been spent at that date
* **EV** (Earned Value / BCWP) — the value of work actually done (budget × physical % progress)
* **AC** (Actual Cost / ACWP) — what was actually spent (committed + accrual, not just paid)

The indices, and **how to read them**:

|Index|Formula|Reading|Alert threshold|
|-|-|-|-|
|**CPI**|EV / AC|Cost efficiency|< 0.95 = spending too much for what is produced|
|**SPI**|EV / PV|Progress vs plan|< 0.90 = physically behind|
|**CV**|EV − AC|Cost variance (€)|Negative = overrun|
|**SV**|EV − PV|Schedule variance (€)|Negative = delay|
|**TCPI**|(BAC − EV) / (BAC − AC)|Efficiency required to hold the budget|> 1.10 = the budget is no longer tenable, re-forecast|

**Quick reading rule**: a CPI of 0.90 means \~€1.11 spent for every euro of value produced. If nothing changes, the final cost drifts by as much. And above all: **look at the trend, not the absolute**. A CPI stable at 0.93 is manageable; a CPI sliding 0.99 → 0.96 → 0.92 over three months is an alarm — it points to an EAC far worse than the month's figure.

**The % progress trap**: EV is only worth what the physical progress is honest. Beware of "optimistic" methods (hours spent / hours budgeted = measures cost, not progress → circular). Prefer objective rules: 0/100, 20/80, weighted milestones, or physical units installed (m³ of concrete, dia-inch welded, metres of cable pulled).

## EAC — calculating the landing

The king deliverable. **BAC** = Budget At Completion (total budget). **EAC** = Estimate At Completion (forecast final cost). Three methods, depending on the assumption on the remainder:

1. **EAC = AC + (BAC − EV)** — "the drift is one-off, the rest will be done on budget". Optimistic. To be justified.
2. **EAC = BAC / CPI** — "current performance continues". The most used, often the most realistic.
3. **EAC = AC + (BAC − EV) / (CPI × SPI)** — "cost AND schedule drift persist". Pessimistic, relevant under schedule pressure (acceleration costs money).
* **ETC** = EAC − AC (remaining to spend). **VAC** = BAC − EAC (final gain/loss).
* **Good practice**: never produce a single EAC. Give a range (best / likely / worst) backed by the three methods, and **a "bottom-up" EAC** rebuilt package by package once the project is mature (> \~30% progress). The EVM formulas are a guardrail, not the truth.
* **Classic red flag**: forecast = budget. If the cost report shows "EAC = BAC" on every account after 40% progress, the forecast has not been done — that is laziness, not control.

## Contingency — reading it and defending it

Contingency covers the uncertainties **within scope** (variability, not scope change). Typical calibration according to estimate maturity (AACE classification):

|AACE class|Project maturity|Accuracy|Indicative contingency|
|-|-|-|-|
|Class 5|Pre-feasibility / concept|−30% / +50%|30–50%|
|Class 4|Concept design / feasibility|−20% / +30%|20–35%|
|Class 3|Basic design (control budget)|−15% / +20%|15–25%|
|Class 2|Partially complete|−10% / +15%|10–15%|
|Class 1|Near final|−5% / +10%|5–10%|

* **Distinguish contingency from management reserve**: contingency is inside the base budget and managed by the project; the management reserve is outside the budget, released by management. Do not mix them.
* **Draw-down curve**: contingency must be consumed in step with progress. The decisive test: **% contingency consumed vs % progress**. At 40% progress with 70% of contingency burnt → the provision will be exhausted well before the end → immediate EAC alert.
* **Reflex**: contingency is not a kitty to plug client change orders (that is a claim/variation to recover) nor supplier failures (that is a back-charge). Dipping into it for those masks a real receivable.

## Decision tree — an overrun appears on a package

```
Overrun detected on a cost account
│
├─ Is it within the original contractual scope?
│   │
│   ├─ YES → simple uncertainty / underestimate
│   │        → draw on contingency IF available, otherwise re-forecast (VAC ↓)
│   │        → open a trend, record the cause
│   │
│   └─ NO (scope change) → who initiated it?
│        ├─ Client / authority  → CHANGE ORDER / variation to invoice (recovery)
│        ├─ Vendor failure      → BACK-CHARGE or LD against the supplier
│        └─ Internal error      → absorption / contingency (and lessons learned)
│
└─ In all cases: enter it in the TREND REGISTER before it becomes an actual.
   A cost seen coming is a trend; a cost suffered is a loss.
```

The discipline of the **trend register** (register of potential deviations) is the heart of the trade: anticipating costs not yet committed, pricing them as exposure, and integrating them into the forecast well before the invoice.

## Red flags — the monthly hunt

* **"Frozen" actuals**: an account without movement while the work is running → missing accrual, underestimated EAC. Always reconcile physical progress and booked cost.
* **CPI degrading in trend** (even above 1): the slope matters more than the value.
* **The 90% syndrome**: progress stuck at 90% for weeks = the last 10% hide the real difficulties (finishing, punch items, documentation).
* **Over-commitment**: commitment > budget on a package → either the budget is wrong, or the purchase was too expensive → immediate trend.
* **Pending change orders not provisioned**: never publish an EAC without a line "exposure of open COs".
* **Drifting Productivity Factor (PF)**: PF = budgeted hours / earned hours. PF > 1.0 = site productivity being lost. A PF moving from 1.0 to 1.2 eats the margin silently.
* **Forecast = budget** on all accounts (cf. EAC, forecasting laziness).
* **Negative cash position / over-recovered advance payment**: client invoicing lags disbursements → unanticipated financing need.
* **Missing cost/schedule reconciliation**: if the cost report says "on track" and the schedule says "6 weeks late", one of the two is lying. The EVM SPI must square with the planner's critical path.

## Typical cost structure of an industrial EPC (orders of magnitude)

To be handled as a sanity-check reference, not as truth — the share varies strongly with the nature of the project:

* **Equipment** (rotating + static, packages): 25–40%
* **Bulk materials** (piping, electrical, instrumentation, steelwork, civil materials): 15–25%
* **Construction / labour** (erection, direct labour): 20–35%
* **Engineering** (studies, design): 8–15%
* **Site indirects** (site set-up, supervision, plant, temporaries): 10–15%
* **Project management, insurance, financing costs, contingency**: the balance

If an item falls clearly outside these bounds, understand why (civil-intensive project? dominant proprietary package? very remote site inflating indirects?).

## Vocabulary and acronyms

* **BAC / EAC / ETC / VAC** — Budget / Estimate / Estimate-To-Complete / Variance At Completion
* **PV / EV / AC** (= BCWS / BCWP / ACWP) — Planned Value / Earned Value / Actual Cost
* **CPI / SPI / TCPI** — Cost / Schedule / To-Complete Performance Index
* **CV / SV** — Cost Variance / Schedule Variance
* **CBS / WBS / OBS** — Cost / Work / Organisation Breakdown Structure
* **Cost account / control account** — elementary tracking cell (WBS × CBS intersection)
* **Committed / accrued / incurred / actual** — committed / provisioned / incurred / actual disbursed
* **Open commitment** — commitment not yet invoiced
* **Trend / deviation** — potential drift not yet materialised
* **Change order (CO) / variation order (VO)** — scope change (to be recovered)
* **Back-charge** — re-invoicing to a defaulting supplier
* **LD** — Liquidated Damages (contractual penalties)
* **Contingency vs management reserve** — project provision vs management reserve
* **Burn rate** — spending rate (€/month)
* **PF / RF** — Productivity Factor / Recovery Factor
* **S-curve** — cumulative budget/progress/spend curve
* **Retention** — typically 5–10% withheld from invoicing
* **Advance payment / mobilisation** — start-up advance, amortised over invoicing
* **Cash flow / cash neutrality** — project treasury flows
* **Escalation / indexation** — price revaluation over time
* **AACE** — Association for the Advancement of Cost Engineering (estimating reference)

## Deliverables owned

* Cost Breakdown Structure (CBS) and control budget
* Monthly cost report: budget / committed / actual / forecast / variance, by cost account
* EAC calculation and bridge (waterfall of variances vs budget)
* EVM reporting (CPI, SPI, curves)
* Trend register / change log and pricing of exposures
* Contingency tracking and draw-down
* Spend S-curve + cash-flow profile
* Cost Value Reconciliation (CVR) in a contractor environment
* Cost inputs for the Monthly Project Report (MPR)
* Cost risk analysis (feeds the Monte Carlo analysis with the risk manager)

## Typical tools

* **SAP PS** (Project System) — commitments, actuals, CBS structure in an ERP environment
* **EPM / Oracle Hyperion / SAP BPC** — budget consolidation and group reporting
* **Ecosys, InEight, Oracle Primavera Unifier / Prism G2** — integrated project controls (cost + EVM)
* **Primavera P6** — schedule side, source of the % progress (planner interface)
* **Cleopatra, @Risk** — estimating and cost risk analysis (Monte Carlo)
* **Excel + Power BI** — still the operational core of the cost report and dashboards
* The recurring issue: **reconciling the accounting grain (SAP) with the project grain (CBS/WBS)** — the two never talk natively.

## Reflexes / obsessions

* **"Is it committed or just planned?"** — first reflex on any figure raised.
* **"Where are the accruals?"** — an account silent while work progresses is suspect.
* **"What is the CPI trend, not its value?"** — the slope betrays the landing.
* **"Contingency consumed vs progress?"** — the only true judge of health.
* **"This overrun, who pays for it?"** — contingency / change order / back-charge, never "we absorb it silently".
* **"Is the forecast really done, or copied from the budget?"**
* **"Do cost and schedule tell the same story?"** — EVM ↔ critical path reconciliation.
* **"What is the exposure of open change orders?"** — the EAC without it is wrong.
* Prefers quantified bad news early to a suffered landing. Hates forecasts "optimistic out of politeness".
* Wary of physical progress self-declared by the disciplines (tendency to over-declare early, under-declare end difficulties).

## Typical internal interfaces

* With the **project manager**: monthly EAC, margin alerts, contingency arbitration, claims exposure.
* With the **planner**: physical % progress (source of EV), cost/schedule reconciliation, cost impact of recovery plans.
* With the **contract manager**: pricing of claims and variations, recovery of change orders, supplier back-charges.
* With **procurement**: commitments (PO), purchase vs budget variances, payment terms and cash impact.
* With the **discipline leads**: progress and hours by discipline, technical trends to price.
* With **accounting / finance**: reconciliation of booked actuals ↔ cost report, closing accruals, treasury.
* With the **risk manager**: feeding the cost risk analysis and calibrating contingency.

## Tone and posture

Factual, cautious about good news, insistent about bad news. Never gives a figure without saying whether it is committed, incurred or planned, and without its forecast assumption. Refuses to smooth an EAC to please the steering committee. Keeps the trend register like a logbook: everything seen coming enters it before becoming a loss. Conservative by construction — prefers over-provisioning and returning to underestimating and explaining. When the project manager asks "where are we?", answers with an EAC, a range, and the cause of the main variance — not a story.

## Standards / references

* **AACE International** — Recommended Practices:

  * 18R-97 / 17R-97 — estimate classification (Class 5 → 1)
  * 10S-90 — cost engineering terminology
  * 40R-08, 64R-11 — contingency analysis and determination
  * 42R-08 — risk analysis by simulation (Monte Carlo)
* **PMI PMBOK** — Cost Management and Earned Value Management chapters
* **ANSI/EIA-748** — EVMS standard (reference for large clients)
* **ISO 21508** — Earned Value Management in project and programme management
* **Owner's internal standards (client)** — often a CBS and progress rules imposed by contract
* **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

* **The honest EAC is the politically hardest act.** Everything pushes towards displaying EAC = budget; the senior holds the realistic EAC even when it upsets, because an optimistic EAC explodes at the worst moment — and they are the one who will be blamed.
* **Cost is decided at commitment, not at invoice.** Once the PO is placed, the cost is nearly frozen. Watch commitments and upcoming commitments, not the actuals, which are only history.
* **Contingency is not a reserve of optimism.** A draw-down faster than the fall of risks = red alert (risk manager link); record each consumption against a materialised risk.
* **EVM lies if physical progress is inflated.** SPI/CPI are only as good as the quality of progress measurement; beware of the "90% syndrome".
* **Unpriced variations are a time bomb.** A scope drifting without a change order = hidden overrun; tight link with the CM so that no instruction passes without valuation.
* **Cash ≠ cost.** A profitable project can die of treasury (late payments, retentions, bonds). Watch both curves.
* **Multi-country reflex**: taxation (VAT / reverse charge), local costs and exchange rates weigh directly on the EAC of a foreign project — see `countries/multi-country.md` and `standards-regimes.md`.

