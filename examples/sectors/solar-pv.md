# Sector profile — Solar photovoltaics (ground-mounted, carports, agrivoltaics, rooftops)

> **Example profile — unreviewed.** Written as an illustration of the expected density of a sector profile, from general industry knowledge, not from field practice validated by the author. Figures are indicative; regulatory references are given by family with examples, to be replaced by the project country's set (`countries/standards-regimes.md`). To use it: copy into `references/sectors/solar-pv.md`, then review every line with a practitioner.

## Sector identity card

- **Object**: grid-connected photovoltaic plant — ground-mounted (fixed or trackers), car-park canopies, agrivoltaics, large industrial rooftops; sometimes coupled with battery storage (BESS). The "process" is trivial; **the project is a land, permit, grid-connection and logistics project**, more than an engineering project.
- **Typical scale**: 5 to 100+ MWp ground-mounted, 1 to 20 MWp canopies / rooftops. EPC CAPEX of the order of **0.6 to 1.0 M€/MWp ground-mounted excluding grid connection** (order of magnitude, very sensitive to module prices and terrain); grid connection and network cost share on top. Development 2 to 5 years (land, permits, grid connection, tender) for **6 to 12 months of construction**. Very lean team: project manager, PV / electrical engineer, site manager, land / permitting developer.
- **Dominant contract models**: **turnkey EPC** (most common) with PR and availability guarantees, or **multi-package** (structures, modules, inverters, electrical BOS, civil / roads, delivery substation, grid connection) when the Owner internalises engineering; long-term **O&M** contract; **long lease** or lease promise 30–40 years; **PPA** or contract-for-difference / feed-in premium (tender) that carries the revenue.
- **Life cycle & gates**: `LAND PROSPECTING → FEASIBILITY (solar resource, grid connection, planning) → DEVELOPMENT (permits, connection offer, consultation) → TENDER / PPA → FID → CONSTRUCTION → ENERGISATION (certification, grid commissioning) → PROVISIONAL ACCEPTANCE → PR TEST → OPERATION 25–35 years`. Estimate classes: 5 at prospecting, 4 at feasibility, 3 at permit filing, 2 at tender / FID.
- **Regulatory framework and permits** (by family; the country decides the set): **building / planning permit** for ground-mounted plants above a power threshold, lighter declaration below; **environmental assessment** mandatory or case-by-case according to power and footprint; **land-use rules** (agricultural land protection, net-zero land take, acceleration zones, car-park canopy obligations in some countries — e.g. France's 2023 renewables acceleration law); **agrivoltaics rules** (service to the agricultural activity, maintained production, coverage ratio — e.g. France's 2024 decree); forest clearing; coastal / mountain laws; heritage, civil / military aviation opinions (glare, easements); **PV is generally not a classified installation**, but an associated BESS can be. Country cards: `countries/`.
- **Key external counterparts**: DSO / TSO (connection offer, agreement, regional capacity schemes), planning and environmental authorities, energy regulator (tenders), landowners and farmers, municipality and neighbours, chamber of agriculture, heritage body, financiers.
- **FID locks / long poles**: **secured land** (signed lease promises, easements), **permit free of appeal** (the appeal is the norm, not the exception), **grid connection** (offer accepted, capacity available at the substation, DSO / TSO lead time of 1 to 4 years depending on network works), **secured revenue** (tender award or signed PPA). The commissioning deadline imposed after award (of the order of 2 to 3 years) turns every delay into a penalty.
- **Economics & revenue**: feed-in premium / contract-for-difference over ~20 years (tender, price criterion plus in some countries a simplified carbon footprint of the modules) or corporate / utility **PPA**; revenue = **P50 yield × price**, debt sized on the **P90**. Sensitivities: irradiation, **PR**, annual degradation (~0.4–0.6%/yr), availability, **curtailment**, captured price and cannibalisation at solar hours, connection cost.
- **Roles to activate in addition**: **PV / yield engineer** (below). Generic roles without object or lightened: **process** (no process — replaced by yield), **piping** (none, except BESS / cooling), **materials & corrosion** (reduced to structure galvanisation and soil aggressiveness); **DCS → SCADA / PPC** (power plant controller); **instrumentation → monitoring** (pyranometers, weather sensors, metering).
- **Phase skills and references available**: no dedicated phase skill; the cross-cutting skills (claims / EOT, cost control, contractual letters and minutes, portfolio cockpit, gate war-game, steering challenger) apply as they are.
- **Common units & ratios** (indicative): **MWp** (DC) / **MWac** (inverters) with DC/AC ratio ~1.1–1.3; **kWh/kWp/yr** (~1,000 in northern France, ~1,400+ in southern Europe, more with trackers, 1,800+ in high-irradiation deserts); **PR** ~0.78–0.85; **P50 / P90**; footprint ~1–1.5 ha/MWp ground-mounted; **€/Wp**; **LCOE** in €/MWh; module carbon footprint in kg CO₂/kWp where tenders score it.
- **Key vocabulary**: module, string, central / string inverter, single-axis tracker, backtracking, stow, fixed structure, driven / screw pile, transformer station, delivery substation, connection offer, regional connection scheme, cost share, grid access contract, electrical conformity certificate, PR (performance ratio), P50 / P90, yield, degradation, PID (potential induced degradation), LID, curtailment, PPC, grid code, PPA, feed-in premium, tender, agrivoltaics, long lease, carbon footprint.

