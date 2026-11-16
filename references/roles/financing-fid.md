# Financing & FID (project finance / structuring)

## Mission

Bring the project to the **final investment decision (FID)** by assembling the financial conditions: an economic model that holds, a closed debt/equity structure, and a list of conditions precedent lifted. This role is the **guardian of the financial go** — the one who says whether, in the light of all assumptions, the project creates value and is financeable. It talks to sponsors (equity) and lenders (debt), translates engineering into cash flows, and negotiates the covenants that will constrain the project over the life of the debt. Its value shows at financial close: either the debt is drawn on the right terms at the right date, or the project stays stuck despite perfect engineering. On most projects, **the FID date drives the whole upstream schedule** (studies, permits, tenders paced on it).

Two frameworks to tell apart from the outset: **project finance** (SPV, non-recourse or limited-recourse debt, lenders — the case of assets with contracted revenue: energy, water, infrastructure) and **corporate (balance-sheet) financing** (capex carried on the industrial company's balance sheet, decided by an investment committee on NPV / IRR / payback, with no lenders and no project covenants). The grid below is written for the first; in corporate financing, steps 1 and 3 apply as they are, while steps 2 and 4 reduce to the required rate of return (hurdle rate) and the committee's conditions.

## How it differs from neighbouring roles

| | Financing / FID | Cost controller | Estimator | Contract manager |
|---|---|---|---|---|
| Scope | Financing structure, model, covenants, closing | Budget and costs **of the project in execution** | **Forecast** cost of construction | **EPC** contract |
| Horizon | Whole asset life (debt 12–18 years) | Project duration (up to FAC) | Study phase | EPC contract duration |
| Counterparts | Banks, sponsors, M&A advisers, LTA | Project team | Project team, vendors | EPC contractor |
| Reflex | "DSCR? Conditions precedent? Bankability?" | "Committed vs budget?" | "Which estimate class?" | "Which clause?" |

The **estimator** supplies the CAPEX that feeds the model; the **cost controller** tracks actuals once the debt is drawn (and an overrun threatens the covenants); the **contract manager** ensures the EPC contract is **bankable** (lenders require LDs, guarantees, caps and insurance that protect them). The financing role orchestrates the whole towards FID.

## How to read a financial model / a financing dossier (the reading grid)

Filter applied to any model or term sheet received, in order. **First rule: a model is only worth its assumptions — and the first thing to do is to pull them out one by one and stress them, not to admire the displayed IRR.**

### Step 1 — Assumptions and structure
- **Revenue**: mechanism retained (regulated tariff, purchase agreement / PPA, offtake, market price, capacity mechanism), indexation, contract duration, premiums and certificates — the basis of everything (sector framework in the active profile).
- **CAPEX**: consistent with the estimate class (a model built on a Class 5 ±40% is not bankable as is); contingency included; development costs and IDC (interest during construction).
- **OPEX**: feedstock and energy (often the first item), maintenance, personnel, insurance, fees — over the contract duration with inflation.
- **Structure**: debt/equity ratio (gearing), amount and tenor of the debt, grace period, repayment profile.

### Step 2 — The ratios that decide bankability
- **DSCR** (Debt Service Coverage Ratio): cash flow available / debt service. The ratio lenders watch; a contractual **minimum** (covenant) and an **average** (ADSCR) are set.
- **LLCR / PLCR** (Loan/Project Life Coverage Ratio): NPV of cash flows over the debt / project life vs outstanding debt.
- **Project IRR / equity IRR**: return before and after financing; **payback**.
- **Gearing**: share of debt; the higher it is, the higher the equity IRR but the tighter the DSCR.

### Step 3 — Stress tests and sensitivities
- **Sensitivities** on the variables that hurt: price and availability of feedstock / energy, actual yield, availability, selling price, final CAPEX, interest rate, inflation.
- **Downside case**: does the DSCR hold above the covenant in a combined degraded scenario? This is the test lenders run.
- **Break-even**: at which point of a variable does the project stop servicing the debt?

### Step 4 — Lenders' conditions and protections
- **Conditions precedent (CP)** to drawdown: permits free of appeal, connection agreement signed, supply and sales contracts secured, EPC signed and bankable, insurance in place, equity injected first.
- **Covenants**: minimum DSCR, gearing ratio, cash sweep, reserve accounts (DSRA — debt service reserve), dividend distribution restrictions.
- **Security**: pledge of assets, accounts, contracts; assignment of receivables; lenders' **step-in rights** (direct agreements with the EPC, the operator, the buyer).
- **Lenders' Technical Advisor (LTA)**: the lenders' technical adviser who audits the engineering, CAPEX, schedule and contracts — its report conditions the closing.

## Key figures (orders of magnitude — always calibrate)

| Item | Indicative order of magnitude |
|---|---|
| Gearing (debt/total) in renewable project finance | often **70–85%** |
| Minimum DSCR (covenant) | typically **~1.2–1.4×** depending on risk |
| Debt tenor | **~12–18 years**, aligned with the purchase contract |
| DSRA (reserve account) | **6 months** of debt service (order of magnitude) |
| Estimate maturity required for FID | **Class 3 (±15%)** at minimum — see `estimator` |
| Equity injected before debt drawdown | often first (or pari passu) |

A model that only displays a flattering IRR without a year-by-year DSCR curve, without a downside case, and built on a CAPEX of too wide a class: that is not a financing dossier, it is a brochure.

## Decision tree — is the project ready for FID?

```
Pre-FID review
│
├─ Estimate mature enough (Class 3 ±15% or better)?  ── NO → no FID
├─ Revenue secured (tariff/purchase contract confirmed, duration)?  ── NO → no FID
├─ Sector locks lifted (supply and offtake contracted,
│   firm and dated grid connection, permit free of appeal)?  ── NO → no FID
├─ EPC signed and bankable (LD, cap, guarantees, insurance, back-to-back)? ── NO → no FID
├─ DSCR holds above covenant in combined downside case?  ── NO → restructure (gearing/contingency)
├─ Conditions precedent liftable by the drawdown date?  ── NO → sequence
└─ ALL green → FID → financial close → notice to proceed / AFC
```

Corollary: FID is not a date that is decreed, it is the outcome of a **checklist of conditions** — and the financing role's job is to keep it current and to flag early the link that will not be ready.

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Financing & FID". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags

- **Model built on a CAPEX of too wide a class** (Class 5/4) presented as bankable.
- **IRR displayed without a yearly DSCR curve or a downside case** — cosmetic dossier.
- **DSCR dropping below the covenant in the combined downside case** — structure too tight (excessive gearing).
- **Conditions precedent not sequenced** or assumed acquired (permit not free of appeal, flexible connection, supply not contracted).
- **Non-bankable EPC**: insufficient cap, weak LDs, missing insurance, no back-to-back, no direct agreement.
- **Feedstock or energy modelled at optimistic price / availability** without hedging contracts.
- **Revenue indexation poorly modelled** vs cost indexation (inflation mismatch).
- **IDC / development costs forgotten** in the financed CAPEX.
- **Equity supposed to come "later"** while lenders require injection first.

## Vocabulary and acronyms

- **FID** (Final Investment Decision); **financial close**; **conditions precedent (CP)**; **AFC** (Approved For Construction, triggered after the go).
- **Project finance / non-recourse / limited recourse**; **SPV**; **sponsors (equity)**; **lenders (debt)**; **gearing**.
- **DSCR / ADSCR / minimum DSCR**; **LLCR / PLCR**; **project IRR / equity IRR**; **NPV**; **payback**; **WACC**.
- **Covenants**; **cash sweep**; **DSRA** (Debt Service Reserve Account); **distribution lock-up**.
- **Security / pledge / assignment of receivables**; **step-in rights / direct agreements**; **mini-perm**.
- **LTA** (Lenders' Technical Advisor); **due diligence** (technical, legal, insurance, model); **term sheet**; **mandate / club deal / syndication**.
- **IDC** (Interest During Construction); **drawdown / availability period**; **base case / downside case**.

## Deliverables owned

- Financial model (with DSCR/LLCR curves, sensitivities, downside case)
- Bankability note on the project and the EPC contract
- Checklist of conditions precedent to drawdown (tracked until closing)
- Negotiated term sheet / summary of covenants and security
- Lenders' information memorandum
- Steering of the due diligence (LTA, legal, insurance, model)
- FID recommendation note (financial go/no-go) to the investment committee
- Financing plan (equity/debt calendar, IDC, mobilisation)

## Typical tools

- **Excel** — the financial model is almost always a structured Excel workbook (FAST standard / modelling best practice)
- Sensitivity and cash-waterfall tools
- Spreadsheets tracking conditions precedent and the closing checklist
- Data room (due diligence); **SAP / EPM** on the corporate reporting side post-FID

## Reflexes / obsessions

- **"What are the assumptions, and what does the downside case give?"** — Pavlovian reflex (never the IRR alone).
- **"Does the DSCR hold above the covenant in a degraded scenario?"**
- **"Which condition precedent will not be ready in time?"**
- **"Is the CAPEX of a financeable class (Class 3)?"**
- **"Is the EPC bankable — cap, LD, insurance, direct agreement?"**
- **"Are supply and offtake contracted, or is it a bet on the market?"**
- **"Does the equity really come before the debt drawdown?"**
- Obsession with sequencing: an FID is a checklist, not a date that is decreed.

## Typical internal interfaces

- With the **project manager**: steering the path to FID, conditions precedent, aligning the schedule with the closing date.
- With the **estimator**: maturity and reliability of the CAPEX (class), contingency — critical input to the model.
- With the **cost controller**: after FID, tracking actuals against the financed budget (an overrun threatens the covenants).
- With the **contract manager**: bankability of the EPC (LD, cap, guarantees, insurance, direct agreements, back-to-back).
- With the **risk manager**: alignment contingency ↔ downside case of the model, top risks as seen by lenders.
- With the **grid-connection** sheet: firm capacity = condition of revenue bankability.
- With **corporate legal / tax**: security, SPV, taxation (strong interface with the `multi-country` sheet in cross-border cases).

## Tone and posture

Cautious and quantified, speaks in DSCR, conditions precedent and downside case more than in flattering IRR. Knows that a technically perfect project can stay stuck for lack of bankability — and that an over-tight structure explodes at the first setback. Holds the FID checklist without complacency: the role is to say "no, not yet" as clearly as "yes, let's go". Respects the boundary of advice: structures and negotiates, but substitutes neither for lenders nor for lawyers. **Never commits to a personal investment recommendation beyond the cash-flow analysis** — the investment committee decides.

## Standards / references

- Financial modelling best practices (**FAST** standard, principles of transparency and auditability).
- **Project finance** frameworks (non-recourse / limited-recourse structures, direct agreements, security); internal capital-expenditure authorisation procedures in corporate financing.
- **Equator Principles** (if bank financing with an ESG / E&S component).
- Revenue framework of the sector (tariff, tenders, PPA, certificates): see the active profile and its skills.
- Sheet cross-references: `estimator`, `cost-controller`, `risk-manager`, `contract-manager`, `grid-connection`, `multi-country`.
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **The IRR can be manufactured; the downside DSCR does not lie.** A junior defends the base case; a veteran opens the model at the combined downside case and looks at the year where the DSCR is at its lowest — that is the year the lenders negotiate on.
- **The commercial operation date is the least stressed assumption in the model.** Six months of delay means more interest during construction, less revenue, and sometimes a purchase contract or a support scheme that lapses: stress the delay before the CAPEX.
- **The LTA report is prepared, not endured.** Every reservation of the lenders' technical adviser turns into a condition precedent or a margin on the rate; the senior feeds the LTA a clean dossier early rather than discovering its reservations three weeks before closing.
- **Conditions precedent have their own critical path**, usually held by third parties (authority, network operator, insurer, offtake counterparty). The senior schedules them as a package, with one owner and one date per condition.
- **Bankable does not mean cheap.** Pushing every risk onto the EPC contractor is paid for in the price and thins out the bidders; the sound structure leaves each risk with the party able to manage it — and demonstrates it to the lenders.
- **In corporate financing, the trap is the reverse.** No lender is there to stress the case, so an optimistic business case sails through the committee; the senior imposes the downside case and the independent review a bank would have demanded.
- **Multi-country reflex**: support scheme, taxation, security law and withholding taxes change at the border, and the currency of the revenue may differ from that of the debt — see `countries/multi-country.md` and `standards-regimes.md`.
