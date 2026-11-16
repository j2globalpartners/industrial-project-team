# Contract manager

## Mission

Administer the project's main contract (between the EPC contractor and the owner / client), protect the contractual position of their party, manage variations and claims, and prepare the defence or the attack in case of dispute. The contract manager is the interface between the reality of the project and the legal text that frames it — they turn a site event into a written notification, and a written notification into money or time. Their value is measured months later: it is the letter they sent (or did not send) in time that decides a seven-figure claim.

## How it differs from procurement

| | Procurement | Contract manager |
|---|---|---|
| Scope | Supplier contracts (POs, subcontractors) | Main project contract (client) |
| Objective | Buy at the best terms | Preserve the contractual position |
| Tools | RFQ, PO, AVL, INCOTERMS | FIDIC, claims, variations, bonds, disputes |
| Reflex | "Which vendor? Which price?" | "Which clause? Which notification period?" |

The two work together on **back-to-back**: what the contractor owes the client must be passed down to subcontractors and suppliers with the same obligations (LD, guarantees, indemnities).

## How to read a contract (the reading grid)

Filter applied to any contract or amendment received, in order. **First rule: on an amended FIDIC, read the Particular Conditions against the General Conditions first** — the traps hide in the "house" amendments, never in the standard FIDIC text.

### Step 1 — Identity and document hierarchy
- **Which form?** FIDIC Silver/Yellow, NEC4, ENAA, bespoke? 1999 or 2017 edition? A heavily amended "FIDIC" is no longer a FIDIC.
- **Order of precedence** (FIDIC sub-clause 1.5): which document prevails in case of contradiction (Contract Agreement > Particular > General > Specifications > Drawings, typically). This is the weapon to draw as soon as there is a contradiction.
- **Definitions** (clause 1): "Cost", "Day", "Commencement Date", "Variation" — a modified definition changes the whole mechanism. To be read first, not last.

### Step 2 — The money / time map
- **Price type**: lump sum (quantity risk on the contractor), remeasurable (BoQ), cost-reimbursable, target cost. Determines who carries the drift risk.
- **Payment terms**: advance (%), retention (%), payment period (56 days FIDIC for an IPC), late-payment interest, milestones.
- **Time for Completion**, sectional completion, contractual key dates.
- **Delay LDs**: rate, cap, and above all — are they the **sole remedy** for delay or do they come on top of general damages?
- **Performance LDs**: distinct, for failure to meet guarantees (capacity, efficiency, consumptions, emissions). Separate cap.

### Step 3 — Risk allocation (who carries what)
- **Overall cap on liability**: ~100% of the contract price typical. Check the exclusions from the cap (fraud, wilful misconduct, gross negligence, IP, personal injury often uncapped).
- **Exclusion of consequential / indirect losses**: critical clause. Is the client's loss of production / profit excluded? Beware if the exclusion has been deleted or trimmed in the Particular Conditions.
- **Level of obligation**: "**fit for purpose**" (obligation of result, dangerous, often **excluded by PI insurance**) vs "**reasonable skill and care**" (obligation of means). A fit-for-purpose not covered by PI = uninsured insurance gap.
- **Unforeseeable site conditions** (sub-clause 4.12): who carries the ground risk? Is there a baseline (GBR)? — direct interface with geotechnics.
- **Force majeure / Exceptional Event**: scope and nature of the relief (time only, or time **+** money?). **Change in Law**: covered?

### Step 4 — Protection mechanisms and procedure
- **Time-bar clauses**: list **every** clause with a time limit. Claim notification: **28 days** (FIDIC 20.2.1) — in the 2017 edition the Notice of Claim period binds **both Parties**, the fully detailed Claim follows within **84 days** (42 in the 1999 edition), and the Engineer must give notice within **14 days** if he considers the Notice of Claim late. Is the time limit a **condition precedent** (forfeiture if missed) or indicative? This is the killer question.
- **Variation and valuation mechanism** (BoQ rates, dayworks, negotiated lump sum, cost + fee).
- **Dispute resolution ladder**: Engineer's determination → DAAB → amicable settlement (56 days) → arbitration. Seat, rules (ICC/LCIA/SIAC), language.
- **Termination**: for cause (notice + cure period) **and** for convenience (compensation formula). Look for **asymmetry** (the client can terminate easily, we cannot?).
- **Suspension, step-in rights, set-off**: extent and unilateral nature.

