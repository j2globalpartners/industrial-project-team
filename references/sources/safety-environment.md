# Documentary sources — electrical, control systems, safety, environment

Cross-cutting reference. Lists, by role, the authoritative documents that support the role sheet, and the facts that can be drawn from them.

**Verification status (research of 13 November 2026).** None of these pages could be opened: the research session had access only to the search engine, not to the websites. Every URL was returned by the search engine; every fact comes from a search-result extract or from a secondary source. **Only the facts tagged [V] were subsequently read in the text**, during a second pass on AIDA, INRS, Ineris and the code du travail numérique [the French online labour code]; Légifrance and EUR-Lex could not be opened. Everything else is to be re-read at the source before any regulatory use.

Fact tags: **[V]** read in the document itself on 13 November 2026 · **[E]** search-engine extract, document not opened · **[S]** concordant secondary source · **[NC]** not confirmed, to be re-read in the text.

## Electrical engineer

| Source | URL | Access |
|---|---|---|
| IEC 60909-0:2016, calculation of short-circuit currents | https://webstore.iec.ch/en/publication/24100 | paid |
| Schneider Electric, Cahier technique no. 158, calculation of short-circuit currents | https://www.se.com/us/en/download/document/ECT158/ | free |
| NF C 15-100, recast series (August 2024) — AFNOR announcement | https://www.afnor.org/en/news/low-voltage-electrical-installations-nf-c15-100-parue | paid, free announcement |
| NF C 13-100 (2015) and NF C 13-200 | https://www.boutique.afnor.org/en-gb/standard/nf-c13100/consumer-substations-installed-inside-a-building-and-fed-by-hv-public-distr/fa107462/18450 | paid |
| Directive 1999/92/EC (ATEX workplaces) | https://eur-lex.europa.eu/eli/dir/1999/92 | free |
| INRS ED 945, implementation of the ATEX regulations (2020) | https://www.inrs.fr/media.html?refINRS=ED+945 | free |
| Ineris, Oméga 36, practical guide to the prevention of ATEX risk (2025) | https://www.ineris.fr/sites/default/files/contribution/Documents/Om%C3%A9ga%2036%20-%20Guide%20pratique%2C%20pr%C3%A9vention%20du%20risque%20ATEX_Octobre%202025.pdf | free |

- In France, **NF C 15-100 (low-voltage installations) was recast in August 2024** into a series of 21 standards; the dates of application vary from one source to another [S]. Where a sheet cites the standard without its year, specify the edition applicable to the project.
- IEC 60909-0:2016 incorporates the contribution of wind farms and of converter-connected generating units [E].
- In France, boundary between the high-voltage standards: NF C 13-100 for the delivery substation fed from the public HTA (medium-voltage) network, NF C 13-200 for the private high-voltage installation [E].
- ATEX zones: zone 0/20, explosive atmosphere present continuously or frequently; zone 1/21, occasional in normal operation; zone 2/22, unlikely or of short duration. Category 1 equipment in zone 0/20, 1 or 2 in zone 1/21, 1 to 3 in zone 2/22 [S].

## Instrumentation engineer

| Source | URL | Access |
|---|---|---|
| IEC 61511-1:2016 + AMD1:2017, safety instrumented systems | https://webstore.iec.ch/publication/61289 | paid |
| The 61508 Association, "SIL Calculations and use of IEC 61508-6" (2024) | https://61508.org/wp-content/uploads/2024/11/10B-SIL-Calculations-and-use-of-IEC-61508-6.pdf | free |
| IChemE, Hazards XXIV, paper 18 (reproduces the SIL tables) | https://www.icheme.org/media/8914/xxiv-paper-18.pdf | free |
| Ineris, Oméga 10, technical safety barriers | https://www.ineris.fr/sites/default/files/contribution/Documents/DRA-17-164432-10199B_OMEGA10_VF_.pdf | free |
| Ineris, Oméga 20, human safety barriers | https://primarisk.ineris.fr/node/3608 | free |

- SIL in low-demand mode (average probability of failure on demand): SIL 1 from 10⁻² to 10⁻¹; SIL 2 from 10⁻³ to 10⁻²; SIL 3 from 10⁻⁴ to 10⁻³; SIL 4 from 10⁻⁵ to 10⁻⁴ [S]. Consistent with the sheet.
- SIL in high-demand mode (dangerous failures per hour): SIL 1 from 10⁻⁶ to 10⁻⁵, up to SIL 4 from 10⁻⁹ to 10⁻⁸ [S].
- Low demand: function demanded no more than once a year [S].
- In France, the Ineris Oméga 10 and Oméga 20 methods assess technical and human barriers in hazard studies (études de dangers) [E].
- Nothing verified on control valves (IEC 60534) or on architectural constraints [NC].

## DCS / control systems engineer

