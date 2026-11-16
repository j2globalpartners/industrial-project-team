# Sector profile — Hydrogen (electrolysis, compression, storage, distribution)

> **Example profile — unreviewed.** Written as an illustration of the expected density of a sector profile, from general industry knowledge, not from field practice validated by the author. Figures are indicative; regulatory references are given by family with examples, to be replaced by the project country's set (`countries/standards-regimes.md`). To use it: copy into `references/sectors/hydrogen.md`, then review every line with a practitioner.

## Sector identity card

- **Object**: hydrogen production by **water electrolysis** (alkaline, PEM; SOEC emerging) fed with renewable or low-carbon electricity, with **purification, compression, storage** and delivery (pipeline, tube trailers, refuelling station) to an industrial use (refining, ammonia, methanol, steel, glass) or mobility. Variants: direct coupling to a renewable park, e-fuels, injection into the gas network.
- **Typical scale**: 1 to 20 MW (pilots, mobility), 20 to 100+ MW (industrial), several hundred MW in valley / hub projects. CAPEX of the order of **1.5 to 3 M€/MW installed all-in** (order of magnitude, falling fast and widely dispersed: the electrolyser weighs ~40–60%, the rest is balance of plant, electrical, compression / storage, civil). Development 2 to 4 years, construction 12 to 24 months. Team: PM, process / integration, electrical (heavy), HSE / safety, contract manager, grid connection, financing — the sector is young, **the classic EPC role sheets apply in full**.
- **Dominant contract models**: **electrolyser supply by an OEM** (with efficiency, degradation and availability guarantees) + **EPC / EPCM** for the balance of plant, or integrated EPC; **electricity PPA** compliant with the renewable-hydrogen framework; **H₂ offtake contract** (take-or-pay, purity and pressure specifications); electrical connection agreement; sometimes a service contract / LTSA on the stacks.
- **Life cycle & gates**: `PRE-FEASIBILITY (offtake, electricity, site) → FEASIBILITY (OEM technology, permits, grid connection) → FEED → FID (grant notified, PPA, offtake, permits) → EXECUTION → COMMISSIONING (inerting, first kg, purity) → PERFORMANCE TEST → OPERATION`. AACE classes 5 → 3 at FEED → 2 at FID; **the FID depends at least as much on the contracts (PPA, offtake, grant) as on the engineering**.
- **Regulatory framework and permits** (by family; the country decides the set): industrial hydrogen production is a **classified / permitted installation** everywhere; **major-hazard regime** above hydrogen inventory thresholds (Seveso III: lower tier of the order of 5 t, upper tier 50 t, to be checked; COMAH / PSM / MHF equivalents elsewhere); hazard study and land-use planning constraints; **pressure equipment** (PED / ASME); **hazardous areas** (ATEX / IEC 60079 or NEC); building permit; transport of dangerous goods (ADR / TPED, DOT); **renewable-hydrogen qualification** (EU RED II / III delegated acts on RFNBO: additionality, temporal then hourly correlation, geographic correlation; US 45V rules; similar schemes elsewhere) and certification (ISCC EU, CertifHy); standards ISO 22734 (electrolysers), ISO/TR 15916 (H₂ safety), ISO 19880 (stations), NFPA 2, EIGA guides. Country cards: `countries/`.
- **Key external counterparts**: TSO / DSO (heavy electrical connection), electrolyser OEM, **offtaker** (industrial, mobility), electricity supplier / renewable producer (PPA), environmental and industrial-safety authority (major hazards), renewable-hydrogen certifier, financiers and grant windows (EU IPCEI, European Hydrogen Bank, national support mechanisms, US IRA credits), hydrogen or gas network operator (H₂ backbones under development).
- **FID locks / long poles**: **compliant electricity PPA** (the electricity price makes or breaks the LCOH), **firm H₂ offtake** (volumes, duration, take-or-pay), **electrical connection** (power of the order of 1.1 to 1.2 × the electrolyser power, often at HV → TSO lead times), **major-hazard permit / hazard study**, **grant notified with its conditions** (dates, local content, additionality), **OEM maturity and solvency**.
- **Economics & revenue**: **LCOH in €/kg** — dominated by electricity (typically 60–75% of the cost over the life) and the **load factor**; system efficiency ~50–55 kWh/kg (order of magnitude, LHV 33.3 kWh/kg); stack degradation and **stack replacement** (~60,000–90,000 h, to be provisioned); CfD-like or capex subsidy; revenue = indexed offtake contract; sensitivities: electricity price, operating hours, efficiency, availability, compression / storage / logistics cost, non-delivery penalties.
- **Roles to activate in addition**: **Electrolysis & H₂ integration engineer** (below). Roles to reinforce: **electrical** (rectifiers, transformers, power quality), **technical safety** (major hazards, H₂ jets), **materials** (embrittlement). Lightened roles: **civil / geotechnical** (skid installation and light buildings, except storage and blast walls).
- **Phase skills and references available**: no dedicated phase skill; the cross-cutting skills (claims / EOT, cost control, contractual letters and minutes, engineering register, specifications, multi-package reconciliation, portfolio cockpit, gate war-game) apply as they are.
- **Common units & ratios** (indicative): **MW** electrolyser (DC / AC — specify), **kg/h**, **t/yr**, **Nm³/h** (~1 kg ≈ 11.1 Nm³); **kWh/kg** (stack ~47–52, system ~50–58); demineralised water ~10–20 L/kg H₂ (stoichiometry 9 L); O₂ co-product ~8 kg/kg H₂; outlet pressure 1–30 bar (alkaline / PEM), compression 200–500 bar (mobility 350 / 700 bar); purity ISO 14687 (PEM mobility: 99.97% and impurities in ppm); **LCOH** €/kg; load factor in h/yr.
- **Key vocabulary**: stack, cell, membrane (PEM), diaphragm (alkaline), KOH, rectifier (thyristor / IGBT), transformer-rectifier, balance of plant (BoP), deoxo, dryer (PSA / TSA), purge, N₂ inerting, diaphragm / dry-piston / ionic compressor, tube trailer, cylinder bundle, buffer storage, station (dispenser), H₂ pre-cooling, RFNBO, additionality, temporal correlation, PPA, take-or-pay, LCOH, major-hazard tier, hazardous area, pressure equipment, hydrogen embrittlement (HE), leak, jet fire, invisible flame, PRD (pressure relief device), vent, F&G.

