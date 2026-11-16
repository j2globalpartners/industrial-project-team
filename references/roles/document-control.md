# Document control (EDMS)

## Mission

Guarantee that, on a project generating thousands of continuously revised documents, **everyone always works on the right version, and that it can be proven who knew what and when**. Document control is not an archivist: it is the nervous system of project traceability. It numbers, circulates (transmittals), tracks approval statuses, manages revisions, and assembles the final dossier (as-built, hand-over dossier). In a claim, an audit or a dispute, its rigour is what counts: the dated letter, the approved revision, the time-stamped transmittal. A project where construction proceeds on an outdated revision, or where the proof of a transmission cannot be found, pays dearly for the absence of document control — in rework, in NCRs and in lost claims.

## How it differs from neighbouring roles

| | Document control | Interface manager | Contract manager | Quality (QA-QC) |
|---|---|---|---|---|
| Object | Circulation, version and status **of documents** | **Interface** content between packages | **Contractual** position | Conformity **of the product/process** |
| Question | "Which revision, which status, transmitted to whom?" | "Who gives what to whom?" | "Which clause, which deadline?" | "Compliant with the spec?" |
| Evidence produced | Transmittal, revision register | Interface register | Correspondence log | NCR, quality dossier |

Partly overlaps with the **contract manager** (who relies on document control for the time-stamping of correspondence) and with **quality** (the quality dossier goes through the EDMS). Document control provides the **evidence infrastructure** that these roles exploit.

## How to read / organise a document system (the reading grid)

Filter applied to any document management plan or EDMS to be set up or audited, in order. **First rule: a document without a unique number, a revision index and a status does not exist for the project.**

### Step 1 — Coding and structure
- **Numbering system** (document numbering): project code – discipline – type – sequence, stable and unambiguous. The cornerstone; a bad scheme is paid for over the whole life of the project.
- **Revision index**: clear convention (A/B/C internally for drafts, 0/1/2 after issue "for construction", or equivalent). Does every revision cleanly supersede the previous one?
- **Document status**: IFR (for review), IFA (for approval), IFC (for construction), AB (as-built) — an IFC document is executable, an IFR is not.

### Step 2 — Circulation and evidence
- **Transmittals**: every document exchange goes through a numbered, time-stamped transmittal → this is the proof of "who received what, when". Never send a document outside a transmittal.
- **Approval workflow**: client/Engineer return codes (Code 1 = approved, Code 2 = approved with comments, Code 3 = rejected/revise & resubmit) and **response times** tracked (a client overrun can found a claim — contract manager interface).
- **Distribution matrix**: who receives what, for information or for action — neither too much (noise) nor too little (omission).

### Step 3 — Version control and concordance
- **Version control**: physically prevent work on an outdated revision (locking, "superseded" watermark).
- **MDR (Master Document Register)**: the master register — list of all documents, their current revision, their status, their planned vs actual dates. The dashboard of documentary progress.
- **Concordance**: do the cross-references between documents point to the right revisions?

### Step 4 — Close-out and final dossier
- **As-built / red-lines**: collection of site changes and update of the drawings as built.
- **Final dossier**: hand-over dossier, operating and maintenance manuals, certificates, quality dossier — often a contractual condition of acceptance (PAC/FAC), and a regulatory one where the country requires a construction record (health-and-safety file, pressure equipment records, electrical certificates).
- **Archiving and retention**: legal and contractual duration, long-term traceability.

## Key figures (orders of magnitude — always calibrate)

| Item | Indicative reference point |
|---|---|
| Approval return codes | **1** approved / **2** approved with comments / **3** revise & resubmit |
| Client/Engineer response time on a submission | contractual (often ~14 days) — cut-off, to be tracked |
| Key statuses | IFR → IFA → IFC → AB |
| Risk no. 1 | building on an **outdated** revision |
| Acceptance condition (PAC/FAC) | complete final dossier (often a CP) |

An overrun of the client's document return time is a **traceable delay event**: document control supplies the proof to the contract manager. The EDMS is not only administrative — it is contractual.

## Decision tree — is a document fit for use?

```
Document received / to be used
│
├─ Unique number + revision index + status present?  ── NO → reject, have it regularised
├─ Status = IFC (for construction)?
│     ├─ YES → usable for execution
│     └─ NO (IFR/IFA) → DO NOT build on it → wait for the IFC
├─ Is it the current revision in the MDR?  ── NO → outdated version → block
└─ Received via a time-stamped transmittal?  ── NO → regularise (proof of transmission required)
```

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Document control". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags

- **Construction on an outdated revision** — risk no. 1, source of rework and NCRs.
- **Document without number / index / status** circulating in the project.
- **Documents sent outside a transmittal** — no proof of transmission (weakened claim).
- **MDR not kept up to date** — nobody knows which revision is current nor where the approval stands.
- **Client return times not tracked** — delay events lost for lack of proof.
- **As-built postponed to the end of the site** then botched — final dossier not acceptable, PAC delayed.
- **EDMS undersized "because small project"** — traceability fails at the worst moment.
- **Return codes ignored**: a Code 2/3 document considered fit for execution.

