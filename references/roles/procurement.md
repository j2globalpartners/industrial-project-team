# Procurement / purchasing / supply chain

## Mission

Buy, have manufactured, have delivered to site — on time, at the required quality, at the best cost and in compliance with the contract — all the project's equipment, bulk materials, services and subcontracts. On an EPC, procurement is the **heaviest budget item** (50-70% of the capex in equipment + bulk + subcontracting) and the most exposed to cost AND schedule risk: a long-lead item ordered late shifts the whole commissioning.

## How it differs from neighbouring roles

||Procurement|Engineering (lead discipline)|Contract manager|Cost controller|
|-|-|-|-|-|
|Decides|The **commercial** (vendor, price, lead time)|The **technical** (TBE: compliant or not)|The main client contract|The cost forecast|
|Question|"Which vendor? which price? which ROS?"|"What is needed? Technically acceptable?"|"Which clause? which notification period?"|"Where do we land? When is which amount due?"|
|Deliverable|CBA, PO, expediting|MR, RFQ, TBE, vendor document review|Claims, variations, bonds|EAC|

Sacred boundary: **engineering decides the technical (TBE), procurement decides the commercial (CBA)**. A technically non-compliant vendor is never awarded because it is cheaper. And **back-to-back** with the contract manager: the obligations suffered on the client side (LD, guarantees, indemnities) must be passed down into the POs.

## How to read a vendor bid / build a CBA (the grid)

The heart of the trade. Comparing "raw" bids is a trap: they carry neither the same scope, nor the same INCOTERM, nor the same exclusions. Prices are never compared — **normalised TCOs** are.

### Step 1 — Bring everyone onto the same line

* **Same INCOTERM**: bring everything back to a common delivery point (often DAP/DDP site). A "cheaper" EXW bid costs more delivered.
* **Same scope**: re-inject each bid's exclusions — transport, seaworthy packing, taxes/customs, spare parts (commissioning + 2 years of operation), erection and commissioning supervision (in man-days), special tools, first fill, training, documentation.
* **Register of commercial deviations**: every "clarification" or reservation a vendor takes on your general conditions **transfers a risk to you**. To be quantified or closed in negotiation. A "cheap" bid with 30 reservations is not the cheapest.

### Step 2 — Build the total cost of ownership (TCO)

Purchase price **+** transport/logistics **+** customs/taxes **+** spares **+** supervision **+** escalation (if long lead time) **+** financial cost of the payment terms (a heavy down payment has a cash cost — discount it) **+** for rotating / energy-intensive equipment, the **life-cycle cost** (energy consumption, maintenance over the life — a compressor 2% less efficient costs more than the purchase-price gap, superior performance in quality).

### Step 3 — Lead time and guarantees

* **ROS vs announced lead time + margin**: a low price that breaks the site is worth nothing. Check the credibility of the lead time (factory order book, not the sales promise).
* **Delay LDs**: rate, cap (often 10% of the PO) — and above all: does that cap cover the **real damage** a delay causes to the site? 10% of a small PO does not cover the standby it triggers. Too agressive delay causes may not stand in court, these need to be reasonable and balanced.
* **Bank guarantees**: performance bond, advance payment bond (before any down payment!), warranty bond.

## Procurement lead times — long-lead items (orders of magnitude)

These lead times drive the schedule: this equipment is ordered **first**, often before the complete design freeze. Very volatile with the market (HV transformers exceeded 24 months after 2021).

|Equipment|Indicative manufacturing + delivery lead time|
|-|-|
|Turbines (gas / steam)|18–30 months|
|Centrifugal compressors|12–24 months|
|HV transformers / GIS|12–24 months (sometimes > 24)|
|Reactors, cryogenic equipment|18–24 months|
|Columns / special vessels (alloys)|10–18 months|
|Special exchangers|10–16 months|
|Special API 610 pumps|9–14 months|
|Severe-service / large-diameter valves|9–16 months|
|MV/HV switchgear|8–14 months|
|DCS / control system|9–12 months|

**Sector-specific long-lead items** (process core, licensed equipment, network delivery station) are listed in the sector profile — often driven by a third party's schedule (network operator, licensor) as much as by the supplier.

## INCOTERMS 2020 — the transfer grid

Who pays what, and where the risk switches. Most costly confusions: **FCA vs FOB** (FOB reserved for conventional sea freight, misused for containers → use FCA), **DAP vs DDP** (DDP = the vendor clears import customs and pays the duties; rarely desirable, the vendor knows the local tax rules poorly), **CIF/CIP** (insurance at the legal **minimum** — often insufficient, require extended cover).

|Family|Terms|Risk transfer|
|-|-|-|
|Departure|EXW|At the vendor (the buyer handles everything)|
|Main carriage unpaid|FCA, FAS, FOB|At loading|
|Main carriage paid|CPT, CIP, CFR, CIF|To the carrier (but cost paid to destination)|
|Arrival|DAP, DPU, DDP|At destination (DDP = duties included)|

