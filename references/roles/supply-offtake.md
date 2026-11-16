# Supply & offtake (upstream and downstream commercial contracts)

## Mission

Secure **what goes into the plant and what comes out of it**, over the life of the asset: raw materials, energy and utilities bought upstream; products, by-products and waste sold or disposed of downstream. This is the role that turns a nameplate capacity into **credible revenue**: a perfectly built plant that is short of feedstock, or that produces without a committed buyer, repays nothing. It negotiates the supply and offtake contracts, measures how much of the business plan is genuinely **contracted**, and says plainly what remains a market bet. It buys neither the equipment nor the works of the project (procurement does) and does not structure the financing (financing & FID does): it gives them volumes, prices and counterparties. Its value shows a few years after start-up: either volumes and prices hold, or the plant runs at part load with a margin that exists only in the model.

## How it differs from neighbouring roles

| | Supply & offtake | Procurement | Contract manager | Financing & FID |
|---|---|---|---|---|
| Subject | **Operating** flows, over the life of the asset | Equipment and works **of the project** | The **construction** contract | Financing structure |
| Horizon | Life of the asset | Duration of the project | Duration of the EPC contract | Tenor of the debt |
| Counterparty | Feedstock suppliers, buyers, traders, public bodies | Vendors, subcontractors | Contractor | Lenders, sponsors |
| Reflex | "Which volume is firm, at what price, with whom?" | "What lead time, what total cost?" | "Which clause, which deadline?" | "Does the DSCR hold?" |

Key boundary with **process**: process says what the plant *can* take in and produce; this role says what it *will have* to take in and *will be able* to sell — and both specifications (quality of the incoming material, quality of the outgoing product) must match what is written in the contracts. With **financing**: it supplies the contracted share of revenues and costs, which is what makes the project bankable.

## Key responsibilities

- **Draw up the supply plan and the sales plan**: volumes, prices, counterparties, year by year, ramp-up included.
- **Rank every volume by degree of commitment** (firm contract, conditional contract, letter of intent, market assumption) and keep the contracting table.
- **Negotiate the supply and offtake contracts** with legal counsel: term, price, indexation, volume commitments, default, assignment.
- **Align the contractual specifications** of the incoming material and the outgoing product with what the process can actually take and make, measurement method included.
- **Measure concentration** by counterparty and price the fallback options.
- **Check that upstream and downstream indexation are consistent**, and give financing the base case and the downside case.
- **Secure the outlet for by-products and waste**, on the same footing as the main product.
- **Watch the market and the catchment**: competing projects in development, movements in prices and availability.

## How to read a supply or sales plan (the reading grid)

Filter applied to any business plan, letter of intent or draft contract, in order. **First rule: rank each volume by its degree of commitment — signed firm contract, conditional contract, letter of intent, market assumption — and count only the first as secured.**

### Step 1 — Volumes and coverage
- **Nameplate requirement** of the plant for each input, and nameplate output of each product, year by year (ramp-up included).
- **Contracted share**: the part of the requirement and of the output covered by firm contracts, in volume **and in duration** (a short contract does not cover a long debt).
- **Profile within the year**: seasonality of upstream availability and downstream demand, and the storage capacity that acts as the buffer.

### Step 2 — Quality and measurement
- **Contractual specification** of the incoming material and the outgoing product, sampling and analysis method, reference laboratory in case of disagreement.
- **Consequence of a deviation**: price adjustment, rejection of the lot, obligation to take back. A specification without a measurement procedure protects no one.
- **Point of transfer** of title and risk, and the metering that is binding.

### Step 3 — Price and indexation
- **Price formula**: fixed, indexed to a published index, or market price with a floor and a cap.
- **Indexation mismatch**: do upstream costs and downstream revenues follow the same indices? An upstream indexed to energy and a fixed-price downstream is a margin that closes.
- **Review and renegotiation clauses**: triggers, frequency, outcome if the parties disagree.