## Sector-specific roles

### Electrolysis & H₂ integration engineer
- **Mission**: accountable for the **integrated performance** (kWh/kg, kg/h, purity, degradation) between the OEM (which guarantees its stack) and the BoP (which guarantees everything else) — the person who prevents the guarantee from falling "between two contracts".
- **Reading grid of an OEM offer**: (1) exact scope of supply (stack only? rectifier? deoxo / dryer? water? cooling? control?); (2) basis of the performances (BOL vs EOL, DC vs AC, temperature and pressure conditions, load range); (3) degradation curve and definition of stack end of life; (4) dynamic operating range (minimum load, ramps, stops / starts, H₂ / O₂ cross-over at low load); (5) required water quality and discharges; (6) guarantees and performance test (method, tolerance, duration); (7) references in operation at the same scale.
- **Anchors (indicative)**: system efficiency 50–58 kWh/kg; minimum load ~10–20% (PEM) / 20–40% (alkaline); degradation ~1–2%/yr of voltage; stack life 60,000–90,000 h; cooling ~30–40% of the electrical energy dissipated as heat; water ~10–20 L/kg.
- **Red flags**: performance guaranteed in DC at stack level while the offtake contract reads in AC at the meter; OEM without a reference at scale; performance test not defined; no provision for stack replacement; dynamic range incompatible with the PPA profile.
- **Senior eye**: "the guarantee is where the figure is measured" — they have the meter and the analyser installed where the guarantee is expressed, and they know the electrolyser is the most visible but rarely the riskiest part of the schedule (the grid connection and the compressors are).

## Role inserts