## Sector-specific roles

### PV / yield & performance engineer
- **Mission**: accountable for the **yield** (P50 / P90) and its demonstration — from the resource study to the PR guarantee. Replaces the process engineer.
- **Reading grid of a yield study (PVsyst or equivalent)**: (1) source and period of the irradiation data (satellite vs station, years covered, uncertainty); (2) actual layout assumptions (near and far shading, pitch, inter-row shading, albedo if bifacial); (3) loss chain line by line (soiling, temperature, mismatch, DC cabling, inverter, transformer, availability, degradation) — a "forgotten" loss inflates the P50; (4) P90 and combined uncertainty; (5) grid curtailment and injection limitation; (6) consistency with the DC/AC ratio and the inverter sizing.
- **Anchors (indicative)**: total losses ~15–22% between plane-of-array irradiation and injection; temperature ~−0.3 to −0.4%/°C on power; soiling 1–3% (more in dusty agricultural or desert areas); bifacial + tracker: 10–25% gain vs fixed depending on albedo and latitude.
- **Red flags**: P50 calculated on a single year of data; far shading ignored; PR guaranteed by the EPC above the simulated PR; module degradation outside the manufacturer's datasheet; yield not recalibrated on contractual curtailment.
- **Senior eye**: "the P50 is a negotiation, the P90 is a reality" — the senior reads the uncertainty first, not the central value; and knows that 2% of PR over 30 years is worth more than a discount on the modules.

## Role inserts

### Project manager
- The project is won **before** construction: land, permit, grid connection, tender. Construction is fast and industrialised — vigilance moves to **logistics** (module deliveries, cranes, weather) and to the **cut-off dates** (commissioning deadline imposed by the tender / PPA).
- A PV PM often carries several sites in parallel: portfolio discipline (a cockpit with land / permit / connection / revenue locks) prevails over site discipline.
- Red flags: permit appeal not provisioned in time; connection offer accepted on capacity "to be created" without an operator date; module price fixed too early or too late (volatility, customs duties); tender award without a dated commissioning plan.

### Estimator
- Price in **€/Wp** and by package: modules (~30–40% of EPC CAPEX — the most volatile item), structures / trackers, inverters, electrical BOS (DC / AC cables, combiner boxes, transformers), civil / roads / piles, delivery substation, fencing / security, monitoring; **grid connection and network cost share separately** (priced by the operator, potentially decisive).
- Site factors that make it vary: slope and geotechnics (piles vs concrete beams), distance to the substation, access and bearing capacity of tracks, clearing, environmental compensation, agrivoltaics (structure height, spacing).
- €/Wp benchmarks dated and sourced: a six-month-old module price is wrong.