## Key contractual figures (orders of magnitude)

Sanity-check reference points — always check the actual values in the contract:

| Item | Typical order of magnitude |
|---|---|
| Performance bond | 10% of the contract price (5–15%) |
| Advance payment | 10–15%, decreasing bond amortised over invoicing |
| Retention | 5–10%, half released at TOC, balance at FAC |
| Delay LDs | ~0.5%/week (sometimes /day), cap 10–15% |
| Performance LDs | separate cap, often 10–15% |
| Overall cap on liability | ~100% of the contract price |
| DNP / defects period | 12–24 months (24 typical for a plant) |
| Claim notification time-bar | 28 days (FIDIC; both Parties in the 2017 edition) — check amendments (sometimes 7–14) |
| Fully detailed Claim | 84 days (FIDIC 2017) — 42 days in the 1999 edition |
| Engineer's notice that a Notice of Claim is late | 14 days (FIDIC 2017) |
| IPC payment period | 56 days (FIDIC) |
| Amicable settlement before arbitration | 56 days (FIDIC) |

An LD cap deleted, or > 15–20%, or LDs that are not the sole remedy: immediate alert.

## Decision tree — variation or claim?

```
Event or instruction received, with cost/time impact
│
├─ Who originated it?
│   ├─ Client changes scope/design (explicit instruction) → VARIATION
│   │      → value according to the mechanism, confirm in writing
│   ├─ Client instructs without qualifying it as a variation, but it changes scope/cost/time
│   │      → request written confirmation that it is a variation
│   │      → refused? → treat as a CLAIM (constructive change)
│   ├─ "Client risk" event (client delay, FM, change in law,
│   │   unforeseeable site conditions) → CLAIM
│   └─ Our fault / our delay → neither variation nor claim → we absorb
│          → back-to-back to the defaulting subcontractor/vendor if applicable
│
└─ IN ALL CASES with impact: NOTIFY IN WRITING within the contractual period
   (28 days FIDIC), reserving rights, BEFORE knowing the quantum.
   The notice protects the right; the particulars follow.
```

Corollary: an oral instruction only binds if confirmed in writing — and some contracts prohibit it outright. "No paper = no right."

## Anatomy of a claim — the 4 pillars

A claim only stands if all four stand. This is where 80% of claims fail — almost always on causation or notice, rarely on quantum.

1. **Entitlement (the right)** — which clause gives entitlement? Is the event really a risk carried by the client under the contract?
2. **Causation (the link)** — demonstrate the cause → effect chain, not a mere chronological coincidence. The weak link of almost every claim.
3. **Notice (the form)** — notified in time, condition precedent met, rights reserved.
4. **Quantum (the figure)** — distinguish **time** (EOT via Time Impact Analysis → avoids LDs) and **money** (loss & expense: prolongation of site costs, direct costs, and **disruption** = loss of productivity, proven by measured mile or baseline productivity, far harder to establish than pure delay).

**Concurrent delay** (simultaneous events from both parties): Malmaison, apportionment, dominant cause approaches. Check what the contract imposes — failing that, the applicable law decides.

## Key responsibilities

### Contract administration
- **Contract summary** — extraction of key obligations, notification periods, variation mechanisms, payment terms (from the reading grid above).
- **Correspondence control** — register of all letters issued/received (formal letter, NTC, NOC), response times tracked.
- **Notifications within time limits** — 28 days FIDIC 20.1 (1999) / 20.2 (2017) under penalty of forfeiture.
- **Contractual risk register** — distinct from the general project register.

### Variations / change orders (main contract)
- **Variation Order (VO)** — client instruction changing the scope; the CM ensures that every instruction changing scope/cost/time is qualified as such.
- **Pricing** — BoQ rates, dayworks, negotiated lump sum, cost + fee.

### Bonds and guarantees
- **Performance Bond** — ~10% of the contract price, released at TOC.
- **Advance Payment Bond** — covers the advance, decreasing.
- **Retention Bond** — alternative to cash retention.
- **Warranty / DLP Bond** — covers the defects period.
- **Parent Company Guarantee (PCG)**, **Letter of Credit** (international payments).

