# Sector profile — Thermal power generation (CCGT, biomass, waste-to-energy, cogeneration)

> **Example profile — unreviewed.** Written as an illustration of the expected density of a sector profile, from general industry knowledge, not from field practice validated by the author. Figures are indicative; regulatory references are given by family with examples, to be replaced by the project country's set (`countries/standards-regimes.md`). To use it: copy into `references/sectors/thermal-power.md`, then review every line with a practitioner.

## Sector identity card

- **Object**: plant producing electricity (and often heat) by combustion — **combined-cycle gas turbine (CCGT)**, open-cycle gas turbine (OCGT, peaking), **biomass plant** (boiler + steam turbine), **waste-to-energy plant (WtE)**, industrial cogeneration, conversion / hybridisation of existing plants (coal → biomass, gas → H₂-ready). The core is the **power island** (gas turbine, HRSG or boiler, steam turbine, generator) delivered by one or two OEMs; everything else is balance of plant.
- **Typical scale**: CCGT 400–900 MW per unit; OCGT 50–300 MW; biomass 10–150 MW; WtE 20–100 MW (sized in **t/yr of waste**, 100,000–400,000 t/yr). CAPEX of the order of **~1 M€/MW for a CCGT** (order of magnitude, rising recently), **2.5–4 M€/MW for biomass**, more for WtE (priced in €/t of annual capacity). FEED → COD: 3 to 5 years (CCGT ~30–36 months of EPC). Complete EPC teams; driven by the power-island OEM.
- **Dominant contract models**: **turnkey EPC** with **performance guarantees** (net output, **efficiency / heat rate**, emissions, noise, availability, start-up time) and LDs; or **split** power island (OEM) + BoP (EPC / multi-package) with a **wrap** or a coordinator; **LTSA / CSA** (long-term service agreement) on the turbine; **fuel supply contract** (gas, biomass — duration, indexation, sustainability; waste — treatment contract with the municipality); **PPA / capacity market**; TSO connection agreement.
- **Life cycle & gates**: `FEASIBILITY (site, grid, fuel, permits) → FEED / EPC tender → FID (permits, grid connection, fuel, offtake) → EPC → CONSTRUCTION → COMMISSIONING (first fire, synchronisation, load tests) → RELIABILITY RUN → PERFORMANCE TEST → PAC / COD → FAC`. AACE classes 4 at feasibility, 2 at EPC award.
- **Regulatory framework and permits** (by family; the country decides the set): **combustion plant permitting** with an **integrated pollution regime** for large plants (IED ≥ 50 MW and the LCP BREF in the EU with NOₓ, SO₂, dust, CO, Hg limits; Clean Air Act NSR / Title V in the US), **waste incineration rules** (WI BREF, Industrial Emissions rules), **fuel storage** and major-hazard rules where applicable, CO₂ allowances (EU ETS and equivalents), water permits (abstraction, thermal discharge), noise, **continuous emissions monitoring** (QAL 1/2/3, EN 14181; 40 CFR 75 in the US), pressure equipment, the **TSO grid code** (HV connection, ancillary services, fault ride-through), biomass sustainability (RED II / III criteria in the EU), public inquiry. Country cards: `countries/`.
- **Key external counterparts**: **turbine / boiler OEM**, **TSO** (HV connection, grid code, capacity market), **gas TSO** (gas connection, firm capacity), environmental and industrial-safety authority, fuel suppliers (gas; biomass: wood chain; municipalities for waste), electricity / heat buyer, neighbours (plume, truck traffic for biomass / WtE), financiers.
- **FID locks / long poles**: **HV electrical connection** (TSO: 2–5 years depending on works), **firm gas connection** (station, pressure), **permits and public inquiry** (IED, air, water), **fuel contract** (biomass: sustainable resource and price; waste: contract with the municipality), **OEM long-lead** (gas turbine, generator, main transformer: 18–30 months), **offtake / market** (PPA, capacity, heat).
- **Economics & revenue**: electricity market (spark spread for gas), **capacity market**, ancillary services, heat sold (district heating, industrial steam), tariff or contract for biomass and waste (gate fee), certificates; sensitivities: **efficiency (heat rate)**, availability, fuel cost, CO₂ (ETS), number of starts, degradation and LTSA costs.
- **Roles to activate in addition**: **Power island engineer (turbine / boiler / water-steam cycle)** (below). Reinforced roles: **commissioning** (the longest and most technical of all industrial sectors), **electrical** (generator, main transformer, HV), **HSE** (high-pressure steam, gas, biomass dust). **Process** becomes thermodynamics and water chemistry.
- **Phase skills and references available**: no dedicated phase skill; the cross-cutting EPC skills (claims / EOT, cost control, contractual letters and minutes, engineering register, multi-package reconciliation, gate war-game, steering challenger, portfolio cockpit) apply as they are.
- **Common units & ratios** (indicative): **MW gross / net** (auxiliaries 2–8% depending on technology), **net efficiency** (CCGT ~58–63% LHV at ISO conditions, biomass ~25–35%, WtE ~20–30% electrical), **heat rate** kJ/kWh, ISO conditions (15 °C, 1,013 mbar, 60% RH) and corrections, fuel **LHV** (biomass: moisture!), t/h of steam, steam pressure / temperature, **availability** ~90–95%, load factor, EOH (equivalent operating hours) for turbine maintenance, emissions in mg/Nm³ at reference O₂.
- **Key vocabulary**: gas turbine, HRSG, steam turbine, generator, condenser, air cooler / cooling tower, boiler (grate, fluidised bed), flue-gas treatment (SCR / SNCR, bag filter, electrostatic precipitator, scrubbing), ash and bottom ash, first fire, steam blowing, chemical cleaning, synchronisation, load tests, reliability run, performance test, heat rate, ISO conditions, degradation, LTSA / CSA, EOH, hot / cold start, grid code, black start, ancillary services, capacity market, spark spread, QAL, emission limit values, LCP / WI BREF.