### Step 4 — Commitments and exits
- **Offtake or delivery commitment** (take-or-pay, deliver-or-pay): minimum volume, penalty, carry-forward or make-up rights.
- **Default**: what happens if the supplier does not deliver, if the buyer does not lift, if the plant is down? Who pays for the shortfall?
- **Exclusivity, term, termination, assignment**: does the contract follow the asset on a sale, or if the lenders enforce their security?

### Step 5 — Counterparties and concentration
- **Strength** of each counterparty (financial health, durability of its business, guarantees given).
- **Concentration**: share of the largest supplier and of the largest buyer. Dependence on a single counterparty is a project risk, not a contract line.
- **Fallback**: substitute market, wider sourcing radius, another outlet — and at what cost.

## Anchor figures (qualitative — always calibrate)

| Item | Indicative anchor |
|---|---|
| Target contract term | matched to the tenor of the debt or the depreciation period; failing that, the longest obtainable with a renewal clause |
| Contracted share expected by lenders | a large majority of the flows that make the revenue; the balance is stressed in the downside case |
| Weight of a single counterparty | beyond a significant share of the volume, to be treated as a named risk on the register |
| Transport cost | often the factor that bounds the sourcing radius for bulky, low-value materials |
| Ramp-up | several years at part load before nameplate operation — to be modelled, volume commitments included |

These anchors are deliberately qualitative: numerical thresholds depend on the sector, the lender and the market, and are set on the project.

## Decision trees — is this volume secured?

```
Volume entered in the business plan (upstream or downstream)
│
├─ Contract signed, firm, with no open condition precedent?
│   ├─ NO → letter of intent or assumption → do not count it in the downside case
│   └─ YES →
│        ├─ Term ≥ financing horizon?  ── NO → model the renewal at a degraded price
│        ├─ Price and indexation consistent with the other side of the chain?  ── NO → quantify the mismatch
│        ├─ Real non-performance penalty and solvent counterparty?  ── NO → theoretical commitment
│        └─ Specification measurable and achievable by the process?  ── NO → a dispute waiting to happen
│
└─ All YES → volume secured; otherwise enter it on the risk register with its fallback

Never: count a letter of intent as a volume, or a full plant from year one.
```

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Supply & offtake". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags — the hunt

- **Letters of intent counted as contracts** in the business plan → the base-case revenue binds no one.
- **A dominant supplier or buyer**, with no priced fallback → its default stops the plant.
- **Contract terms far shorter than the financing**, with no degraded renewal assumption.
- **Contracts that cannot be assigned**, or that can be terminated on a change of control → incompatible with project finance.
- **Diverging upstream and downstream indexation** → margin exposed to an index nobody hedges.
- **By-products and waste with no contracted outlet** → they are often what stops the plant, by filling the storage.
- **Offtake commitment without a penalty**, or with a penalty capped at a token level → theoretical commitment.
- **Quality specification with no measurement method and no reference laboratory** → a dispute at the first contested delivery.
- **Seasonality ignored**: annual volumes sufficient, but not enough storage to get through the trough.
- **Volume commitments firm from the day of start-up**, ignoring the ramp-up → penalties while the plant is still learning.
- **Sourcing radius overlapping that of a competing project** already in development.

## Vocabulary and acronyms