## Decision tree — award (recommendation to award)

```
Bids received
│
├─ 1. Engineering TBE: which bids are TECHNICALLY compliant?
│      → discard the non-compliant (no catching up by price)
│
├─ 2. Among the compliant: CBA on normalised TCO
│      → rank by evaluated total cost, not by purchase price
│
├─ 3. Commercial deviations of the best bidder: acceptable?
│      → no → negotiate / close, or move to the next one
│
├─ 4. Vendor capacity \& health: order book, financials,
│      track record on THIS service, factory load at ROS time
│      → a vendor in financial difficulty on a long-lead item = major risk
│
└─ 5. Justified single source? (proprietary, lead time, fleet standardisation)
       → document the single-source justification (ethics / audit)
```

**Make-or-buy / packaging** upstream: group into packages large enough to interest first-tier vendors, without creating a single point of failure on a critical package.

## Vendor criticality matrix → expediting and inspection effort

The intensity of the follow-up is calibrated; bolting is not handled like a compressor:

* **Criticality A** (long-lead, on the critical path, complex manufacturing) → **level 3 expediting** (resident at the factory) + inspection at hold points + witnessed FAT.
* **Criticality B** (moderate impact, medium lead time) → **level 2** (periodic factory visits) + inspection at key points.
* **Criticality C** (standard bulk, multi-sourced) → **level 1** (desk/phone follow-up) + receiving inspection.

Criteria: schedule impact × manufacturing complexity × vendor track record × supply risk. increase criticality by one if one the criteria is red.

## Key responsibilities

### Strategy and preparation

* **Procurement strategy / plan** — make or buy, packages, contracting modes (lump sum, unit rate, cost reimbursable).
* **Procurement schedule** — aligned with the schedule, ROS (Required On Site) milestones worked back from the long-lead times not revealed to the vendor, always include a margin (included in the schedule) but know the ROS!
* **AVL** — Approved Vendor List, qualified with the client and quality; critical for long-lead items.
* **Procurement procedures** — ethics, segregation of duties, traceability of decisions.

### Purchasing cycle

PR (with technical MR) → RFQ to qualified vendors → TBE (engineering) + CBA (commercial) → negotiation → firm **PO** → **expediting** → **inspection** (with quality: FAT, hold/witness points) → **logistics** (packing, transport, customs) → **receipt** (goods receipt in the ERP, reservations) → invoicing/payment by milestones → close-out (warranties, archiving).

**Typical payment milestones**: down payment 10–15% (against bond), \~30% on material procurement / approved drawings, \~40% on successful FAT, \~15% on site delivery, balance + retention (5–10%) on final acceptance.

### Vendor documentation

* **Vendor Document Register (VDR)** — all expected documents (drawings, calculations, manuals, certificates).
* **Flow tracking** — review by discipline, A/B/C codes (approved / approved with comments / rejected), vendor returns. A document not returned = risk of stoppage at receipt.

## Red flags — the hunt

* **Lowest price AND shortest lead time** from the same bidder → often unrealistic, the vendor "buys the market" and will catch up through claims.
* **List of commercial exceptions** buried in the vendor's general terms → risk transfer through the back door.
* **Down payment without advance payment bond** → down payment lost in case of default.
* **LD cap too low** vs the site damage a delay triggers.
* **Scope gaps** MR/TBE vs bid: spares, supervision, first fill, tools, transport, taxes "excluded".
* **"Or equal"** / unapproved sub-suppliers slipped into manufacturing without re-validation.
* **Performance guarantee values** without proper description of performance run and measurement / determination of methodologies.
* **Single point of failure** (one vendor, one factory, one transport route) on a critical long-lead item.
* **Vendor financial health**: a bankruptcy during manufacturing of a long-lead item is catastrophic → check the accounts on long-lead-time markets.
* **Unhedged FX exposure** on a PO in foreign currency.
* **Refurbished components** presented as new.

## Vocabulary and acronyms

* **PR / RFQ / PO / VOR** — Purchase Requisition / Request For Quotation / Purchase Order / Variation Order Request
* **MR / TBE / CBA** — Material Requisition / Technical Bid Evaluation / Commercial Bid Analysis
* **ITT / ITB** — Invitation To Tender / Bid; **NDA** (sensitive technology)
* **AVL / VVL** — Approved / Validated Vendor List
* **ROS / ETD / ETA** — Required On Site / Estimated Time of Departure / Arrival
* **TCO** — Total Cost of Ownership
* **INCOTERMS 2020** — EXW, FCA, CPT, CIP, DAP, DPU, DDP (any mode) / FAS, FOB, CFR, CIF (sea)
* **L/C** — Letter of Credit; **B/L** — Bill of Lading; **CMR** — road consignment note
* **COC / MTR** — Certificate of Conformity / Material Test Report
* **VDR / VDB** — Vendor Document Register / Database
* **Expediting** — levels 1 (desk) / 2 (visits) / 3 (resident)
* **LD** — Liquidated Damages; **Performance / Advance payment / Warranty bond**
* **Long lead items** — critical equipment with long lead times; **Bulk** — materials in quantity
* **Backcharge** — re-invoicing to the vendor of a cost it should have borne
* **Force majeure** — exonerating clause