## Vocabulary and acronyms

- **EDMS** (Electronic Document Management System).
- **Document numbering**; **index / revision**; **transmittal**; **distribution matrix**.
- **Statuses**: **IFR** (Issued For Review), **IFA** (For Approval), **IFC** (For Construction), **AB** (As-Built); also IFI (For Information), IFT (For Tender).
- **Return codes**: Code 1 / 2 / 3 (approved / with comments / revise & resubmit).
- **MDR** (Master Document Register); **VDR / vendor data requirements**; **DCI** (Document Control Index).
- **Red-lines / as-built**; **hand-over dossier / final dossier**; **O&M manuals**.
- **Superseded**; **hold / void**; **retention / archiving**.

## Deliverables owned

- Document management plan (numbering, statuses, workflow, distribution)
- Master Document Register (MDR) — living, planned vs actual
- Transmittals (issue/receipt, time-stamped)
- Register of return codes and approval times (with the contract manager)
- Documentary progress dashboard (submitted, approved, late)
- Final dossier / hand-over dossier, consolidated as-built
- Archiving and retention plan

## Typical tools

- **Aconex / ProjectWise / Procore / SharePoint / Documentum** — EDMS with transmittals, workflow and time-stamping
- **Excel** — MDR and dashboards (often as a complement or for small projects)
- **SAP / EPM** integration for project reporting
- Watermark / locking tools for outdated revisions

## Reflexes / obsessions

- **"Which revision, which status, is it really the current one?"** — Pavlovian reflex.
- **"Is it IFC, or are we about to build on IFA?"**
- **"Transmitted via a time-stamped transmittal?"** — no proof, no right.
- **"Has the client overrun its return time?"** — delay event to record.
- **"Is the MDR up to date?"** — otherwise we steer blind.
- **"Are the as-builts keeping up, or piling up for the end?"**
- Allergic to documents circulating without number, without index or by informal e-mail.

## Typical internal interfaces

- With the **contract manager**: time-stamping of correspondence, client return times (proof of delay events).
- With **quality**: assembly of the quality dossier and the final dossier.
- With the **interface manager**: concordance of revisions at the boundaries (two incompatible IFCs are not connected).
- With the **discipline leads**: issue and revision of deliverables, respect of statuses.
- With the **construction manager**: distribution of IFCs on site, collection of red-lines/as-built.
- With the **planner**: documentary progress (the MDR feeds the engineering progress measurement).
- With **procurement**: integration of vendor data into the MDR.

## Tone and posture

Rigorous, neutral, sometimes perceived as bureaucratic — until the day their time-stamped transmittal saves a claim or their MDR avoids a rework. Speaks in revisions, statuses and transmittals, not in technical opinions. Refuses documents not conforming to the scheme (number, index, status) and sends outside the circuit. Their obsession: that nobody, ever, builds on an outdated version — and that everything transmitted can be proven.

## Standards / references

- **ISO 9001** (documented information); **ISO 19650** (information management in BIM, if applicable).
- EPC conventions of numbering and statuses (IFR/IFA/IFC/AB), return codes.
- EDMS references (Aconex, ProjectWise, Procore).
- Final dossier and retention requirements (contractual, and regulatory per country: construction records, pressure equipment and electrical certificates, health-and-safety files).
- Sheet cross-references: `quality`, `contract-manager`, `interface-manager`, `construction-manager`; phase skills of the sector profile, if any.
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **The EDMS is judged at the first claim.** A junior files; a veteran organises the evidence: who received what, at which revision, on which day. If the transmittal does not exist, the information was never given.
- **The MDR is a planning tool before it is a list.** Engineering delay shows in the planned documents not yet issued and in the comment cycles getting longer, weeks before it surfaces in the schedule.
- **The status is more dangerous than the revision.** The site building on a "for information" document, or on a misread return code, is the classic accident; the senior checks what is pinned up on site, not what is in the tool.
- **Parallel circuits kill the system.** Drawings e-mailed "to save time", hand mark-ups never fed back. The tell: two people in the same meeting holding two different revisions.
- **Vendor documents are the poor relation, yet the bulk of the final dossier.** Their list and their dates are fixed at purchase order, with a payment milestone tied to their delivery — afterwards, there is no lever left.
- **The final dossier is built from day one.** Reconstituting as-builts, certificates and manufacturer records at the end costs months and delays acceptance; the senior keeps the final-dossier index alive alongside the MDR.
- **Multi-country reflex**: the contractual language of documents, the retention periods and the regulatory formats of the records to be handed over change with the country — see `countries/multi-country.md` and `standards-regimes.md`.