## Sector-specific roles

### Power island engineer (turbine, boiler, water-steam cycle)
- **Mission**: accountable for the **guaranteed thermodynamic performance** (net output, heat rate, emissions) and for the OEM / BoP integration — the one who reads the heat balance and the correction curve.
- **Reading grid of a heat balance / an OEM guarantee**: (1) reference conditions (ISO or site) and **correction curves** (ambient temperature, pressure, humidity, LHV, power factor, degradation); (2) net / gross scope and list of auxiliaries included; (3) guarantee points (100%, part load, heat mode); (4) measurement tolerances (ASME PTC 46 / 22 / 4); (5) admitted recoverable / non-recoverable degradation; (6) cycling constraints (starts, ramps) vs the expected operating profile; (7) emissions guaranteed at which reference O₂ and which load.
- **Anchors (indicative)**: ~0.5–0.7% of output lost per °C of ambient above ISO on a gas turbine; non-recoverable degradation of a few % over the life; auxiliaries 2–4% (CCGT) to 8–10% (biomass / WtE); HRSG flue-gas outlet temperature ~80–100 °C.
- **Red flags**: guarantee at ISO conditions while the site is hot; gross output guaranteed when the sales contract is net; correction curves missing from the offer; contractual performance test without measurement tolerance; real cycling profile absent from the guarantees.
- **Senior eye**: "efficiency is won at design and lost in operation" — they check water chemistry, fouling and air in-leakage before blaming the turbine.

## Role inserts

### Project manager
- Project driven by the **power-island OEM** (lead times, performances, interfaces) and by the **TSO** (connection date); **commissioning** is the longest and most exposed phase (first fire, grid tests, reliability run). The PM holds the **alignment of dates**: fuel available, gas and electrical connection, operating permit, operating teams trained.
- Red flags: COD promised to the market (capacity, PPA) without commissioning margin; OEM / BoP interfaces not wrapped; fuel contract not signed at FID.

### Estimator
- Break down: **power island** (30–50% of CAPEX), mechanical BoP (cooling, water treatment, fuel), **flue-gas treatment** (heavy in biomass / WtE), electrical BoP (generator, main transformer, HV), civil (turbine foundations, stack, buildings), connections (electricity, gas), development; benchmark in €/MW **per technology** and per size (biomass €/MW do not compare with a CCGT).

### Cost controller
- Large OEM payment milestones (down payments, shipment, first fire, PAC) and currency; **performance LDs** quantified (€/kW shortfall, €/kJ/kWh of heat rate) as exposure; commissioning fuel cost (often significant and disputed: who pays the test gas?); LTSA as a long-term commitment outside CAPEX.

### Planner
- Typical critical path: **OEM turbine / generator / transformer (18–30 months)** → heavy foundations → island erection → BoP → **commissioning 6–12 months** (chemical cleaning, steam blowing, first fire, synchronisation, load tests, grid-code tests, reliability run, performance test); external milestones: TSO connection, gas, operating permit, fuel availability; connection windows imposed by the operator.

