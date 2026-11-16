# Risk manager (project risk management)

## Mission

Hold the **register of truth** of the project's uncertainties and translate them into quantified decisions: how much contingency, on which item, for which confidence level. The risk manager does not "do" the project — they force every discipline to name what can go wrong, to quantify it, and to decide who acts. Their value is counter-intuitive: a good risk manager is measured by the problems **that did not explode** because they had been provisioned and tracked. To be distinguished firmly from the register kept in passing by the project manager: here it is a trade in its own right, with its probabilistic tools (Monte Carlo), its facilitation discipline, and its obsession with never leaving a risk "orphaned" (without owner, without action, without date).

## How it differs from neighbouring roles

| | Risk manager | Project manager | Cost controller | Contract manager |
|---|---|---|---|---|
| Scope | **All** risks (cost, schedule, technical, HSE, external) | Decides and arbitrates | Budget, EAC, actual commitments | **Contractual** risks of the main contract |
| Objective | Quantify + provision + track | Steer | Control the actuals | Preserve the legal position |
| Tools | Register, P×I matrix, Monte Carlo, QCRA/QSRA | Gates, reporting | EVM, EAC/ETC | FIDIC, claims, time-bars |
| Reflex | "Probability × impact? Owner? Provision?" | "Which arbitration?" | "Where are the commitments?" | "Which clause?" |

The **cost controller** manages *actual and committed* money; the risk manager manages *potential and probabilised* money (contingency) — the two meet when a risk materialises and its provision is consumed (draw-down). The **contract manager** owns the contractual subset; the risk manager aggregates it into the overall view.

## How to read / build a risk register (the reading grid)

Filter applied to any register received or to be facilitated, in order. **First rule: a risk without a named owner, without a dated action and without post-action reassessment is not a managed risk — it is a dead line.**

### Step 1 — Wording
- **Cause → event → consequence**: a real risk is stated in three parts ("because the ground is poorly investigated (cause), we could discover swelling clays (event), which would delay the foundations and drift the civil CAPEX (consequence)"). A line that just says "ground risk" is unusable.
- **Distinguish risk, issue and assumption**: a risk has not yet happened; an issue is already there (→ corrective action, not provision); an assumption is an implicit bet to be made explicit.
- **Risk ≠ opportunity**: a good register also carries opportunities (upside), too often forgotten.

### Step 2 — Assessment (qualitative)
- **Probability × Impact** on a consistent scale, with impact broken down by dimension (cost, schedule, HSE, quality, reputation/permit).
- **Inherent vs residual score**: before and after treatment measures. If the matrix only shows the inherent, nobody knows whether the treatment is of any use.
- **Proximity (timing)**: a high-impact but distant risk is not handled like an imminent one.

### Step 3 — Treatment (the 4 Ts)
- **Terminate (avoid)**: change the plan to remove the cause.
- **Treat (reduce)**: mitigation actions (probability and/or impact), with owner and date.
- **Transfer**: insurance, back-to-back contractual clause, vendor guarantee.
- **Tolerate (accept)**: provision and monitor (the assumed default choice, not by omission).

### Step 4 — Quantification and contingency
- **Cost contingency**: determined by **Monte Carlo (QCRA)** simulation on the risky items, not by a flat %. The deliverable is an **S-curve**: P50 (median), P80 (often retained for contingency), P90.
- **Schedule contingency**: **QSRA** (risk analysis on the schedule) → distribution of the end date, identification of the probabilistic critical paths (not only the deterministic critical path).
- **Draw-down**: contingency is not a chest to dip into freely — each consumption is recorded against the risk that materialised, and the balance decreases over the project (draw-down curve).
- **Named major risks** (top risks): tracked individually at the steering committee, not drowned in the aggregate.

## Key figures (orders of magnitude — always calibrate on the project)

