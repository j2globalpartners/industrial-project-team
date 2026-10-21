# Multi-country dimension — the cross-cutting layer

## What this file is for

The role sheets describe each trade **code-agnostic**, without a home country. This file is the **cross-cutting layer** that retunes every role once the project country is defined: a civil engineer does not read the same structural code, a permitting lead does not file the same dossier, a grid-connection lead does not talk to the same operator, a contract manager does not rely on the same default liability, and a financing structure does not carry the same tax risk. **Read it alongside the role sheet as soon as a project country is defined** — and read `standards-regimes.md` for the technical codes that apply there. Country notes are in `country-cards.md` (five cards shipped as examples); to add a country, start from `\_template-country.md`.

Rule of use: **never transpose the team's home practice as-is** — and never assume a regime when no country is defined: ask. The notes are points of vigilance and orders of magnitude; precise thresholds, rates and procedures must be checked locally and kept current. What depends on the **sector** (support scheme, permit categories, product specifications) lives in the sector profile, section "Country × sector notes"; what depends only on the **country** lives here.

## The nine axes that change from one country to another

For any role, these are the axes that move when a border is crossed. The senior reflex: ask, on each axis, "what is different here from the practice I know?"

1. **Permitting / environment** — which authority, which regime (national, regional, Land), which acceptability sticking point.
2. **Network connection** — which operator (gas, electricity, heat, H₂, water), which access right, which capacity (firm / flexible), which lead time.
3. **Support scheme / remuneration** — tariff, tender, certificates, guarantees of origin, offtake contract: *the mechanism depends on the sector* (see profile), but the arena (regulator, one-stop shop) depends on the country.
4. **Contract law** — default applicable law, statutory liabilities (ten-year liability?), local standards (CCAG, VOB/B…), governing language.
5. **Tax** — VAT (reverse charge), withholding taxes, SPV taxation, permanent-establishment risk.
6. **Labour / posting of workers** — posting declarations, A1 certificates, local site obligations, minimum wage.
7. **Technical standards regime** — which code families apply (Eurocodes with national annex, ASME/ASCE/NEC, BS, GB, IS, AS/NZS…), network standards, hazardous-area system, third-party inspection, units — **the map is `standards-regimes.md`**.
8. **Language \& governance** — language of the dossier and the procedure, governance of the local SPV, place of effective management.
9. **Market \& supply chain** — unit costs, labour, availability of local contractors, supplier origin standards (flanges, voltages).

## How each role retunes (reading by trade)

* **Environment / permitting**: changes the most. Regime, authority and calendar are *national* (even regional in BE / ES / DE). The acceptability sticking point is the sector's, but the administrative arena differs.
* **Grid connection**: counterpart and procedure entirely different per country (table below). The firm / flexible concept is universal; the actors are not.
* **Financing / FID**: bankability depends on the local support scheme and security law; the SPV structure raises the cross-border tax risk (§ substance).
* **Contract manager**: FIDIC remains a common base, but the **applicable law** and the **default statutory liabilities** (ten-year liability FR / BE, civil warranties) change the risk allocation — a point often underestimated when a contract is "copy-pasted" from one country to another.
* **Civil / geotechnical**: the country's structural code family **with its national annex or local seismic map** (climatic loads — snow, wind, seismicity — and coefficients differ). A calculation done under another country's annex is not valid here.
* **Electrical / instrumentation / DCS**: common IEC references but national installation and connection rules (voltage levels, protections, network decoupling, grid code).
* **Procurement / construction**: posting of personnel, local social declarations, contract taxation (VAT), flange / voltage standards depending on supplier origin (strong interface).
* **Cost / estimator**: unit costs, tax and local labour; benchmarks to be recalibrated by country.
* **HSE**: labour regulation and site references are national (SPS coordination FR, VCA BE/NL, SiGeKo DE…); the group requirement level remains the floor.

## Summary table — counterparts \& framework (nine example cards shipped; the regime map covers the rest)