### Contract manager
- EPC with **multiple performance guarantees** (net output, heat rate, emissions, noise, availability, start-up) and **bonus / malus LDs**; contractual test method and tolerances (ASME PTC); OEM / BoP **wrap** or coordination; **LTSA** (scope, EOH, availability guarantees, parts); TSO connection agreement and grid code as contractual obligations; fuel contract (take-or-pay, quality, LHV, sustainability); in biomass / WtE: upstream contracts (wood, waste) that carry the revenue.

### Risk manager
- Dominant: **OEM delay**, **TSO / gas connection**, **performance** (heat rate, emissions), **fuel** (price, availability, quality, sustainability), **market** (spark spread, capacity), regulatory (ETS, BREF), acceptability (plume, trucks), cycling higher than planned (wear, LTSA).

### Financing & FID
- Project finance on PPA / capacity market / treatment contract (WtE, municipality) or balance-sheet financing; sensitivities: spread, availability, fuel cost, CO₂; CPs: connection, permits, fuel contract, EPC / OEM, LTSA.

### Project insurance
— nothing specific —

### Process engineer
- Becomes **thermodynamics and water chemistry**: heat balance and water-steam cycle, cooling sizing (water vs air — water permits), water treatment (demineralisation, boiler chemistry), combustion and **flue-gas treatment** (NOₓ: SCR / SNCR; dust; acids; dioxins in WtE), ash / bottom ash / APC residue management; in biomass: fuel preparation and drying, variable LHV.

### Mechanical engineer
- **Island** (turbines, generator — OEM), feedwater pumps, condenser, exchangers, fans, conveyors and shredders (biomass / WtE), boiler (grate, fluidised bed, tubes, refractories), stack; ASME / EN 12952 (boilers), API 611 / 612; shaft-line vibrations and alignment.

### Materials & corrosion engineer
- **High-temperature corrosion** (chlorine and alkalis in biomass / WtE: superheater corrosion — steel choice, Inconel overlays), ferritic / austenitic steels in HP steam, **FAC** (flow-accelerated corrosion) in the water-steam cycle, acid corrosion at the flue-gas outlet; killer pair: **under-alloyed superheater + chlorinated fuel**.

### Piping engineer
- **HP / HT steam** piping (EN 13480 / B31.1, creep, heavy stress, spring supports), feedwater lines, fuel gas, **steam blowing** to be designed; red flag: HP-line stress analysis done after the supports are ordered.

### Civil / structural engineer
- **Turbine foundations** (dynamic bases, DIN 4024, decoupling), boiler (heavy steelwork), **stack**, turbine buildings, basins and cooling towers, biomass silos and sheds, waste pit; wind / snow / seismic loads with the national annex.

### Geotechnical engineer
- Dynamic bases (dynamic soil parameters), deep foundations under island and stack, water table for the pits (WtE), old industrial sites (plant conversions: contaminated soils, existing foundations).

### Electrical engineer
- **Generator, main transformer and HV evacuation** (TSO), unit auxiliary transformer, MV / LV auxiliaries, **generator protections**, synchronisation, **grid code** (fault ride-through, reactive, frequency / voltage control, black start where applicable), emergency supply (diesel, UPS); long-lead transformers.

### Instrumentation engineer
- Boiler / turbine instrumentation (OEM), **protection systems** (BMS / burner management — NFPA 85 / EN 12952-8, steam safety), flue-gas analysers and **CEMS** (QAL 1/2/3 or 40 CFR 75), online water chemistry, energy metering; SIL on BMS and overpressure.

### DCS / control systems engineer
- DCS integrating the OEM automation (turbine, BMS), **load control and grid regulation** (frequency, TSO remote control), start-up / shutdown sequences, historian for performance, cybersecurity (critical site — NERC CIP-type regimes), separate SIS.

### HSE
- Hazards that kill: **high-pressure steam** (invisible leaks), **gas** (hazardous areas at the station and in the turbine hall), **biomass dust** (explosion, self-heating of stockpiles), confined spaces (boiler, silos, waste pit — H₂S / CO), **high voltage**, heavy lifts, heat; large sites: co-activity and cascaded subcontracting.

### Technical safety
- Hazard study (gas, storages), **boiler explosion / BMS**, biomass stockpile or waste-pit fire (IR detection, water spray), transformers (oil), generator hydrogen cooling, F&G at the gas station; "dumb" failures: steam water hammer, **condenser implosion**, re-ignition without purge.