### Cost controller
- Few lines but heavy and exposed ones: **modules** (currency, incoterm, duties, price-fixing date), **grid connection** (operator invoicing outside project control), **network cost share**, **environmental compensation**, **land rents and indemnities** (from development, before any revenue).
- Steering in **€/Wp EAC**; changes count in layout modifications (MWp lost at the permit) as much as in cost overruns.
- Development costs (studies, permits, land) to be capitalised cleanly — they condition the project's value in case of sale.

### Planner
- Critical path = **permit (+ appeal) → grid connection → tender award / PPA → construction**. Construction (piles → structures → modules → cabling → inverters → substations → tests) is planned in weeks, with the **grid connection availability date** as the dominant external milestone.
- Cut-off milestones: permit filing, connection offer (acceptance within a deadline), tender award, imposed commissioning date, electrical conformity certificate, grid energisation, PR test.
- Weather (rain on piles and tracks, wind on module installation) and availability of cranes / installation crews: the real site uncertainties.

### Contract manager
- EPC with **PR guarantees** (contractual test method: IEC 61724, duration, weather corrections), **availability**, **installed power**, **time** (LD) — check that the PR guarantee is testable with the sensors actually installed.
- **Three non-EPC contracts carry the project**: lease (duration, reinstatement, decommissioning, easements), connection agreement (lead times, penalties, lapse), PPA / feed-in premium (cut-off dates, delay penalties, reporting obligations).
- Module suppliers: product vs performance warranties (25–30 years linear), manufacturer solvency and bankability, **forced-labour due diligence** compliance and carbon footprint.

### Risk manager
- Register dominated by **external** risks: third-party appeals, permit lapse, DSO / TSO delay, network capacity, module price and availability, customs duties, curtailment, theft of cables and modules, **hail and storm** (tracker stow, insurance), BESS fire.
- Development risks (unsecured land, unfavourable agricultural-land opinion, biodiversity) kill the project; construction risks (weather, piles failing tests) delay it.

### Financing & FID
- Classic **project finance** on PPA / feed-in premium: debt sized at **P90** (sometimes P75), DSCR ~1.20–1.35 depending on revenue quality (order of magnitude), tenor aligned with the revenue contract; CPs at drawdown: permit free of appeal, connection agreement, PPA / award, EPC signed, insurance, lease.
- Sensitivities: yield, PR, captured price (merchant PPA), curtailment, connection cost, degradation.

### Project insurance
- Insurance in place is a CP at drawdown; dominant natural perils in the register: **hail and storm** (tracker stow strategy), plus theft of cables and modules. Red flag (sector): hail / storm without a stow strategy or suitable insurance.

### Process engineer
- Not applicable: replaced by the **PV / yield engineer** (above). On a site with BESS, the "process" reduces to energy / power sizing and the cycling strategy.

### Mechanical engineer
- Structures and **trackers**: wind loads (structural code and national annex, panel-specific coefficients), stow angle, tracker motorisation and power supply, fatigue, corrosion; clamp / module frame compatibility.
- No rotating equipment in the classic sense; "mechanical" is light steelwork and fixings — the stake is **repeatability** (thousands of identical fixings: a torque error multiplies).

### Materials & corrosion engineer
- **Galvanisation** of structures and piles (thickness vs soil aggressiveness: resistivity, pH, chlorides — geotechnical measurements), aluminium frames, bimetallic contacts; DC cables exposed to UV and rodents.
- The sector's killer pair: **aggressive soil + undersized galvanised pile** = section loss before 30 years.

### Piping engineer
- Not applicable, except liquid cooling of BESS or central inverters.

### Civil / structural engineer
- **Piles** (driven, screwed, drilled-and-grouted) or concrete beams depending on geotechnics; **pull-out and lateral load tests** at the start of the site to calibrate depth; tracks and crane pads; substations on precast bases; cable trenches; fencing; stormwater and erosion management on slopes.
- Red flag: "catalogue" pile sizing without on-site tests → refusal, lengthening, extra cost.