### Project manager
- The FID is an **assembly of contracts**: PPA, offtake, grant, OEM, EPC, grid connection — the PM holds the **consistency of dates and scopes** between them (a take-or-pay starting before commissioning = penalties on day one).
- Long poles: electrical connection (HV), compressors and transformer-rectifiers, major-hazard permit, **grant conditions** (dates, disbursement milestones).
- Young technology: manage the **OEM uncertainty** (lead times, performances, solvency) as a first-rank risk, with contractual plan Bs.

### Estimator
- Break down: electrolyser (stack + OEM BoP), **upstream electrical** (transformers, rectifiers, HV / MV — often underestimated), water treatment, cooling, **compression and storage** (can equal the electrolyser in €/MW depending on pressure and autonomy), buildings / skids / blast walls, safety (F&G, vents), grid connection and cost share, delivery logistics.
- Anchor: electrolyser prices falling fast and very dispersed by technology and OEM — date and source every benchmark, distinguish "stack" cost from "installed system" cost.
- OPEX is the real subject: electricity, stack replacement, water, compressor maintenance.

### Cost controller
- Heavy and early OEM payment milestones (down payment, FAT, delivery); currency and raw-material indexation (iridium, platinum, nickel); **stack replacement provision** from the budget; grants = conditional revenue (milestones, eligible expenses, local content) — keep the eligibility accounting alongside the EAC.

### Planner
- Long-lead: **transformer-rectifiers and compressors (12–24 months)**, electrolyser (12–24 months), HV connection (often > 24 months). Commissioning includes **inerting**, leak tests, purity ramp-up and dynamic tests with the network — several weeks to months.
- External milestones: PPA and offtake start dates, grant deadlines, renewable-hydrogen qualification.

### Contract manager
- **OEM guarantees** (efficiency at BOL / EOL, degradation, availability, purity, dynamic range) vs **EPC / BoP guarantees**: hunt the gaps (who guarantees the kWh/kg at the meter?); single contractual performance test; performance and delay LDs; stack replacement warranty.
- **Take-or-pay offtake** and **as-produced / baseload PPA**: align volumes, dates, force majeure, indexation, renewable-hydrogen compliance (who carries the non-certification risk?).
- Young technology: OEM solvency clauses, documentation escrow, spare parts, assignment of warranties.

### Risk manager
- Dominant risks: **price and availability of compliant electricity**, **offtake default**, **grid connection delay**, **OEM performance / degradation**, **H₂ safety** (leak, jet fire, confined explosion), regulatory evolution (renewable-hydrogen rules, major-hazard thresholds), **grant** (non-award, clawback), stack supply chain.

### Financing & FID
- Bankability conditioned by: compliant long-term PPA, take-or-pay offtake with a solid counterparty, assignable OEM guarantees, notified grant; DSCR sensitive to **electricity price and load factor**; stack replacement reserve; CPs at drawdown: permits, renewable-hydrogen certification, grid connection, EPC / OEM signed.

### Project insurance
— nothing specific —

### Process engineer
- Mass / energy balance from the electrolyser to the delivery point: **purification** (deoxo, drying → ISO 14687 purity), **O₂ management** (safe vent, possible recovery), **water** (demineralisation, conductivity, regeneration discharges), **heat** (cooling, recovery), **compression and buffer storage** (autonomy, cycles), N₂ vents and purges, emergency shutdown and depressurisation philosophy.
- Red flag: H₂ / O₂ cross-over at low load ignored in the control philosophy (low-load limit = safety, not only efficiency).

### Mechanical engineer
- **Compressors** (diaphragm, dry piston, ionic): long-lead, bad actors, N+1 redundancy, pulsations; storage (cylinders, tubes, low-pressure spheres); exchangers and air coolers; **pressure equipment** in the highest categories frequently.
- Codes: ASME VIII / EN 13445, API 618 / 619, ISO 19880, EIGA; H₂-compatible materials (materials link).