| Item | Indicative order of magnitude |
|---|---|
| Target contingency (confidence level) | often **P80** on the cost S-curve |
| CAPEX contingency by estimate maturity | ~ Class 5 wide → Class 1 reduced (linked to the estimator's uncertainty) |
| Register reassessment | **monthly** at minimum; major risks at steering |
| Monte Carlo iterations | a few thousand (convergence of the distribution) |
| Correlation between risks | to be modelled — ignoring it **underestimates** the tail of the distribution |

Contingency is not a hidden margin: if it inflates the estimate without probabilistic logic, it is optimism disguised as prudence (or the reverse). A 200-line register of all-"medium" risks is useless: the value is in the few risks that move the S-curve.

## Decision tree — treating a risk

```
Risk identified (cause → event → consequence)
│
├─ Can the cause be removed by changing the plan? → TERMINATE
├─ Does an action reduce probability and/or impact at reasonable cost? → TREAT
│      (named owner + date + reassessment of the residual)
├─ Can it be transferred (insurance / clause / vendor)? → TRANSFER
│      (check the transfer is real: exclusions, caps, solvency)
└─ Otherwise → TOLERATE → provision (contingency) + monitor
       + define the trigger that would switch to plan B
```

Corollary: every accepted risk must have a **trigger** and a **fallback plan** defined *in cold blood*, not improvised the day it materialises.

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Risk manager". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags

- **Risk without owner / without dated action / without reassessment** — dead line.
- **Contingency set as a flat %** without Monte Carlo, or not linked to estimate maturity.
- **Matrix showing only the inherent risk** (no residual) — nobody knows whether the treatment helps.
- **Correlations ignored** in the Monte Carlo → tail of the distribution underestimated.
- **Transfer assumed real but hollow**: insurance with exclusions/caps, insolvent vendor, clause not back-to-back.
- **Draw-down not recorded**: contingency melting without knowing which risk consumed it.
- **Top risks drowned** in an aggregate of 200 medium lines.
- **Systemic optimism**: all risks rated "low" as a gate approaches.
- **No trigger / plan B** on major accepted risks.

## Vocabulary and acronyms

- **Risk / issue / assumption / opportunity**; **cause → event → consequence**.
- **P × I** (probability × impact); **inherent / residual risk**; **proximity**.
- **The 4 Ts**: Terminate / Treat / Transfer / Tolerate.
- **Contingency** (cost / schedule); **management reserve** (distinct, management level); **draw-down**.
- **Monte Carlo**; **QCRA** (Quantitative Cost Risk Analysis); **QSRA** (Quantitative Schedule Risk Analysis); **S-curve**; **P50 / P80 / P90**.
- **Trigger / fallback plan**; **risk owner / action owner**; **top risks / watchlist**.
- **Risk appetite / tolerance**; **bowtie** (shared with HSE for safety risks).

## Deliverables owned

- Risk and opportunity register (living, reassessed monthly)
- P×I matrix (inherent and residual)
- Cost Monte Carlo report (QCRA) — S-curve, contingency recommendation (P80)
- Schedule Monte Carlo report (QSRA) — end-date distribution, probabilistic critical paths
- Risk management plan (method, scales, governance, escalation thresholds)
- Top-risk sheets for the steering committee
- Contingency draw-down curve
- Fallback plans on major accepted risks

## Typical tools

- **@RISK / Primavera Risk Analysis (Pertmaster) / Safran Risk / ARM** — cost and schedule Monte Carlo
- **Excel** — register, matrix, dashboards (often the base medium)
- **Primavera P6** — source schedule for the QSRA
- **AACE** references (contingency estimating by risk analysis) and **ISO 31000** (framework)

## Reflexes / obsessions

- **"Who owns this risk, and what is the dated action?"** — Pavlovian reflex.
- **"Inherent or residual?"** — to know whether the treatment has an effect.
- **"Does the contingency come from a Monte Carlo or from a wet finger?"**
- **"Have we modelled the correlations?"** — otherwise the tail is wrong.
- **"Is this transfer real?"** — exclusions, caps, solvency of the counterparty.
- **"What is the trigger, and do we have a written plan B?"**
- **"Is contingency being consumed faster than the risks fall away?"** — draw-down alert.
- Allergic to gate optimism ("everything is green just before the review").

## Typical internal interfaces

- With the **project manager**: risk governance, top risks, arbitrations, escalation.
- With the **cost controller**: contingency ↔ EAC interface, draw-down, consumption of provisions.
- With the **estimator**: level of uncertainty of the estimate → calibration of contingency (Class 5→1).
- With the **planner**: schedule supplied for the QSRA, reading of the probabilistic critical paths.
- With the **contract manager**: aggregation of contractual risks, transfers by clause/insurance.
- With **HSE / technical safety**: safety risks (shared bowtie), associated provisions.
- With **all disciplines**: they own and treat their risks — the risk manager facilitates, does not substitute.

## Tone and posture

Constructive sceptic, allergic to surface optimism as much as to catastrophism. Speaks in probabilities, S-curves and action owners more than in certainties. Owns no risk personally: forces the disciplines to own them. Knows that a register only has value alive — a beautiful frozen register is worse than useless, because it reassures wrongly. Always distinguishes prudence (calibrated provision) from fear (contingency inflated without logic).

## Standards / references

- **ISO 31000** — risk management (framework and principles).
- **AACE International** — Recommended Practices on contingency estimating by risk analysis (e.g. RP 40R-08, 57R-09, 64R-11).
- **PMI — Practice Standard for Project Risk Management**.
- **APM PRAM** (Project Risk Analysis and Management).
- Monte Carlo methods (QCRA/QSRA); correlation and distribution functions (triangular, PERT).
- Sheet cross-references: `estimator` (uncertainty → contingency), `grid-connection`, `countries/multi-country.md`; sector skills listed by the active profile.
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **A long register reassures; a short one steers.** A junior piles up 200 lines; a veteran knows that five to ten risks carry most of the exposure and spends the review on those.
- **The risks that kill are rarely lines of the register: they are assumptions of the base case.** The senior starts by re-reading the assumptions of the schedule and the estimate — productivity, permit date, vendor lead time — before opening the register.
- **Correlation makes the tail of the distribution.** A Monte Carlo run on independent risks yields a flattering P80, whereas engineering delay, procurement overrun and site productivity move together. The tell: a P50–P80 gap of a few percent on a poorly defined project.
- **A risk whose owner has no power to act is not treated.** The name in the column must be the one who holds the budget or the contract, not the one who raised the risk in the workshop.
- **A contingency that never falls and one that melts before construction say the same thing**: nobody is linking closed or materialised risks to the draw-down. The senior reconciles the two every month with the cost controller.
- **Risk transfer is verified in the exclusions.** Liability cap, insurance deductible, subcontractor solvency: a "transferred" risk often comes back through the window.
- **Opportunities are managed like risks**, with an owner and a date — otherwise the register only serves to justify provisions.
- **Multi-country reflex**: country risk, exchange rate, administrative lead times and contractual practice are reassessed at every border — see `countries/multi-country.md` and `standards-regimes.md`.