| Source | URL | Access |
|---|---|---|
| IEC 62682:2022, management of alarm systems | https://webstore.iec.ch/publication/65543 | paid |
| ANSI/ISA-18.2-2016 | https://www.isa.org/products/ansi-isa-18-2-2016-management-of-alarm-systems-for | paid |
| EEMUA 191, 4th ed. (November 2024) — table of contents | https://eemua.org/getattachment/9d3f8071-55c3-49bf-a74a-3bf6ad4a2e0f/Contents-EEMUA-Publication-191-Edition4-November-2024.pdf | paid, free table of contents |
| ANSSI [French national cybersecurity agency], cybersecurity of industrial systems — classification method, v2.0 (March 2025) | https://cyber.gouv.fr/sites/default/files/document/anssi-guide-systemes_industriels-methode_de_classification_v2-0.pdf.pdf | free |
| ANSSI, detailed measures, v2.0 (November 2025) | https://messervices.cyber.gouv.fr/documents-guides/Guide_Systemes_industriels__Mesures_detaillees_v2.pdf | free |
| IEC 62443, overview page | https://syc-se.iec.ch/deliveries/cybersecurity-guidelines/security-standards-and-best-practices/iec-62443/ | free summary |

- ISA-18.2 indicators, per operator position, over at least 30 days: about 150 alarms per day "very likely to be acceptable", 300 per day "maximum manageable"; fewer than 1% of ten-minute periods above ten alarms [S]. Consistent with the sheet.
- Standing alarms (active for more than 24 hours): fewer than five per day; chattering or fleeting alarms: target zero [S].
- Alarm flood according to EEMUA 191: begins above ten new alarms in ten minutes [S]. **The edition in force is the 4th (2024)**, not the 3rd of 2013.
- In France, **the ANSSI guide was recast in 2025**: four cybersecurity classes instead of three, classification by zones [S].
- IEC 62443: zones and conduits, seven foundational requirements, security levels [E].
- No standard dedicated to the cause and effect matrix has been identified [NC].

## HSE

| Source | URL | Access |
|---|---|---|
| IEC 61882:2016, HAZOP studies — application guide | https://webstore.iec.ch/publication/24321 | paid |
| CCPS, Layer of Protection Analysis (2001) | https://aiche.org/ccps/resources/tools/lopa | paid |
| INRS ED 6184, confined spaces (2016) | https://www.inrs.fr/media.html?refINRS=ED+6184 | free |
| INRS ED 703, ventilation of confined spaces (2015) | https://www.inrs.fr/media.html?refINRS=ED%20703 | free |
| INRS ED 941, work by outside contractors | https://inrs.fr/dam/inrs/CataloguePapier/ED/TI-ED-941.pdf | free |
| Code du travail [French labour code], article R. 4512-7 | https://code.travail.gouv.fr/code-du-travail/r4512-7 | free |
| INRS, regulatory framework of health-and-safety coordination (coordination SPS) | https://www.inrs.fr/metiers/btp/coordination-sps/reglementation.html | free |

- In France, a written prevention plan (plan de prévention) is required before work in two cases: an operation of at least 400 foreseeable working hours over twelve months at most, subcontractors included, or hazardous work listed by order, whatever its duration (article R. 4512-7) [V]. The joint prior inspection precedes the drawing-up of the plan, for each operation [V].
- In France, health-and-safety coordination (coordination SPS, article R. 4532-1): category 1 above 10,000 man-days with at least ten contractors (building) or five (civil engineering); category 2 above 500 man-days, or a site lasting 30 days with more than 20 workers at peak; category 3 for the rest. Category 1 requires an inter-contractor safety committee (collège interentreprises de sécurité) [V].
- Confined spaces (INRS guidance, France): every entry is subject to an entry permit validated on the spot by the person in charge of the operation; an attendant is mandatory, with the means to reach the workers and the emergency services without leaving his post [V]. Oxygen and lower-explosive-limit thresholds: not found in the page read [NC].
- An independent protection layer must be effective, independent of the initiating event and of the other layers, and auditable [S].

## Technical safety

| Source | URL | Access |
|---|---|---|
| Arrêté du 29 septembre 2005 [French order on probability, kinetics, intensity and severity in hazard studies] | https://aida.ineris.fr/reglementation/arrete-290905-relatif-a-levaluation-a-prise-compte-probabilite-doccurrence-cinetique | free |
| Circulaire du 10 mai 2010 [French circular on the methodological rules for hazard studies] | https://aida.ineris.fr/reglementation/circulaire-100510-recapitulant-regles-methodologiques-applicables-etudes-dangers-a | free |
| Ineris, Oméga 9, hazard study of a classified installation (2015) | https://prestations.ineris.fr/sites/default/files/PrestaWeb/Pages-Solution/Documents%20Associ%C3%A9s/Omega9.pdf | free |
| HSE (United Kingdom), Reducing risks, protecting people (2001) | https://www.hse.gov.uk/enforce/expert/r2p2.htm | free |
| ISA-TR84.00.07-2018, effectiveness of fire and gas detection systems | https://www.isa.org/products/isa-tr84-00-07-2018-guidance-on-the-evaluation-of | paid |