## Deliverables owned

* Procurement Plan / Strategy; Procurement Schedule (with ROS)
* Approved Vendor List; RFQ packages
* Commercial Bid Analysis (CBA on TCO); Recommendation to Award
* Signed Purchase Orders; Expediting reports; Logistics Plan
* Vendor Document Register (with engineering)
* Monthly procurement status report; Claims / backcharge log; Close-out report

## Typical tools

* **SAP MM** — reference (PR, PO, GR, IR)
* **Ariba, Coupa, Jaggaer** — e-procurement / electronic RFQs
* **Aconex, ProjectWise** — vendor document management
* **Primavera Unifier** — procurement workflows
* Excel — still king of CBAs and trackers

## Reflexes / obsessions

* **"Are we in the AVL? Vendor pre-qualified for THIS service?"** — no award without qualification.
* **"ROS tenable with this vendor?"** — a low price is useless if the lead time breaks the site.
* **"TCO or purchase price?"** — normalise before comparing.
* **"Clear INCOTERM, who handles transport and risk?"** — frequent FCA / FOB / DAP confusion.
* **"Payment terms vs project cash flow?"**
* **"Bank guarantees in place before the down payment?"**
* **"LDs capped, and cap compatible with the risk?"**
* **"Quality hold points defined in the ITP?"**
* **"VDR up to date? Return codes handled?"**
* **"Backcharge preserved if vendor default?"**
* **"Vendor financial health checked on this long-lead item?"**
* Wary of "small" suppliers without a track record on critical equipment, even when cheaper.

## Typical internal interfaces

* With the **project manager**: recommendation to award, purchasing strategy, supplier claims.
* With the **cost controller**: commitments, accruals, payments, PO variations, FX exposure.
* With the **planner**: ROS dates, vendor drift, critical-path impact.
* With the **discipline leads**: MR, TBE, vendor document review, hold/witness points.
* With **maintenance**: track record of own experience and awareness of TCO
* With **quality**: vendor qualification, ITP, inspection, vendor NCRs.
* With **construction / logistics**: transport, unloading, site storage, delivery sequence.
* With the **contract manager**: back-to-back, vendor claims and backcharges, guarantees.
* With **finance**: L/C opening, international payments, FX hedging.

## Tone and posture

Pragmatic, a negotiator, attentive to contractual detail. Not easily impressed by vendor talk. Asks for evidence (references, certifications, audits, accounts) rather than claims. Methodical on traceability. Strictly distinguishes the technical decision (engineering) from the commercial decision (their own). Their compass: compliance, lead time, total price, risk — in that order when the equipment is critical. Fair and knows who the own - flexibility and a reliable relationship with a professional vendor is worth a lot more than a small amount of money saved and risking unexpected down times during operation.

## Standards / references

* **INCOTERMS 2020** (ICC) — international commercial terms
* **ISO 9001** — quality (vendor qualification); **ISO 20400** — sustainable procurement
* **UCP 600** — uniform customs and practice for documentary credits (L/C)
* **Vienna Convention (CISG)** — international sale of goods
* **FIDIC** and national contract forms — EPC contract side (back-to-back)
* **AACE RP 56R-08** — estimate classification (purchasing budget link)
* **Owner standards** — qualified vendor lists and procurement procedures specific to each major
* **Public procurement rules** where the buyer is public (EU directives, FAR in the US, national codes)
* **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

* **On long-lead items, the lead time drives the purchase, not the price.** The sector's long-lead equipment (listed in the active profile) is often driven by the operator / vendor: place the long orders early, even at the cost of a reservation fee.
* **Back-to-back is the project's life insurance.** What the client contract imposes (LD, guarantees) must flow down to the suppliers (contract manager link): a subcontractor without LDs = uncovered risk.
* **The lowest bidder is not the best.** A cheap but unreliable or insolvent vendor costs dearly in operation and in warranties: qualify (supplier panel / after-sales link), not only compare prices.
* **Vendor data and FAT/SAT are contracted.** A supplier delivering without documentation or FAT blocks erection and commissioning (document control, interface manager links).
* **Solvency and local after-sales are criteria, not details**: a failure without nearby after-sales = long unavailability (O\&M link).
* **Multi-country reflex**: supplier panel, after-sales, posting of workers, VAT and customs of the contracts vary by country — and the code of the destination regime decides what a certificate must show — see `countries/multi-country.md` and `standards-regimes.md`.
* **Exclusions** are more relevant than was is included.
* **DDP excludes unloading and intermediate storage (if required):** eventual liability gap if installation is included but unloading done by third party or owner
* **Most saving is in the RFQ** (hidden margins on performance and design, not clarified requirements, expensive materials, unclear interfaces) - supports leads in sorting out before contacting vendor

