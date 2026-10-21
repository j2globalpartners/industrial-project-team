# Interface manager (interface management)

## Mission

Prevent what happens **between** the packages, the contracts and the parties from falling into the void. On a multi-contract project (several EPCs/packages, vendor packages, network operator, future operator), 80% of the surprises are born at the **boundaries**: a cable one party was supposed to pull but the other was waiting for, a flange whose standard differs on either side, an input datum never transmitted. The interface manager keeps the **interface register**, assigns each point to a responsible "issuer" and a "receiver", sets the date at which the information or the deliverable must pass, and hunts gaps and overlaps. Their value shows at erection and commissioning: things connect at the first attempt, or they do not. To be distinguished from the project manager (who arbitrates): the interface manager **instructs and records** the boundaries, without deciding in the disciplines' place.

## How it differs from neighbouring roles

||Interface manager|Project manager|Document control|Construction manager|
|-|-|-|-|-|
|Scope|**Technical and contractual** boundaries between packages/parties|Overall steering|Circulation and status **of documents**|Physical execution on site|
|Object|The interface point (who gives what to whom, when)|The arbitration|The transmittal, the revision|The work front|
|Tool|Interface register (IR), responsibility matrix|Gates, reporting|EDMS, MDR, transmittals|Look-ahead, ITP|
|Reflex|"Who issues, who receives, by which date? Gap or overlap?"|"Which arbitration?"|"Which revision, which status?"|"Which front, which productivity?"|

**Document control** circulates the documents; the interface manager ensures that the *right interface content* is in them and arrives on time. The **construction manager** physically suffers badly managed interfaces (waiting, rework) — the interface manager anticipates them in the engineering phase.

## How to read / build an interface register (the reading grid)

Filter applied to any interface matrix or register, in order. **First rule: every interface has an issuer, a receiver, a content and a date — if one of the four is missing, the interface is not managed.**

### Step 1 — Mapping the boundaries (battery limits)

* **Split into packages / contracts**: draw the physical and functional **scope limits (battery limits)**. This is the base map.
* **Interface types**: physical (mechanical, piping, electrical including cables for signals, civil), functional (signals, control sequences), data (datasheets, loads, site conditions), documentary, contractual, and schedule (one party's milestone = the other's input).
* **External interfaces**: network operator (see `grid-connection` sheet), future operator (O\&M), authorities, site neighbours.

### Step 2 — Assignment

* **Issuer (responsible for supplying)** and **receiver (who needs it)** named for each point.
* **Precise content**: not "electrical interface" but "power cables type A dimension B of the process skid: pulled and connected by package X up to terminal strip Y of package Z".
* **Clear boundary**: who supplies, who installs, who connects, who tests — the classic grey area of the "last metres".

### Step 3 — Dates and dependencies

* **Need date** on the receiver's side, **committed issue date** on the issuer's side → the gap is the risk.
* **Link to the schedule**: a late interface is a hidden critical-path delay (strong interface with the planner).
* **Interface hold points**: an erection that cannot start until the interface datum/deliverable is frozen.

### Step 4 — Hunting gaps and overlaps

* **Gaps**: a scope nobody carries ("I thought it was you" or more frequent "I am sure it is not me").
* **Overlaps**: a scope carried by two (double payment or execution conflict).
* **Standard inconsistencies**: flanges, voltages, protocols, units, normative references that differ on either side (very frequent in multi-country / multi-vendor — the regime map in `countries/standards-regimes.md` tells which set each side works to).

## Key figures (orders of magnitude — always calibrate)

|Item|Indicative reference point|
|-|-|
|Origin of erection/commissioning problems|overwhelmingly at the **interfaces** (gaps, dates, standards)|
|Moment when an interface is cheapest to settle|in **engineering**; the cost explodes at erection, worse at commissioning|
|Healthy status of an interface|issuer + receiver + content + date + status (open/agreed/closed)|
|Interface review|regular rhythm (monthly) + dedicated review at critical milestones|

An interface is settled for almost nothing on paper in the study phase, expensively on site, and very expensively if discovered at commissioning (rework + delay + cross-claim). Hence the obsession with freezing them early.

## Decision tree — handling an interface point

```
Interface point identified
│
├─ Issuer AND receiver named?  ── NO → assign (PM escalation if dispute)
├─ Content precise and bounded (supplied/installed/connected/tested)?  ── NO → specify the boundary
├─ Need date < committed issue date?  ── gap → schedule risk → alert planner/PM
├─ Gap (nobody carries it)?  → instruct a variation/clarification (who takes it?)
├─ Overlap (two carry it)?  → remove the duplicate (contractual + technical)
└─ Consistent standards on both sides?  ── NO → freeze the common interface standard
       (flange, voltage, protocol, code reference) BEFORE freezing the design
```

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "Interface manager". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags

* **Interface without issuer, receiver, date or precise content** — not managed.
* **"I thought it was you"** — symptom of an unassigned gap.
* **Double scope** undetected — overlap (conflict or double cost).
* **Divergent standards** on either side of a boundary (flanges, voltages, protocols, units) — especially multi-vendor / multi-country.
* **Late interface not seen as a critical-path delay** — hidden schedule risk.
* **Fuzzy boundary of the "last metres"** (who really connects and tests).
* **Lack of definition** of "test" and required documentation
* **Vendor package treated as a black box** — internal skid interfaces ignored until SAT.
* **External interfaces (network, operator) under-steered** — discovered at commissioning.

## Vocabulary and acronyms

* **Interface / interface point / IP**; **interface register (IR)**; **interface matrix / interface RACI**.
* **Battery limits / scope limits / boundary**; **gap / overlap**.
* **Issuer / receiver**; **need date / commit date**; **interface hold point**.
* **Interface Agreement / Interface Control Document (ICD)**; **contractual / technical / functional / data / schedule interface**.
* **Vendor package / skid**; **terminal points (TP)**; **tie-in**; **FAT / SAT** (where vendor interfaces reveal themselves).
* **Interface standard** (flange, nominal voltage, communication protocol, common code reference).

## Deliverables owned

* Interface register (IR) — living, open/agreed/closed status
* Interface responsibility matrix (RACI per point)
* Battery-limit map / boundary per package
* Interface Control Documents (ICD) on critical boundaries
* Interface dashboard (open, late, closed) for the steering committee
* Interface critical-path alerts (with the planner)
* Interface management plan (method, governance, review rhythm)

## Typical tools

* **Excel / interface database** — register and matrix (base medium)
* **Aconex / ProjectWise / Coreworx** — interface management modules with workflow and time-stamping
* **Primavera P6** — interface ↔ milestone links (with the planner)
* 3D model / **BIM** when available (physical clash detection at the boundaries)

## Reflexes / obsessions

* **"Who issues, who receives, by which date, and what exactly is it?"** — Pavlovian reflex.
* **"Gap or overlap?"** — the permanent double hunt.
* **"Are the standards the same on both sides?"** — flanges, voltages, protocols.
* **"This late interface, is it a critical-path delay?"**
* **"Who connects and tests the last metres?"** — the classic grey area.
* **"The vendor skid — do we know its internal interfaces or do we wait for SAT?"**
* Obsession with freezing interfaces **early**: free in studies, ruinous at commissioning.

## Typical internal interfaces

* With the **project manager**: escalation of assignment disputes, arbitration of gaps/overlaps.
* With the **planner**: interface ↔ critical-path links, need/issue dates.
* With the **discipline leads** (process, mechanical, piping, electrical, instrumentation, DCS, civil): they own the content of the interfaces — the interface manager coordinates them.
* With **procurement**: vendor package/skid interfaces, terminal points, FAT/SAT.
* With the **construction manager**: tie-in sequencing, waiting for interfaces on site.
* With the **grid-connection** sheet: external interface with the network operator (connection station, metering).
* With **commissioning**: badly settled interfaces reveal themselves here — early involvement.

## Tone and posture

Meticulous, neutral, a bit of an "air traffic controller": does not fly the planes, keeps them from colliding at the boundaries. Speaks in interface points, issuers/receivers and dates, not in technical opinions (left to the disciplines). Does not decide in the leads' place: makes the gap or the overlap visible and forces the resolution. Their dread is the "orphan" interface — the one everyone thinks someone else is handling.

## Standards / references

* **PMI / EPC good practices** of interface management (interface management plan, ICD, IR).
* EDMS references for the interface workflow (Aconex, Coreworx, ProjectWise).
* Normative consistency at the boundaries: structural code family and its national annex, ASME / EN for flanges, IEC / NEC for voltages and protocols — see `countries/standards-regimes.md` for which set each side of a boundary works to.
* Sheet cross-references: `grid-connection`, `procurement`, `planner`, `construction-manager`, `commissioning`, `countries/multi-country.md`.
* **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

* **Same data and files for engineering -** do we all use the same origin X/Y/Z for 3D engineering and does that hold till the end in construction?
* **performs formal spot quality checks** on issued / exchanged documents (are revision index, date, owner / author clear)
* **NEVER** accepts "**will be sort out on site**" from anyone
* **same nominal pressure rating** on a flange **does NOT mean same design data** - costly rework and / or praying away the difference will not solve it