- **Offtake / purchase agreement**; **take-or-pay / deliver-or-pay**; **tolling**.
- **Letter of intent (LOI)** / heads of terms / **firm contract**; **conditions precedent**.
- **Contracted share**; **concentration**; **sourcing radius / catchment**.
- **Indexation formula**; price **floor / cap**; **price review clause**.
- **Specification**; **price adjustment** (for off-spec quality); **rejection of a lot**; point of **transfer of title and risk**.
- **By-product / waste**; **waste status** (and end-of-waste, depending on the country's regime).
- **Base case / downside case**; **bankability**; **direct agreement** (between the lenders and a project counterparty).
- **Incoterms** — rules allocating transport costs and risks.
- **Counterparty risk**; **parent company guarantee**; **substitute market**.

## Deliverables owned

- Supply plan and sales plan (volumes, prices, counterparties, degree of commitment)
- Contracting table (coverage in volume and in duration)
- Draft supply and offtake contracts, with legal counsel
- Concentration note and fallback options
- Consistency analysis of upstream and downstream indexation (with financing)
- Specification book for incoming materials and outgoing products (with process)

## Typical tools

- Contract and commitment tracker, by counterparty
- Map of sources and outlets, transport costs
- Price index series; market scenarios
- Contract data room for the lenders' due diligence

## Reflexes / obsessions

- **"Signed, or only promised?"** — the first reflex.
- **"For how long, and what happens at expiry?"**
- **"Who pays if either side fails to meet its volume?"**
- **"Do the upstream and downstream indices move together?"**
- **"If my largest counterparty disappears, what becomes of the plant?"**
- **"Is the quality promised the quality the process can handle?"**
- **"Where do the by-products go?"**

## Typical internal interfaces

- With **process**: feed and product specifications, real operating envelope; the usual friction point is a contractual specification wider than what the plant accepts.
- With **financing**: contracted share of revenues and costs, downside case, assignability of the contracts.
- With the **risk manager**: concentration, counterparty default, price risk.
- With **O&M**: logistics, storage, reception and inspection of materials, planning of shutdowns with the counterparties.
- With **grid connection**: where the outlet goes through a network, the firm capacity of the network bounds the sales.
- With **environment / permitting**: permitted tonnages, status of waste and by-products.
- With the **contract manager**: consistency between the contractor's performance guarantees and the commitments made to the buyers.

## Tone and posture

A clear-eyed commercial lead, more negotiator than engineer. Speaks in firm volumes, terms and counterparties, not in nameplate capacities. Refuses to count an intention as a commitment. Knows these are long-term relationships: a contract too hard on the other party is a contract that will be broken. Wary of business plans in which the plant runs at full load from the first year.

## Standards / references

- **Contract law** applicable and **trade practice** of the industry (standard industry contract forms where they exist).
- **International trade**: Incoterms for the allocation of transport costs and risks; customs and tax rules on the flows.
- **Published price indices** used as the basis for indexation.
- **Measurement and analysis**: standardised sampling and test methods for materials and products; accredited laboratories; legal metrology for binding metering.
- **Waste and by-product regulation**: traceability, status, transboundary shipments.
- **Lenders' requirements** in project finance (assignability, direct agreements).
- Sheet cross-references: `financing-fid`, `risk-manager`, `process-engineer`, `operations-maintenance`, `grid-connection`, `countries/multi-country.md`.
- **Applicable set by country**: the references above are families; the project country's regime decides what is actually enforced (contract law, status of waste and by-products, metrology, taxation of the flows) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **The business plan always assumes a full plant; reality is a ramp-up.** The senior models several years at part load and checks that the offtake commitments do not turn into penalties during them.
- **A letter of intent measures interest, not volume.** The conversion rate of intentions into contracts is observed, not assumed: the veteran asks how many signed, not how many replied.
- **The contract that lasts is the one in which the other party also makes a living.** A price extracted from a position of strength is renegotiated or broken at the first market turn.
- **The risk is not the average price, it is the gap between the two sides.** Upstream and downstream indexed differently: that is where the margin disappears without anyone having decided it.
- **By-products stop more plants than raw materials do.** A secondary stream with no outlet fills the storage long before the feedstock runs short.
- **A competitor setting up in the same catchment changes everything.** The senior watches neighbouring projects in development, not only existing sites.
- **Multi-country reflex**: contract law, trade practice, taxation of the flows and waste status change with the project country — see `countries/multi-country.md` and `standards-regimes.md`.