### Environment & permitting
- **IED / LCP or WI BREF** (emission limit values, BAT, QAL monitoring) or the country's air permitting, environmental authorisation with public inquiry, **water** (abstraction, thermal discharge, towers), **noise**, ETS, biomass sustainability (RED), ash management plan; opposition sticking point: **plume, emissions, truck traffic** (biomass / WtE), the coal image in conversions.

### Procurement
- Long-lead: **gas turbine, steam turbine, generator, main transformer (18–30 months)**, boiler, flue-gas treatment, HRSG; concentrated OEM market (a few players) → negotiate the LTSA at the same time as the purchase; fuel as a strategic purchase (long-term contracts, wood / waste logistics).

### Construction manager
- Heavy erection: dynamic foundations, **turbine / generator / transformer lifts**, boiler and steelwork, HP piping (qualified welders, heat treatment), HV cabling; site of 500–2,000 people at peak; OEM (supervision) / BoP co-activity; cleanliness of the water-steam cycle.

### Quality (QA/QC)
- HP welds (NDT, PWHT, WPS / welder qualification), material certificates, **cycle cleanliness** (chemical cleaning, steam blowing with targets), boiler tests (hydrostatic), witnessed OEM FAT, transformer and generator tests, pressure-equipment dossiers.

### Commissioning
- **The key phase of the sector**: cold tests → **chemical cleaning** → **steam blowing** → **first fire** → pressure ramp-up → **synchronisation** (first connection to the grid, with the TSO) → load and protection tests → **grid-code tests** → **reliability run** (contractual period) → **performance test** (ASME PTC, corrected conditions) → PAC / COD. The milestone that counts is **synchronisation** (depends on the TSO) then PAC; test fuel and the sale of test electricity are contractual subjects to be settled beforehand.

### O&M (operations & maintenance)
- **LTSA / EOH** (turbine inspections: combustion, hot gas path, major), water chemistry, HRSG / boiler fouling, **performance degradation** (heat-rate tracking), cycling (fatigue), flue-gas treatment (consumables, QAL), ash management, contractual availability; operating teams trained before commissioning (they run the tests).

### Grid & utility connection
- **HV electricity (TSO)**: offer, agreement, grid code, capacity market, ancillary services; **gas (gas TSO)**: station, firm capacity, pressure; **heat**: district heating network; **water**: abstraction and discharge; the electrical connection is almost always the long pole.

### Interface manager
- **Island OEM ↔ BoP** (supply limits, design data, control), project ↔ TSO (synchronisation, tests), project ↔ operator (training, hand-over), project ↔ fuel supplier (logistics, quality), project ↔ heat network.

### Document control
- OEM documentation (manuals, curves, certificates), pressure-equipment and boiler dossiers, **performance-test and emissions reports** (QAL) — contractual and regulatory documents; as-built and operating dossier handed over before PAC.

### Site & stakeholder engagement
- Neighbours are a named counterpart (identity card): plume, and truck traffic for biomass and waste-to-energy; permits go through a public inquiry.

### Supply & offtake
- Both ends are FID locks (identity card): the **fuel contract** (gas; biomass — sustainable resource, price, duration, indexation; waste — treatment contract with the municipality) and the **offtake / market** (PPA, capacity market, heat).

## Country × sector notes (to be checked locally)

- **France**: ICPE 2910 / 3110 / 2770-2771, LCP / WI BREF, RTE (HV connection, capacity mechanism), ETS, biomass sustainability (RED), multiannual energy programme (place of gas and biomass).
- **Germany**: BImSchG + 13th / 17th BImSchV, KWKG (cogeneration), ÜNB for the connection, coal exit; **Belgium**: CRM (capacity market) and regional permits; **Poland**: capacity market, coal → gas / biomass conversions, URE; **Spain**: REE, Iberian market, State / regional authorisations.
- **United States**: NSR / Title V air permits, 40 CFR 75 CEMS, NERC reliability standards and interconnection queues, RTO capacity markets, NFPA 85 for combustion systems.
- **Gulf / Asia**: large CCGT and IPP programmes under long-term PPAs with state offtakers; desalination coupling in the Gulf; local grid codes and IEC/ASME mixed practice.

## Cross-cutting red flags of the sector

- **COD committed to the market without commissioning margin** (the longest and least predictable phase).
- **Performance guarantees at ISO conditions** while the site and the contract are at real / net conditions.
- **OEM / BoP interfaces not wrapped** → performance and time falling between two contracts.
- **Fuel contract not firm** (biomass: resource, sustainability; waste: municipality).
- **TSO connection handled as a formality**.
- **Real cycling ignored** in the guarantees and the LTSA.