|Country|Factories Nordzucker|Gas distribution|Gas transmission|Elec distribution|Elec transmission|Permitting (authority)|Energy regulator|Dossier language|Currency|
|-|-|-|-|-|-|-|-|-|-|
|🇫🇷 FR|none|GRDF (+ local DSOs)|NaTran (ex-GRTgaz) / Teréga|Enedis (+ local DSOs)|RTE|Prefect / DREAL (ICPE), DDT (planning)|CRE|French|EUR / €|
|🇧🇪 BE|none|ORES / Fluvius / RESA / Sibelga|Fluxys|ORES / Fluvius / RESA / Sibelga|Elia|Regional (permis unique WAL / omgevingsvergunning FL)|CWaPE / VREG / Brugel (reg.), CREG (fed.)|FR (WAL) / NL (FL)|EUR / €|
|🇵🇱 PL|Opalenica (OPA)<br />Chelmza (CHE)|PSG|GAZ-SYSTEM|OSD (Tauron, Enea, Energa, PGE, Stoen)|PSE|Decyzja środowiskowa (RDOŚ) + pozwolenie na budowę|URE|Polish|PLN|
|🇪🇸 ES|none|Nedgia / Redexis / Nortegas|Enagás|Distribuidoras (i-DE, e-distribución, UFD…)|REE|State / autonomous communities (autorización ambiental)|CNMC|Spanish (+ reg.)|EUR / €|
|🇩🇪 DE|Clauen (CLA)<br />Nordstemmen (NST)<br />Schladen (SLA)<br />Uelzen (UEL)<br />Klein Wanzleben (WZL)|VNB|FNB|VNB|ÜNB (Amprion, TenneT, 50Hertz, TransnetBW)|Land (BImSchG)|BNetzA|German|EUR / €|
|🇩🇰 DK|Nakskov (NYK)<br />Nykobing (NYK)|Local gas DSO|Energinet|Local netselskab|Energinet|Municipality / relevant environmental authority (VVM)|Forsyningstilsynet|Danish|DKK|
|🇸🇪 SE|Örtofta (ORT)|Local gas DSO|Nordion Energi / Swedegas|Local / regional nätbolag|Svenska kraftnät|Municipality / Länsstyrelsen / Land and Environment Court|Energimarknadsinspektionen (Ei)|Swedish|SEK|
|🇫🇮 FI|Porkkala (POR)<br />Säkylä (SÄK or SAK)|Local gas DSO|Gasgrid Finland|Local DSO|Fingrid|Municipality / competent national or regional authority (YVA / environmental permit)|Energiavirasto|Finnish / Swedish where applicable|EUR / €|
|🇱🇹 LT|Kedainiai (KED)|ESO|Amber Grid|ESO|Litgrid|Municipality / environmental authority (PAV / statybos leidimas)|VERT / NERC|Lithuanian|EUR / €|

*(Actors and competences given as reference points — to be confirmed project by project. Detail per country in `country-cards.md`.)*

## The substance / permanent-establishment risk (cross-border governance)