- In France, thresholds for effects on people (Annex II of the arrêté du 29 septembre 2005): thermal 3, 5 and 8 kW/m², or as a dose 600, 1,000 and 1,800 [(kW/m²)^4/3].s; overpressure 50, 140 and 200 mbar — irreversible effects, lethal effects, significant lethal effects. 20 mbar marks the limit of indirect effects through broken glass [V].
- In France, thresholds for effects on structures (same order): overpressure 20 mbar (glazing), 50 (minor damage), 140 (serious damage), **200 (domino effects)**, 300 (very serious damage); thermal 5 kW/m² (glazing), **8 (domino effects)**, 16 (prolonged exposure, excluding concrete), 20 (concrete withstands for several hours), 200 (collapse of concrete) [V]. The HSE sheet previously gave 300 mbar for domino effects; the sheet has been corrected accordingly.
- Toxic thresholds under the same French order: lethal effects correspond to a lethal concentration of 1%, significant lethal effects to 5% [V].
- In France, the 2005 order was amended by an order of 4 September 2025, which adds a title on the maps of effect zones to be attached to the hazard study [V].
- Probability under the same French order: five classes A to E [V]; their numerical bounds (10⁻⁵ to 10⁻² per year) and the severity scale appear in tables that the reading did not render [S].
- In France, criticality grid of the 2010 circular: 25 cells, "NO" cells ranked 1 to 4 and risk-control-measure cells ranked 1 to 2 [E].
- UK tolerability framework: three regions — unacceptable, tolerable if reduced as low as reasonably practicable, broadly acceptable [E]. Numerical bounds of individual risk [NC].
- Fire and gas detection: geographic coverage measures the share of a zone that is monitored, scenario coverage the share of scenarios detected; no standard sets a target rate [S].

## Environment & permitting

| Source | URL | Access |
|---|---|---|
| Instruction du 28 octobre 2024 [French instruction on the environmental permit procedure] | https://aida.ineris.fr/reglementation/instruction-281024-relative-a-procedure-dautorisation-environnementale | free |
| DRIEAT Île-de-France, guide to the environmental permit (November 2025) | https://www.drieat.ile-de-france.developpement-durable.gouv.fr/IMG/pdf/20251125_guide_autorisation_environnementale.pdf | free |
| Décret n° 2024-423 du 10 mai 2024 [French decree on litigation procedure for environmental permits] | https://aida.ineris.fr/reglementation/decret-ndeg-2024-423-100524-portant-adaptation-procedure-contentieuse-relative | free |
| Revised IED directive — EUR-Lex summary | https://eur-lex.europa.eu/FR/legal-content/summary/industrial-and-livestock-rearing-emissions.html | free |
| AIDA, access to the BREFs and guide to the IED review (2020) | https://aida.ineris.fr/guides/documents-bref | free |
| AIDA, Seveso establishments | https://aida.ineris.fr/inspection-icpe/risques-accidentels/seveso/etablissements-seveso | free |

- In France, **the "industrie verte" [green industry] reform**: for applications filed on or after 22 October 2024, the examination of the application and the public consultation run in parallel; the consultation, conducted online, lasts three months and includes one opening and one closing public meeting [V, instruction du 28 octobre 2024]. Stated objective: to bring the average lead time down from 17 to 9 months [S]. Exact duration of the phases [NC].
- In France, **third-party appeals: two months instead of four** for decisions taken on or after 1 September 2024 (décret n° 2024-423) [V]. The appeal must be notified to the author and to the beneficiary of the decision, by registered letter, within fifteen clear days, failing which it is inadmissible; rule applicable since 1 January 2024 (décret n° 2023-1103, article R. 181-51) [V]. Extension through an administrative appeal for reconsideration (recours gracieux) [S]. Some prefecture web pages still display four months.
- In France, opinion of the environmental authority: two months for a regional mission, three months otherwise. Case-by-case screening: decision within 35 days, silence amounting to an obligation to carry out an environmental impact assessment [E].
- Revised IED directive: entry into force on 4 August 2024, transposition by 1 July 2026; new BREFs announced, including water electrolysis and batteries [E].
- IED review (as applied in France): file due within the year following publication of the conclusions on best available techniques for the main activity heading [E].
- Upper-tier Seveso (as applied in France): hazard study updated at least every five years; emergency plans tested and reviewed every three years [V].

## Not found

Annexes of the arrêté du 29 septembre 2005 (toxic thresholds, headcounts of the severity scale); code articles on Légifrance; texts of the directives on EUR-Lex; IEC 61508; discrimination (selectivity) and earthing systems; guide words of IEC 61882; website of the European BREF bureau; the ICPE nomenclature [French classified-installations nomenclature].
