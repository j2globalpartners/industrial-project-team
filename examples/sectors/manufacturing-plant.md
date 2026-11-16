# Sector profile — Manufacturing plant (pharma, food, aerospace, automotive, batteries, electronics)

> **Example profile — unreviewed.** Written as an illustration of the expected density of a sector profile, from general industry knowledge, not from field practice validated by the author. Figures are indicative; regulatory references are given by family with examples, to be replaced by the project country's set (`countries/standards-regimes.md`). To use it: copy into `references/sectors/manufacturing-plant.md`, then review every line with a practitioner.

## Sector identity card

- **Object**: industrial building + **production lines** (machines, robots, conveying, cleanrooms, utilities) to manufacture a **product** in series — not to transform a continuous flow. The project is **driven by the product and its qualification**: what counts is the start-of-production date (SOP) with a qualified process, a compliant yield and rate, more than the building itself. Variants: new plant (greenfield), extension, new line in an existing site, production transfer.
- **Typical scale**: from a few M€ (one line) to several billion (gigafactory). Business case → SOP: 2 to 4 years, with a **ramp-up** of 6 to 24 months after SOP. Team: project manager, industrialisation / methods, process (line OEMs), building & utilities, quality / qualification, automation, HSE, purchasing — often as **in-house owner** with an EPCM or a building design firm.
- **Dominant contract models**: **separate packages** — **building** (civil / trades, design firm, design-build or trade packages) and **process** (supply and erection of the lines by the OEMs, with FAT / SAT and rate, yield and availability guarantees); **EPCM** or owner's engineer to integrate; framework contracts with the OEMs; the property insurer (FM Global HPR-type) as a quasi-contractual prescriber; **utilities** (HVAC, cleanrooms, clean utilities) as a critical separate package.
- **Life cycle & gates**: `BUSINESS CASE (capacity, product, site) → CONCEPT / BASIC (layout, flows, URS) → DETAILED DESIGN → BUILDING CONSTRUCTION + LINE MANUFACTURING (FAT) → INSTALLATION / SAT → QUALIFICATION (IQ / OQ / PQ) → RAMP-UP → SOP`. In pharma: **DQ / IQ / OQ / PQ**, process validation (PPQ), regulatory inspection (EMA / national agencies, FDA) before the commercial batch; in automotive / aerospace: **APQP / PPAP**, FAI (AS9102), customer approval. AACE classes: 4 at business case, 3 at basic, 2 at purchase launch.
- **Regulatory framework and permits** (by family; the country decides the set): building permit and **land use** (zoning, land take); **classified-installation permitting** according to the activities (metals, painting, battery charging, solvents, storages; chemicals — batteries and pharma can reach major-hazard thresholds); **workplace design and machinery safety** (EU Machinery Directive 2006/42/EC → Regulation (EU) 2023/1230 applicable in 2027, CE marking of the lines; OSHA / ANSI B11 in the US); **fire** (sprinklers, smoke extraction, compartmentation — insurer's requirements, NFPA in the US); **GMP** (EU GMP annexes 1 and 15, GAMP 5, 21 CFR Part 11, ISO 14644 for cleanrooms); **food hygiene** (IFS / BRC, EHEDG, FDA FSMA); **EN 9100 / NADCAP** (aerospace); **IATF 16949** (automotive); chemicals regulation (REACH, TSCA); major-hazard regime where applicable. Country cards: `countries/`.
- **Key external counterparts**: **line OEMs** and integrators, building design firm and building inspection body, **insurer**, authorities (municipality, environmental authority, labour inspectorate, medicines agency for pharma, food safety authority), **customers** (approval), local authority and developer (land, industrial estate), electricity and gas network operators (utilities), notified bodies (CE marking).
- **FID locks / long poles**: **land and permits** (land take, classified installations), **electrical connection** (modern plants are electricity-intensive: HV frequent), **line long-lead** (12–24 months, saturated OEMs), **HVAC / cleanrooms** (long-lead and critical path of the qualification), **qualification / approval** (pharma, aerospace: the SOP date depends on an inspector or a customer), **recruitment and training** of operators.
- **Economics & revenue**: installed capacity (parts / yr, t / yr, GWh / yr), **OEE** (availability × performance × quality), **yield** at ramp-up, unit cost, **time-to-market** (each month of SOP delay = lost turnover and sometimes customer penalties); grants (national investment programmes, regional aid, IPCEI, US IRA / CHIPS) with conditions; balance-sheet financing most often.
- **Roles to activate in addition**: **Industrialisation & qualification engineer** and **HVAC / cleanroom & clean utilities engineer** (below). Renamed roles: **process → lines and flows** (with the OEMs); **DCS → automation / MES / SCADA**; **piping → utilities** (including clean utilities); **grid connection → utilities and energy**; **commissioning → SAT + qualification**. Lightened roles: materials (hygienic / 316L), geotechnical (standard), technical safety (except major hazards).
- **Phase skills and references available**: no dedicated phase skill; the cross-cutting skills (claims / EOT, cost control, contractual letters and minutes, multi-package reconciliation — very suited to building / process packages, specifications, annex simplification, visual management, gate war-game) apply as they are.
- **Common units & ratios** (indicative): capacity in units / h, **takt time**, **OEE** (world class ~85%, ramp-up 40–60%), yield (%), floor area (m² per line, process / logistics / support ratio), cleanliness classes (ISO 5 to ISO 8; grades A–D in pharma), dry-room dew point (batteries: −40 to −60 °C), electrical power in MW (often 5 to 50 MW, > 100 MW in a gigafactory), €/m² of building, € per unit of capacity, ramp-up curve in months.
- **Key vocabulary**: URS (user requirements specification), FAT / SAT, IQ / OQ / PQ, PPQ, validation, GAMP 5, data integrity, MES, SCADA, OEE, takt, yield, ramp-up, SOP (start of production), FAI, PPAP, APQP, cleanroom, dry room, flows (product, personnel, waste), layout, clean utilities (WFI, purified water, clean steam, compressed air), HVAC, ISO classification, EHEDG, hygienic design, CE marking, machinery directive / regulation, HPR insurer, sprinklers, land take.

## Sector-specific roles

### Industrialisation & qualification engineer
- **Mission**: accountable for the **qualified capacity at the SOP date** — translates the product into URS, selects and steers the OEMs, runs FAT / SAT and the **qualification** (IQ / OQ / PQ or PPAP / FAI), and holds the ramp-up curve.
- **Reading grid of an OEM line offer**: (1) scope vs URS (what is missing is on you); (2) **guaranteed rate and OEE**, test method (duration, reference product, definition of stoppages); (3) guaranteed yield and scrap rate; (4) interfaces (utilities, automation, MES, machine safety); (5) FAT / delivery / SAT lead times and qualification plan; (6) CE documentation and qualification dossier supplied; (7) spare parts and training.
- **Anchors (indicative)**: ramp-up OEE 40–60% vs nominal 75–85%; pharma qualification duration 3–9 months after SAT; FAT at the OEM = 60–80% of problems detected before the site.
- **Red flags**: URS written after consulting the OEMs; rate guaranteed without a definition of stoppages; qualification not planned as a phase of its own; ramp-up absent from the business case.
- **Senior eye**: "a process is qualified, not a machine" — they have it tested with the real product, the real operators and the real utilities, and know that the first year of production is the real acceptance test.

### HVAC / cleanroom & clean utilities engineer
- **Mission**: accountable for the **ambient conditions** (cleanliness class, temperature, humidity, dew point, differential pressures) and the **clean utilities** — often the real critical path of the qualification.
- **Grid**: (1) classification and pressure cascade per zone; (2) thermal and humidity balances (internal load of the machines often underestimated); (3) air change rates and filtration (HEPA); (4) clean utilities (WFI, purified water, clean steam, compressed air, gases) — materials (electropolished 316L, ASME BPE), loops, sanitisation; (5) monitoring and alarms (EMS); (6) qualification plan (ISO 14644 tests, filter integrity).
- **Red flags**: HVAC plant sized on the empty building; dry-room dew point promised without a load test; clean utilities outside the ITP.
- **Senior eye**: a cleanroom is qualified in summer and in winter — a class test passed in April says nothing about August.

## Role inserts

### Project manager
- The project is judged on the **SOP date with a qualified process**: the two chains — building / utilities and lines / qualification — must converge, and it is the **integration** (building ↔ process ↔ automation ↔ quality interfaces) that makes or breaks the date; the PM holds the **layout and the flows** frozen early (every machine move ricochets on the utilities and the floor).
- Red flags: SOP promised to the customer / the grant without qualification or ramp-up margin; layout changed after the lines are ordered; operator recruitment launched after SAT.

### Estimator
- Break down building (€/m² by zone type: logistics, process, cleanroom — ratio 1 to 5 or more), **HVAC / utilities** (often 15–30% of the building in pharma / batteries), lines and equipment (OEMs), automation / MES / IT, tooling, **qualification** (hours, consumables, product), ramp-up (losses), connections, land; benchmarks by product and capacity, not per m².

### Cost controller
- Two budgets to reconcile: **building** (physical progress, works valuations) and **process** (OEM milestones: order, FAT, delivery, SAT, qualification); OEM currencies; **cost of layout changes**; conditional grants (milestones, eligibility); distinguish CAPEX from start-up costs (ramp-up, training, qualification product).

### Planner
- Two parallel critical paths: **building → utilities → cleanrooms → HVAC qualification** and **URS → OEM order → FAT → delivery → SAT → IQ / OQ / PQ → ramp-up → SOP**; the two meet at the hand-over of the zones; long-lead: lines (12–24 months), HVAC, transformers; **qualification** is a phase with its own resources (quality, operators).

### Contract manager
- Building packages (works contracts, design firm, inspection body, statutory warranties — ten-year liability where it exists) vs **OEM contracts** (rate / OEE / yield guarantees, FAT / SAT, LDs, parts, CE and qualification documentation, intellectual property on tooling); **contractual interfaces** between the packages (who supplies, installs, connects, tests); obligations towards the insurer and the customer (approval).

### Risk manager
- Dominant: **OEM long-lead and solvency**, **qualification and approval** (inspection, customer), **HVAC / cleanrooms**, unstable layout, **ramp-up** (yield, rate), recruitment, electrical connection, permits (classified installations, land take), fire (insurer), cyber / OT, product change during the project.

### Financing & FID
- On balance sheet or with grants (national investment programmes, regions, IPCEI, IRA / CHIPS): conditions (jobs, milestones, local content) to be integrated into the schedule; business case sensitive to ramp-up yield and the SOP date; sale-and-leaseback of the building sometimes.

### Project insurance
- The **property insurer** (FM Global HPR-type) acts as a quasi-contractual prescriber (identity card): fire analysis, sprinklers, compartmentation, lithium storage. Red flag (sector): insurer's requirements discovered after the permit.

### Process engineer
- Becomes **lines and flows engineer**: mapping of the manufacturing process, capacity per station, bottlenecks, **flows** (product, personnel, materials, waste, cross-contamination in pharma / food), URS per equipment item, required utilities, intermediate storages, **hygienic design** (food, EHEDG), special processes (surface treatment, painting, welding — NADCAP in aerospace).

### Mechanical engineer
- Machines and robots (OEM), conveying, handling, tooling; **machine safety** (ISO 12100 risk analysis, ISO 13849 categories / PL, CE marking of the integrated assembly — who is the "manufacturer" of the assembled line?); pressure equipment (autoclaves, compressors); vibrations and installation.

### Materials & corrosion engineer
- **Electropolished 316L** and ASME BPE in pharma, hygienic design in food, solvent and electrolyte compatibility (batteries), floor coatings (resin, ESD conductivity), corrosion in production atmospheres (salt, vapours); killer pair: **non-hygienic material + aggressive cleaning** = contamination and corrosion.

### Piping engineer
- **Utilities**: compressed air, vacuum, gases, chilled water, steam, **clean utilities** (WFI, PW, clean steam — orbital welding, slope, loops, ASME BPE), solvent networks (hazardous areas), extraction; process piping limited to the OEMs.

### Civil / structural engineer
- **Industrial slab** (flatness, rolling loads, resin, machine anchors), steelwork and cladding, mezzanines, **fire compartmentation** (insurer), plant rooms, foundations of vibration-sensitive machines, extension of an existing building (party walls, phasing).

### Geotechnical engineer
- Standard, except slabs with heavy loads and vibration-sensitive machines; brownfields (contamination, existing foundations).

### Electrical engineer
- **Load list** (machines + HVAC + utilities — often underestimated by 20–30%), MV / HV connection, distribution, power quality (drives, harmonics), **secured supplies** (cleanrooms, IT, continuous processes), lighting, ESD, hazardous areas (solvents, batteries).

### Instrumentation engineer
- Ambient monitoring (EMS: particles, pressures, temperature, humidity), clean-utility instrumentation, **traceability and data integrity** (qualified sensors, calibration), machine safety (safety sensors).

### DCS / control systems engineer
- Becomes **automation / MES / SCADA**: PLCs (IEC 61131), supervision, **MES** (production orders, traceability, product genealogy), ERP interfaces, **GAMP 5 / 21 CFR Part 11** (computerised system validation, audit trail), OT cybersecurity (IEC 62443), standardisation between lines.

### HSE
- Hazards that kill: **machines** (crushing, entanglement — lock-out, guards), **forklifts and logistics flows** (pedestrian collisions), **hazardous areas** (solvents, food dust, electrolytes), chemicals (CMR), fire (lithium batteries: thermal runaway), work at height on site, site / production co-activity in extensions; workstation ergonomics from design.

### Technical safety
- Scope: **fire** (insurer's analysis, sprinklers, compartmentation, lithium storage), major hazards where applicable (solvents, electrolytes), hazardous areas, integrated **machine safety**; little classic QRA.

### Environment & permitting
- Building permit and **land take**, classified installations by activity (often registration / notification, full authorisation for large sites and major-hazard sites), water and discharges (food: loaded effluents), noise, traffic, **workplace regulations** (premises), insurer's dossier; in pharma: establishment licence (opening authorisation); opposition sticking point: traffic, land take, odours (food).

### Procurement
- **Line OEMs** (12–24 months, market concentrated by technology), HVAC / cleanrooms, transformers, automation; **URS before consultation**, contractual FAT with criteria, spare parts and obsolescence; building packages as works contracts; operating purchases (consumables, materials) to be prepared for the qualification.

### Construction manager
- Two nested sites: **building** then **line installation** (access, doors, finished slabs, cleanliness, utilities available); **delivery and lifting schedule** of the machines; protection of clean zones (access protocols, cleaning); extension in a living site: co-activity with production.

### Quality (QA/QC)
- **Product and process** quality as much as construction: building / utilities ITP (clean-utility welds, HVAC tests), **FAT / SAT** with criteria, **qualification** (IQ / OQ / PQ, protocols and reports), computerised system validation (GAMP 5), **FAI / PPAP** (aerospace / automotive), documentary traceability for the regulatory inspection.

### Commissioning
- Becomes **SAT + qualification**: utilities start-up → HVAC / cleanroom qualification → line SAT → **IQ / OQ / PQ** or capacity tests (run-off) → pilot production / validation batches → **inspection or approval** → SOP → **ramp-up**. The milestone that counts is the **release of the first commercial batch** (pharma) or the **customer validation** (automotive / aerospace), not the end of installation.

### O&M (operations & maintenance)
- **TPM**, OEE, preventive maintenance of the lines (OEM plans), critical parts, CMMS, automation obsolescence, **periodic requalification** (HVAC, clean utilities, machines), change control (GMP), training; design for maintainability (access, modularity, component standardisation).

### Grid & utility connection
- Becomes **utilities and energy**: electrical connection (often the long pole — MV / HV, DSO / TSO), gas, water and sewage (capacity of the local wastewater plant — food), heat / cold, telecoms; power to be reserved early, with the growth of the next phases.

### Interface manager
- **Building ↔ process ↔ utilities ↔ automation ↔ quality**: the interface matrix (who supplies, installs, connects, tests, qualifies) is the central document; interfaces with existing production (extensions) and with the customer / the inspector (qualification requirements).

### Document control
- **Qualification** dossier (URS, DQ, IQ, OQ, PQ, protocols, reports) and **CE** documentation of the machines: regulatory and inspection documents; building hand-over dossier; data integrity of electronic records (21 CFR Part 11); as-built drawings of the utilities.

### Site & stakeholder engagement
- **Land and permits** are an FID lock (identity card): land take and zoning, with the local authority and the developer of the industrial estate as counterparts.

### Supply & offtake
— nothing specific —

## Country × sector notes (to be checked locally)

- **France**: building permit / land take (ZAN), ICPE 2xxx / 4xxx, labour code (INRS workplace design guides), ANSM (pharma), DDPP (food), France 2030 grants; **Germany**: BImSchG, Betriebssicherheitsverordnung, TÜV, Bebauungsplan; **Belgium / Poland / Spain**: regional permits, machinery / Seveso transposition, national medicines agencies (FAMHP, URPL, AEMPS).
- **EU**: Machinery Regulation 2023/1230 (2027), EU GMP, REACH, IED for large sites.
- **United States**: OSHA machine guarding and lock-out (29 CFR 1910), NFPA 13 / 855, FDA 21 CFR 210/211 and Part 11, IRA / CHIPS incentives, state and county permitting.
- **Asia (Korea, Japan, China, Southeast Asia)**: large battery and electronics plants under national industrial policies; local machine-safety and fire codes; Korean KOSHA and Japanese Industrial Safety and Health Act for machines.

## Cross-cutting red flags of the sector

- **Layout not frozen before the lines are ordered**.
- **URS written after the OEM offers**; rate guaranteed without a definition of stoppages.
- **Qualification and ramp-up absent from the schedule and the business case**.
- **HVAC / cleanrooms handled as an ordinary building package**.
- **Load list underestimated**; late electrical connection.
- **CE marking of the assembled line without an identified manufacturer**.
- **Insurer's requirements discovered after the permit**.