### Materials & corrosion engineer
- **Hydrogen embrittlement**: ban high-strength steels, control weld hardness (NACE / ISO-type limits), prefer 316L of verified grade, avoid certain martensitic / hardened grades; H₂-compatible elastomers at high pressure (explosive decompression); copper / brass limited; hot KOH (alkaline): nickel, suitable steels.
- The sector's killer pair: **steel too strong + high-pressure H₂ + hard weld** = delayed cracking.

### Piping engineer
- **ASME B31.12** (H₂), H₂ piping classes, 100% inspected welds, welded rather than threaded fittings, high-integrity flanges and gaskets, helium or H₂ leak tests; **vents** sized (velocity, height, distance, absence of ignition), expansion on hot stack outlet lines; cleaning and degreasing of O₂ lines.

### Civil / structural engineer
- Skids and light buildings, slabs for electrolysers and compressors (vibrations), **fire / blast walls**, storage and tube-trailer loading areas, KOH bunds, purge drainage, layout distances from the hazard study.

### Geotechnical engineer
- Standard, except compressor foundations (dynamics) and storage foundations; nothing specific to the sector.

### Electrical engineer
- **Second core of the trade.** MV / HV connection, transformers and **rectifiers** (thyristors vs IGBT: harmonics, power factor, filters), power quality and **grid code** (flicker, harmonics, reactive), auxiliary distribution, electrical hazardous areas, earthing and static electricity protection; load list including compressors, cooling and water treatment (often 10–20% above the electrolyser).
- Red flag: requested connection power = stack power (auxiliaries and rectifier efficiency forgotten).

### Instrumentation engineer
- **H₂ detection** (sensors, high-point positioning, coverage rate), purity analysers (O₂, H₂O, N₂) and O₂-in-H₂ / H₂-in-O₂ (stack safety), flow measurements (Coriolis, thermal) at the guarantee point, high-integrity pressure / temperature, pressure SIFs, KOH level, cross-over.

### DCS / control systems engineer
- OEM control (stack) vs site system: **integration**, emergency shutdown and depressurisation sequences, **PPA profile tracking** (ramps, minimum load, stops / restarts), network interface (PPC), dedicated SIS, cybersecurity (OEM remote access).

### HSE
- Hazards that kill: **H₂** (flammability range 4–75%, ignition energy ~0.02 mJ, **invisible flame**, high-pressure jets, accumulation at high and confined points), **O₂** (enrichment, fire), **KOH** (chemical burns), DC high voltage, nitrogen (asphyxia), pressure equipment.
- Reflexes: detection and ventilation of high points, no confinement without venting, strict hot-work permits, UV-IR flame cameras / detectors, H₂ training for everyone on site.

### Technical safety
- **Major-hazard study**: leaks from pipes and storages (jet fires, explosion in confined or congested areas, dispersion), effect distances, **layout and blast walls**, H₂ F&G (suitable gas and flame detectors), PRDs and vents, SIL of the SIFs (pressure, cross-over, detection), inherent safety (limit the pressurised inventory).
- The sector's "dumb" catastrophic failure: **H₂ cross-over into O₂ at low load** (explosive atmosphere in the O₂ circuit) and **a badly positioned vent** ignited by an ignored source.

### Environment & permitting
- **Classified-installation and major-hazard regime** — tier and distances drive the layout; hazard study, public inquiry under full authorisation, land-use planning constraints at the upper tier; water abstraction and discharge (water permits), compressor noise; **renewable-hydrogen certification** and grant dossiers (environmental conditions); acceptability: **explosion risk** and the "major-hazard" image are the sticking point, more than nuisances.

### Procurement
- Long-lead: **transformer-rectifiers (12–18 months)**, **compressors (12–24 months)**, electrolyser (12–24 months), analysers, high-pressure H₂ valves; concentrated and consolidating OEM market → **solvency and reference due diligence**, bank guarantees, critical parts; critical materials (PEM iridium, nickel); local content and grant eligibility.

### Construction manager
- **Skid** erection (little civil work, much lifting and connection), cleanliness and degreasing (O₂), systematic **pressure and leak tests**, OEM coordination on site (erection supervision), hazardous area as soon as H₂ is introduced (end of classic co-activity).