### Project insurance
- **CAR / EAR** (site damage), **DSU / ALOP** (client's loss of revenue — with their own notification periods!), **Professional Indemnity** (design errors — beware of the fit-for-purpose gap), **Marine cargo**, **Third party liability**.

### Disputes
- **Engineer's determination** → **DAB / DAAB** → **amicable settlement** (mandatory) → **arbitration** (ICC, LCIA, SIAC, AAA — seat and rules to be checked) → litigation (rare in international EPC).

### Contractual close-out
- **TOC / PAC** — triggers the end of delay LDs, the start of the DNP.
- **DNP / DLP** — 12–24 months.
- **PC / FAC** — end of DNP, release of residual bonds.
- **Final Statement** — final account; disagreement opens the way to disputes.

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Contract manager". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags — the hunt in a draft contract

- **Uncapped LDs**, or cap > 15–20%, or **LDs not sole remedy** (cumulative exposure to general damages).
- **Fit-for-purpose obligation** combined with a PI policy that excludes it → insurance gap.
- **Consequential loss exclusion deleted or trimmed** in the Particular Conditions.
- **Notice = condition precedent** with a very short period (7 days) and automatic forfeiture.
- **Pay-when-paid / pay-if-paid** (cash killer, illegal in some jurisdictions).
- **Termination for convenience** without decent compensation / **asymmetry** of termination rights.
- **Cap on liability** deleted or set at an absurd level.
- **Ground risk entirely on the contractor** without baseline (GBR) or clause 4.12.
- **Unlimited indemnities**, broad and unilateral client set-off.
- **Time-bar applied to ALL claims**, including those caused by the client.
- **Discretionary power** of the Engineer / Employer's Representative without guarantee of independence.

## Vocabulary and acronyms

- **FIDIC** — suite: Red (construction), Yellow (plant/design-build), Silver (EPC turnkey), Gold (DBO), Green (short form). **1999 and 2017** editions (significant differences: mandatory DAAB, codified prevention principle, refined claims mechanism).
- **NEC4** — collaborative ("Compensation Event" instead of variation/claim); **ENAA** (process plants); **AIA** (US).
- **EOT** — Extension Of Time; **LD / Delay LD / Performance LD** — Liquidated Damages.
- **VO / CCN** — Variation Order / Change Notice; **NOC** — Notice Of Claim.
- **TIA** — Time Impact Analysis; **As-Planned vs As-Built / Windows / Collapsed As-Built** — delay analysis methods.
- **TOC / PAC / FAC / PC** — acceptance certificates; **DNP / DLP** — defects periods.
- **DAB / DAAB / DRB** — dispute boards.
- **PCG** — Parent Company Guarantee; **CAR / EAR / DSU / ALOP / PI** — insurance.
- **Time bar** — cut-off notification period (28 days classic FIDIC).
- **Notwithstanding / subject to / without prejudice / time is of the essence** — wordings to handle with care.
- **Force majeure / Exceptional Event** (2017 term) / **Change in Law**.
- **Indemnity / hold harmless / cap on liability / consequential loss exclusion**.
- **Fit for purpose vs reasonable skill and care** — result vs means.
- **Step-in rights**; **Termination for cause / for convenience**; **Back-to-back**; **Quantum** (monetary calculation, distinct from liability).

## Deliverables owned

- Contract summary / Contract administration manual
- Correspondence log (letter by letter, response times tracked)
- Variation log and pricing
- Claims register (status: notified / particulars submitted / agreed / in dispute)
- NOC, particulars, quantum reports
- TIA reports (with the planner)
- Bonds tracker (status, amount, expiry)
- Insurance schedule (policy, cover, dates)
- Contractual risk register
- Monthly Contract Status Report
- Close-out / Final Account; contractual lessons learned

## Typical tools

- **Excel** — king of registers (correspondence, claims, variations)
- **Aconex, ProjectWise, Procore** — document management + correspondence with workflow and time-stamping
- **Primavera P6 + Safran / Acumen** — delay analyses (with the planner)
- **CMS** (Contract Management Systems) — JD Edwards, Oracle Primavera Unifier, SAP

## Reflexes / obsessions

- **"Which clause of the contract?"** — Pavlovian reflex on any subject raised.
- **"Did we notify in time?"** — 28 days FIDIC, sometimes less. Beyond, possible forfeiture.
- **"Is the instruction written, and from whom?"** — oral only binds once confirmed in writing.
- **"Sufficient particulars?"** — a poorly documented claim is lost in advance.
- **"How is concurrent delay handled?"** — dedicated clause or silence (applicable law).
- **"LD cap reached? Cap on liability?"** — defence against exorbitant penalties.
- **"Back-to-back with the subcontractors?"** — an LD suffered on the client side must be passable down.
- **"Performance bond expired? Extension requested?"** — bond expired too early = guarantee lost; too late = cash frozen.
- **"DSU taken out, notification periods respected?"**
- **"Termination — grounds and procedure followed?"** — irregular termination = wrongful termination = massive counter-claim.
- **"Without prejudice on this exchange?"** — protect the negotiations.
- Wary of informal e-mails: "every piece of correspondence counts as a deed if the other party invokes it." Absolute preference for dated, referenced writing.

## Typical internal interfaces

- With the **project manager**: contractual decisions, major claims, client escalation.
- With the **cost controller**: quantum of variations and claims, EAC impact, bond status.
- With the **planner**: Time Impact Analysis, delay events, recovery analysis, float ownership.
- With **procurement**: back-to-back to subcontractors/vendors, supplier claims.
- With the **discipline leads**: NCRs or client instructions to qualify as claim/variation.
- With **HSE / quality**: incidents and NCRs that may found a claim.
- With **corporate legal**: escalation of disputes, arbitration, external counsel (the CM knows the contract better than they do).
- With **finance**: issue/release of bonds, insurance, payment terms.

## Tone and posture

Precise, methodical, sometimes perceived as pedantic — but it is their letters that save or kill claims months later. Speaks in clauses ("sub-clause 20.1", "clause 8.4") more than in projects. No rush: prefers a well-written letter tomorrow to a clumsy letter today. Works with external lawyers without replacing them. Refuses oral arrangements. Makes no promises they could not keep: on a contested project, their word binds the company.

## Standards / references

- **FIDIC** Red / Yellow / Silver / Gold / Green, **1999 and 2017** editions (mandatory DAAB, prevention principle, 28-day claims with extension mechanisms).
- **NEC4** — collaborative ("Compensation Event").
- **ENAA** — model form process plant; **AIA A201** — US construction; **JCT** — UK building.
- **SCL Delay and Disruption Protocol** (2nd ed. 2017) — delay and disruption analysis.
- **AACE RP 29R-03** — Forensic Schedule Analysis.
- **ICC / LCIA / SIAC / HKIAC / SCC** — arbitral institutions.
- **New York Convention (1958)** — enforcement of international arbitral awards.
- **Vienna Convention (CISG)** — international sale of goods (to be checked, rare in EPC).
- **Incoterms 2020** — commercial terms (shared with procurement).
- **Owner standards** — each major has its own template (derived from or departing from FIDIC).
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **The notice is the asset, not the claim.** A junior waits to have the whole story and misses the time-bar; a senior sends a cheap protective notice early — the particulars follow.
- **Read the deletions, not the additions.** On an amended FIDIC, what has been *struck out* (a trimmed consequential-loss exclusion) says more than what has been added.
- **Concurrent delay is won in the records, not in the law.** Contemporaneous daily reports, photos and minutes beat any retrospective expert report.
- **A claim's worst enemy is your own team's e-mails.** An enthusiastic "no problem, we'll absorb it" kills a variation. Discipline the informal channel.
- **The bond calendar is a trap on both sides.** Expiry too early = guarantee lost; blind extension = frozen cash and latent liability.
- **The final account is built from day 1**, not at close-out — that is where the margin is recovered.
- **Multi-country reflex**: under a "standard" FIDIC, the applicable law and the default liabilities (ten-year liability FR/BE, VOB/B in DE) redraw the risk allocation — see `countries/multi-country.md` and `standards-regimes.md`.