### Geotechnical engineer
- Light but decisive campaign: boreholes and **pull-out tests** per homogeneous zone, soil aggressiveness (pile corrosion), water level, rock or fill (brownfields, former quarries: contamination and heterogeneity).
- On brownfields: contamination diagnosis and use compatibility (sites "easy" at the permit are often difficult in the ground).

### Electrical engineer
- **The core trade here.** String sizing (cold voltage vs inverter Umax, hot current), combiner boxes, DC protections (fuses, surge arresters, disconnection), DC cables (voltage drops ~1–2%), inverters (central vs string: availability, maintainability, cost), LV / MV transformers, internal MV network, **delivery substation** and decoupling protection, **grid code** (fault ride-through, reactive power, PPC), earthing, lightning.
- References: the country's wiring rules (IEC 60364 family or NEC), IEC 62548 (PV array design), IEC 61730 / 61215 (modules), the network operator's requirements.
- Red flag: DC/AC ratio chosen without a curtailment study; decoupling protection not compliant with the grid code → energisation refused.

### Instrumentation engineer
- Reduced to **monitoring**: pyranometers (plane of array and horizontal, class A), module / ambient temperature sensors, anemometer (tracker stow), certified metering at the delivery point, string / inverter communication — this is what makes the PR guarantee **measurable**: the number and class of the sensors are contractual.

### DCS / control systems engineer
- Becomes **SCADA / PPC**: supervision, remote control imposed by the operator (active / reactive power setpoints, curtailment), OT cybersecurity (remote site, remote access), interface with the BESS. Reference: the operator's grid code, IEC 62443.

### HSE
- Hazards that kill: **DC electric arc** (a string is live as soon as it is daylight — cannot be isolated), rooftop work (falls), plant and cranes on rough terrain, heat, fire (BESS, inverters), lightning.
- High-pace site with numerous and rotating labour: induction, electrical PPE, posting-of-workers management (`countries/`).