### Quality (QA/QC)
- **H₂ welds: 100% inspection** (RT / UT), hardness, PMI of grades, EN 10204 3.1 / 3.2 certificates or equivalent, pressure tests, **leak tests** (helium / H₂), O₂ cleanliness; pressure-equipment dossiers (conformity marking, notified body / authorised inspector); witnessed FAT of the electrolyser and the compressors.

### Commissioning
- Sequence: cleaning / blowing → pressure tests → **N₂ inerting** → water fill and conditioning (KOH / demineralised water) → rectifier energisation → **first H₂** → purity ramp-up (analysers) → progressive pressurisation, compressors, storage → SIF and emergency shutdown tests → dynamic tests (ramps, minimum load) → **performance test** (kWh/kg, kg/h, purity, availability) → first delivery to the offtaker.
- The milestone that counts: **first delivery on the offtaker's specs** (purity, pressure), not the first kg.

### O&M (operations & maintenance)
- Bad actors: **compressors**, KOH pumps and filters, dryers, analysers, H₂ sensors (calibration); **stack degradation** tracking (voltage at constant current); water quality; planned **stack replacement**; availability vs PPA profile; OEM critical parts; operating a major-hazard site (emergency plan, drills).

### Grid & utility connection
- **Electricity**: offtake connection power (often HV), TSO / DSO offer, agreement, power quality; **H₂**: pipeline to the offtaker or H₂ network (framework under construction), purity and pressure specs at the delivery point; **gas**: H₂ injection into the network (limited rates, framework to be checked); **water**: abstraction and discharge.

### Interface manager
- Interfaces that bite: **OEM ↔ BoP** (supply limits, guarantees, control), site ↔ offtaker (specs, meter, logistics), site ↔ renewable producer / PPA (profile, remote control), site ↔ network operator (connection, grid code), renewable-hydrogen certification (data to be produced).

### Document control
- **Pressure-equipment dossiers** (conformity, calculation notes, test minutes), major-hazard dossier / hazard study, OEM documentation under escrow, **renewable-hydrogen traceability** (hourly electricity / production data) — dossiers that condition commissioning and acceptance.

### Site & stakeholder engagement
— nothing specific —

### Supply & offtake
- Both ends are FID locks (identity card): a **compliant electricity PPA** — the electricity price makes or breaks the LCOH — and a **firm H₂ offtake** (volumes, duration, take-or-pay, purity and pressure specifications) with a solid counterparty.

## Country × sector notes (to be checked locally)

- **France**: national hydrogen production support mechanism (tenders), national strategy, ADEME; ICPE 3420 / 4715 / 1416; H₂ network framework under construction (NaTran).
- **Germany**: very active H₂ framework (H₂ core network — Kernnetz, H2Global auctions, EEG / support), BImSchG, VDE-AR-N for the connection.
- **Spain**: H₂ strategy and valleys (PERTE), State / regional authorisations, REE connection.
- **Belgium / Poland**: frameworks being structured (Fluxys H₂ backbone, industrial projects) — to be checked project by project.
- **EU**: RED III / RFNBO delegated acts, European Hydrogen Bank, IPCEI, taxonomy.
- **United States**: 45V production tax credit (IRA) with its hourly-matching and additionality rules, DOE hydrogen hubs, NFPA 2 and NEC Article 500 hazardous areas, OSHA PSM above the threshold.
- **Gulf / Australia / Chile**: export-oriented green hydrogen and ammonia projects (very large renewable parks, port logistics); offtake and certification for export markets are the locks.

## Cross-cutting red flags of the sector

- **PPA not compliant with the renewable-hydrogen rules** or whose profile does not match the electrolyser's dynamic range.
- **Offtake not firm** or take-or-pay starting before demonstrated commissioning.
- **Performance guarantee falling between the OEM and the BoP**.
- **Connection power underestimated** (auxiliaries, rectifier efficiency).
- **Stack replacement not provisioned**.
- **Grant taken for granted** before notification and without meeting its conditions.
- **H₂ safety handled like natural-gas safety** (invisible flame, high points, jets).