Critical point when a **team based in one country** runs an **SPV located in another** (foreign SPV, management from the team's country — or the reverse). Two symmetrical risks:

* **Unintended permanent establishment**: the team's activity on behalf of the foreign SPV can create a *permanent establishment* in the team's country, or the reverse.
* **Place of effective management**: a foreign SPV **managed from the team's country** can be deemed a tax resident there (place of effective management), with a risk of double taxation or requalification.

Reflexes:

* **Document substance** in the SPV's country (decision-making bodies, board, signatures, meetings held locally).
* **Formalise intra-group services** (service agreement, transfer pricing) between the managing entity and the SPV.
* **Map who decides what and where** (DOA, RACI, governance) — these governance deliverables are the proof of substance.
* Deal with it upstream with **corporate tax / legal**: this is not a subject to discover at the first audit.

## Cross-cutting red flags

* **Home practice transposed as-is** (permit regime, network operators, statutory liabilities, contract forms) in another country.
* **Structural calculation under another country's national annex or code** used on the site (different snow / wind / seismic loads).
* **Network capacity assumed** without having identified the right local operator and its access regime (firm / flexible).
* **VAT not reverse-charged** where the local regime requires it (30bis / co-contractor BE, §13b DE, inversión del sujeto pasivo ES, reverse charge FR).
* **Undeclared posting of workers** (Limosa BE, SIPSI FR, Mindestlohn / Zoll DE, RUT DK) or missing A1 certificates; also check country-specific site-registration duties such as `personalliggare` in SE and `veronumero` in FI.
* **Foreign SPV run from the team's country without documented substance** — permanent-establishment / effective-management risk.
* **Governing contract language** not identified (a "bilingual" contract always has a version that prevails).
* **Support scheme assumed stable** while it is changing — to be re-checked at every milestone, in the sector profile.
* **Regionalisation ignored** in BE / ES / DE (the rule is not national but regional / Land).

## Cross-cutting vocabulary and acronyms

* **A1** (posted worker's social security), **permanent establishment**, **place of effective management**, **transfer pricing**, **national annex (NA)** to the Eurocodes, **reverse charge**, **grid code**, **SPV**, **DOA**.
* **FR:** ICPE, DREAL, DDT, CRE, GRDF, NaTran, Teréga, Enedis, RTE, PTF, S3REnR, décennale, CCAG, SIPSI, SPS, ZAN.
* **BE:** permis unique, permis d'environnement, omgevingsvergunning, CWaPE, VREG, Brugel, CREG, ORES, Fluvius, RESA, Sibelga, Fluxys, Elia, Synergrid, flexible-access, green certificates, 30bis, VAT co-contractor / medecontractant, Limosa, VCA.
* **PL:** decyzja środowiskowa, pozwolenie na budowę, warunki przyłączenia, RDOŚ, URE, GAZ-SYSTEM, PSG, PSE, OSD, split payment, BHP, PLN.
* **ES:** autorización ambiental, DIA, comunidad autónoma, CNMC, Enagás, Nedgia, Redexis, Nortegas, REE, permisos de acceso y conexión, PNIEC, IVA, inversión del sujeto pasivo, LOE, REA.
* **DE:** BImSchG, 4. BImSchV, UVP, Land, BNetzA, VNB, FNB, ÜNB, VDE-AR-N, DVGW, EEG, VOB/B, BGB, USt, Reverse-Charge §13b, Mindestlohn, SiGeKo.
* **DK:** Miljøbeskyttelsesloven, VVM, Energistyrelsen, Energinet, Forsyningstilsynet, netselskab, nettilslutning, fjernvarme, AB 18, ABT 18, ABR 18, Arbejdstilsynet, RUT, BR18, DS/EN, totaløkonomi.
* **SE:** Miljöbalken, Plan- och bygglagen (PBL), MKB, samråd, Länsstyrelsen, mark- och miljödomstol, Energimarknadsinspektionen (Ei), Energimyndigheten, Svenska kraftnät, nätkoncession, EKS, Klimatklivet, Elsäkerhetsverket, Arbetsmiljöverket, personalliggare.
* **FI:** Ympäristönsuojelulaki, YVA, elinvoimakeskus, Energiavirasto, Business Finland, Fingrid, Gasgrid Finland, YSE 1998, KSE, SFS-EN, työturvallisuus, veronumero, energiatehokkuus, toimitusvarmuus, huoltovarmuus, elinkaarikustannus.
* **LT:** PAV, statybos leidimas, Aplinkos apsaugos įstatymas, VERT / NERC, ESO, Litgrid, Amber Grid, STR, ES fondai, Modernisation Fund, FIDIC, darbuotojų sauga ir sveikata, LST EN, atsipirkimo laikotarpis, prijungimo sąlygos.
* Keep the detailed definitions and project-specific caveats in `country-cards.md`.

## Reflexes / obsessions

* **"What is different here, on each of the 9 axes, from the practice I know?"** — the basic reflex.
* **"Who is the local network operator, and what is its access regime?"**
* **"Under which code and national annex was this structural calculation done?"**
* **"Does the local VAT regime require reverse charge? Is the posting of workers declared?"**
* **"Does the foreign SPV have substance where it sits, or is it run from abroad?"**
* **"Is the support scheme I am assuming still current in this country?"**
* **"Which language governs the contract?"**
* Regional reflex in BE / ES / DE: never reason "national" without checking the regional / Land level. Nordic reflex in DK / SE / FI: engage authorities, municipalities, network operators and affected stakeholders early; in LT, clarify utility capacity, connection conditions and EU-funding dependencies early.

## Typical internal interfaces

* With **financing / FID**: SPV structure, local securities, substance risk, support scheme.
* With the **contract manager**: applicable law, default statutory liabilities, governing language.
* With **environment / permitting**: local regime and authority, administrative calendar.
* With the **grid-connection** sheet: network counterparts and access regime by country.
* With **civil / geotechnical**: national annexes to the Eurocodes (loads, seismicity).
* With **procurement / construction**: posting of workers, contract VAT, supplier origin standards.
* With **corporate tax / legal** (outside the project team): permanent establishment, transfer pricing, securities.

## Tone and posture

Cautious and systematic: asks the right questions per country rather than asserting certainties (regulatory detail changes fast and by region). Refuses the copy-paste of home practice. Knows that the value of a multi-country operator is precisely **not to be surprised** by what changes at the border — network counterpart, VAT regime, normative annex, or substance risk. Systematically refers to local counsel (tax, legal, permitting) for binding detail, while knowing how to frame the questions.

## Standards / references \& cross-references

* **Technical standards regimes** by country group and discipline: `standards-regimes.md` (Eurocodes with national annexes, ASME/ASCE/ACI/NEC, BS, GB, IS, AS/NZS, SANS, SNI, KDS, NCh…).
* Network standards: operator requirements (FR), Synergrid (BE), DVGW / VDE-AR-N (DE), IRiESP / IRiESD (PL), CNMC / REE standards (ES), Energinet and local DSO requirements (DK), Svenska kraftnät and local / regional network requirements (SE), Fingrid and local DSO requirements (FI), Litgrid / ESO requirements (LT).
* Tax / labour: VAT and posting regimes by country (to be handled with local counsel).
* **Sheet cross-references**: `grid-connection`, `financing-fid`, `contract-manager`, `environment-permitting`, `civil-engineer`, `geotechnical-engineer`, `procurement`, `risk-manager`, `hse`.
* **Sector cross-reference**: section "Country × sector notes" of the active profile (`sectors/<profile>.md`).