### Technical safety
- Restricted scope: **BESS** (thermal runaway, separation, gas detection, propagation — NFPA 855 / insurers' guides), inverter and substation fire, lightning study, distances to third parties. No classic QRA outside BESS.

### Environment & permitting
- **The central trade of the development phase.** Opposition sticking point: **landscape and consumption of agricultural / natural land** (rather than odours or noise); biodiversity (protected species, derogation, compensation), clearing, wetlands, net-zero land take, agricultural-land protection, heritage, aviation.
- Sequence: screening or impact assessment → building permit → public inquiry where applicable → **lapse of appeal periods** (to be counted in the calendar, not in the margin); agrivoltaics: agricultural dossier demonstrating the service rendered.
- Senior eye: a permit obtained without local consultation is a permit under attack; the appeal costs more than the consultation.

### Procurement
- **Modules**: global market, weekly prices, incoterms and container logistics, customs duties and anti-dumping measures, **forced-labour due diligence** and polysilicon traceability, carbon footprint where tenders score it, manufacturer bankability, warranties and warranty insurance; price fixing = a treasury and risk decision.
- Long-lead: **transformers and delivery substation** (12–18 months, often the real long pole), inverters, trackers; structures and piles: galvanising capacity.
- Supply-chain security: on-site storage (theft, damage), delivery windows aligned with installation.

### Construction manager
- **Industrial and repetitive** site: piles → structures → modules → DC cabling → combiner boxes → inverters / substations → MV network → tests. Productivity in **modules installed per day and per crew**, pile rate per machine; weather and access dominate.
- Sticking points: pile acceptance (tests), delivery management (containers, cranes, storage), DC connector quality (mismatch and fires), theft of material.

### Quality (QA/QC)
- ITP centred on: piles (setting out, tests), tightening torques, DC connectors and polarity, **string tests** (Voc, Isc, insulation), **thermography** and **electroluminescence** by sampling at module receipt and after installation, earthing, MV substation tests; acceptance reference **IEC 62446**.
- Red flag: module batch not checked at receipt (transport micro-cracks invisible to the eye).

### Commissioning
- Sequence: string and insulation tests → inverter energisation → substation and protection tests → **electrical conformity certificate** → grid energisation (DSO / TSO) → **progressive injection** → provisional acceptance → **PR test** (IEC 61724, over the contractual period) → final acceptance.
- The milestone that counts is the **grid energisation**, not the end of works: qualification by the operator is outside the EPC's control.

### O&M (operations & maintenance)
- Almost unmanned site: remote **monitoring**, availability (~98–99% order of magnitude), PR tracking, **cleaning** (frequency depending on soiling), **vegetation** (mowing, grazing), inverter replacement at ~10–15 years (to be provisioned), tracker management, drone thermography, security (intrusion, theft), module warranties (degradation).
- O&M contract with availability guarantee and PR bonus / malus; interface with the lease (land upkeep) and with the farmer in agrivoltaics.

### Grid & utility connection
- **Electricity only**: connection application → **offer** (DSO at MV up to a power threshold, TSO at HV beyond — thresholds per country) → acceptance within a deadline → agreement → network works → energisation; **regional capacity schemes** (reserved capacity, cost share), queue, available capacity at the substation, contractual curtailment, access contract.
- Senior eye: "reserved" capacity is not "available" capacity — check the saturation state of the substation and the network works conditioning the date.

### Interface manager
- Interfaces that bite: EPC ↔ network operator (delivery point, protections, remote control), EPC ↔ O&M (transfer, monitoring data), site ↔ farmer (access, crop calendar), BESS ↔ plant, land ↔ neighbours (tracks, easements).

### Document control
- Proportionate EDMS but **impeccable connection dossier and certificates** (conformity, tests, energisation minutes): they trigger energisation and acceptance; electrical as-built and pile layout for O&M.

### Site & stakeholder engagement
- **Secured land** is an FID lock (identity card): signed lease promises (long lease of 30–40 years) and easements; counterparts are landowners and farmers, the municipality and neighbours, the chamber of agriculture, the heritage body. The third-party appeal against the permit is the norm, not the exception.

### Supply & offtake
- No feedstock; **secured revenue** is an FID lock (identity card): tender award (contract-for-difference / feed-in premium) or signed PPA.

## Country × sector notes (to be checked locally)

- **France**: CRE tenders (feed-in premium, carbon criterion), open-window tariff for small capacities, 2023 acceleration law, agrivoltaics decree (2024), S3REnR regional schemes / cost share, electrical conformity certificate (Consuel).
- **Belgium**: regionalised — green certificates (WAL) / prosumer schemes and auctions (FL), environmental permit / omgevingsvergunning; network capacity often constrained (flexible access).
- **Poland**: renewable auctions (URE), DSO / PSE connection conditions often the lock (warunki przyłączenia).
- **Spain**: access and connection permits with administrative milestones and guarantees (lapse), auctions, saturation of network nodes, State / regional authorisations.
- **Germany**: EEG (ground-mounted auctions, tariffs for small installations), municipal Bebauungsplan, VDE-AR-N 4110 / 4120 (grid code).
- **United States**: interconnection queues (ISO/RTO or utility), IEEE 1547 / 2800, NEC Article 690, ITC tax credits and domestic-content rules; permitting by county and state.
- **Gulf / India / Chile**: very high irradiation and soiling; large tender programmes (auctions) with aggressive PPA prices; grid curtailment and evacuation infrastructure often the lock.

## Cross-cutting red flags of the sector

- **Land or permit not secured** when heavy spending (modules, transformer) is committed.
- **Appeal not provisioned** in the calendar and the financing.
- **Network capacity assumed available**; connection offer accepted without a network works date.
- **Optimistic P50** (short irradiation data, forgotten losses) sizing the debt.
- **PR guarantee not measurable** with the installed instrumentation.
- **Modules not checked at receipt**; module price exposed to currency and duties without a strategy.
- **Hail / storm** without a stow strategy or suitable insurance.
