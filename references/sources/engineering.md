# Documentary sources — engineering (process, mechanical, materials, piping, civil, geotechnical)

Cross-cutting reference. Lists, by role, the authoritative documents that support the role sheet, and the facts that can be drawn from them.

**Verification status (research of 13 November 2026).** None of these pages could be opened: the research session had access only to the search engine, not to the websites. Every URL was returned by the search engine; every fact comes from a search-result extract or from a secondary source. **Only the facts tagged [V] were subsequently read in the document itself**, during a second pass (Ineris, Infociments, AFGC, Syntec-Ingénierie). Almost all the standards cited are paid documents: for a design value, only the standard in force is authoritative.

Fact tags: **[V]** read in the document itself on 13 November 2026 · **[E]** search-engine extract, document not opened · **[S]** concordant secondary source · **[NC]** not confirmed, to be re-read in the text.

## Process engineer

| Source | URL | Access |
|---|---|---|
| API Standard 521, Pressure-relieving and Depressuring Systems, 7th ed. (2020) | https://www.api.org/products-and-services/standards/important-standards-announcements/standard521 | paid |
| ANSI/ISA-5.1-2024, Instrumentation and Control Symbols and Identification | https://www.isa.org/standards-and-publications/isa-standards/isa-standards-committees/isa5-1 | paid |
| ISO 10628-1:2014, diagrams for the chemical and petrochemical industry | https://www.iso.org/standard/51840.html | paid |
| Ineris, sheet « Barrière technique de sécurité — soupapes de sécurité » [technical safety barrier — safety relief valves], v3.0 (2024) | https://www.ineris.fr/fr/document-synthese-relatif-barriere-technique-securite-bts-soupapes-securite | free |
| Ineris, Oméga 10, assessment of technical safety barriers | https://www.ineris.fr/sites/default/files/contribution/Documents/DRA-17-164432-10199B_OMEGA10_VF_.pdf | free |
| CCPS, Guidelines for Pressure Relief and Effluent Handling Systems, 2nd ed. (2017) | — | paid |

- API 521 requires the causes of overpressure to be examined one by one, the relief rate to be determined for each, and then the system to be designed [E]. The named list of scenarios has not been re-read [NC].
- A conventional safety instrumented function does not replace a relief valve sized against a single-failure scenario [S, quotation from API 521].
- Allowable accumulation (ASME VIII): 10% single valve, non-fire; 16% multiple valves; 21% fire case [S; these rules are reported to have migrated to Section XIII, NC].
- ISA-5.1 changed its title in 2024 ("and Control"); its annexes have become technical reports [E].
- The Ineris sheet (France) assesses a relief valve as a barrier against its performance criteria: effectiveness, response time, failure modes and confidence level [V].

## Mechanical engineer

| Source | URL | Access |
|---|---|---|
| API Standard 610 (identical to ISO 13709), centrifugal pumps | https://www.api.org/products-and-services/standards/digital-catalog | paid |
| ANSI/HI 9.6.3-2024, Guideline for Operating Regions, Hydraulic Institute | https://www.pumps.org/2022/03/21/reliability-basics-understanding-npsh-por-and-aor/ | paid, free article |
| Hydraulic Institute / Europump, Pump Life Cycle Costs — DOE summary (2001) | https://www.energy.gov/sites/prod/files/2014/05/f16/pumplcc_1001.pdf | free |
| Directive 2014/68/EU, pressure equipment | https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32014L0068 | free |
| ASME BPVC Section VIII Division 1 | https://asme.org/codes-standards/find-codes-standards/bpvc-viii-1-bpvc-section-viii-rules-construction-pressure-vessels-division-1 | paid |
| Implementing Decision (EU) 2025/165, harmonised references (EN 13445) | https://eur-lex.europa.eu/eli/dec_impl/2025/165/oj | free |

- API 610: preferred operating region from 70 to 120% of best-efficiency-point flow; rated flow between 80 and 110% [S; clause number in the current edition NC]. Consistent with the sheet.
- Hydraulic Institute: the preferred region is the one in which the flow remains close to shockless entry into the impeller; the allowable region is the one in which the pump can operate outside the preferred region, with a reduced service life; the NPSH margin required depends on the region [V]. Typical width 70 to 120%, varying with specific speed [E].
- Pumping systems account for nearly 20% of world electricity demand and 25 to 50% of the consumption of certain plants [V, summary of the Hydraulic Institute / Europump guide]. Life cycle cost: initial investment, installation, energy, operation, maintenance, production downtime, environment, decommissioning [E].
- Directive 2014/68/EU: applies above 0.5 bar; for a vessel containing a Group 1 gas, entry threshold at V > 1 L and PS·V > 25 bar·L; below that, sound engineering practice without CE marking; four risk categories [E]. Mapping of categories → conformity assessment modules [NC].
- ASME VIII: Division 1 above 15 psig; Division 2, alternative, more demanding rules with higher allowable stresses; Division 3 for very high pressure [E].

## Materials & corrosion engineer

| Source | URL | Access |
|---|---|---|
| API RP 571, Damage Mechanisms Affecting Fixed Equipment in the Refining Industry, 3rd ed. (2020) | https://store.accuristech.com/api/products/preview/2108271 | paid |
| ANSI/NACE MR0175 / ISO 15156 (2020), materials for H₂S environments — AMPP excerpt | https://store.ampp.org/download/sample/52224 | paid, free excerpt |
| Emerson/Fisher guide to NACE MR0175 | https://www.emerson.com/is/content/emerson/en/final-control/flow-controls/documents/d351798x012_09.pdf | free |
| API 579-1 / ASME FFS-1, Fitness-For-Service — overview (State of California) | https://www.dir.ca.gov/dosh/pressure-vessels/documents/API-579-Fitness-for-Service-Overview.pdf | free |
| NACE TM0212-2018, internal microbiologically influenced corrosion of pipelines | https://webstore.ansi.org/preview-pages/NACE/preview_NACE+TM0212-2018.pdf | free preview |
| R. Marchal, « Rôle des bactéries sulfurogènes dans la corrosion du fer » [role of sulphide-producing bacteria in the corrosion of iron], Rev. IFP (1999) | https://ogst.ifpenergiesnouvelles.fr/articles/ogst/pdf/1999/05/marchal_v54n5.pdf | free, in French |

- API RP 571 lists some sixty damage mechanisms [S].
- H₂S service: the partial-pressure threshold of 0.3 kPa (0.05 psi) is the **historical** definition, still relevant for sulphide stress cracking of carbon and low-alloy steels; the current standard defines sour service by the capacity of the environment to crack the material [E].
- Usual maximum hardness: 22 HRC, or 250 HV under conditions [S].
- Fitness for service: three assessment levels, from conservative screening to specialist analysis [E].
- A rewrite of the ISO 15156 series is being drafted (2025): check the edition before citing a clause.

## Piping engineer

| Source | URL | Access |
|---|---|---|
| ASME B31.3, Process Piping, 2024 edition — table of contents of the 2022 edition | https://www.asme.org/getmedia/2d6bec7b-1177-4ee1-82ea-e5d5a86abab7/B31-3_2022_ToC.pdf | paid, free table of contents |
| Becht, "ASME B31.3 Process Piping: Changes in the 2024 Edition" | https://becht.com/?p=14168 | free |
| EN 13480, metallic industrial piping, 2024 edition | https://www.evs.ee/en/evs-en-13480-5-2024 | paid |
| Directive 2014/68/EU, Annex I §7.4 (proof test) | https://www.legislation.gov.uk/eudr/2014/68/annex/I/division/2/2020-12-31/data.pdf | free |
| CLAP sheets (French interpretations of the directive), UNM | https://unm.fr/wp-content/uploads/2022/10/clap57f.pdf | free |

- ASME B31.3: an edition becomes applicable six months after its date of issue; the 2024 edition is dated 27 December 2024 [E].
- Fluid service categories: "Normal" by default, "Category D" (low pressure and moderate temperature), "Category M" (the most hazardous fluids), high pressure. **The choice rests with the owner** [S].
- B31.3 hydrostatic test: 1.5 times the design pressure [S]. Consistent with the sheet.
- Proof test under the directive: the greater of 1.25 × the maximum loading in service and 1.43 × PS; according to a CLAP sheet (France) this point is aimed at vessels, and its application to piping is a matter of interpretation [E].
- Pump nozzle loads: project practice is to ask the manufacturer early to agree to twice the allowable values of API 610 [S].

## Civil / structural engineer

| Source | URL | Access |
|---|---|---|
| Eurocodes, Joint Research Centre website | https://eurocodes.jrc.ec.europa.eu/en-eurocodes | free |
| Infociments, concrete exposure classes | https://www.infociments.fr/betons/notions-de-classes-dexposition | free |
| AFGC, « Bien prescrire les bétons » [specifying concrete properly], sheet 2.1 Exposure classes (2023) | https://www.afgc.asso.fr/app/uploads/2023/02/2_1_RECO_Classe_exposition_saison-2-20230214.pdf | free |
| AFGC, note 5.2, determination of concrete cover | https://www.afgc.asso.fr/app/uploads/2016/10/5_2_NI_Determination_Enrobage_armatutres.pdf | free |
| DIN 4024-1 and -2, machine foundations | https://webstore.ansi.org/standards/din/din40241988 | paid |
| ACI 351.3R-18, Report on Foundations for Dynamic Equipment | https://www.concrete.org/Portals/0/Files/PDF/Previews/351.3R-18_preview.pdf | free preview |

- The Eurocodes comprise ten standards and 58 parts; the second generation is being rolled out (CEN deadline of 30 March 2026). State which generation is meant before citing a clause [E].
- NF EN 206/CN (the French edition of EN 206 with its national complement): 18 exposure classes, grouped by risk of corrosion (XC, XD, XS) and of attack on the concrete (XF, XA) [V].
- In France, **the choice of exposure classes is the responsibility of the project owner (maître d'ouvrage)**, assisted where applicable by the design and supervision consultant (maître d'œuvre) [V]; for XA, specify the aggressive agent [E].
- Concrete cover: the structural class associated with a design working life of 50 years is S4; the classes run from S1 to S6 [V]. Increase for 100 years and execution tolerance of 10 mm [E].
- Machine foundation blocks: DIN 4024-1 deals with flexible structures, DIN 4024-2 with rigid foundations; no numerical criterion (mass ratio, frequency separation) has been confirmed [NC].

## Geotechnical engineer

| Source | URL | Access |
|---|---|---|
| NF P 94-500 (November 2013), geotechnical engineering missions | https://www.boutique.afnor.org/en-gb/standard/nf-p94500/geotechnical-engineering-missions-classification-and-specifications/fa177810/1408 | paid |
| Syntec-Ingénierie, application guide to NF P 94-500 (2015) | https://www.syntec-ingenierie.fr/app/uploads/2015/01/2015-05-07.Guide-eco-application-norme-nfp94-500-missions-geotechniques.pdf | free |
| Cerema, Eurocode 7 — shallow foundations (NF P94-261), guide (2015) | https://piles.cerema.fr/IMG/pdf/cerema_guide_methodologique_eurocode7_application_aux__fondations_superficielles__nf_p94-261__decembre_2015_cle27e8f2-1.pdf | free |
| Cerema, Eurocode 7 — deep foundations (NF P94-262), guide (2014) | https://piles.cerema.fr/IMG/pdf/cerema_guide_methodologique_eurocode7_application_aux__fondations_profondes__nf_p94-262__decembre_2014_cle737925-1.pdf | free |
| Arrêté du 22 juillet 2020 [French order on the content of geotechnical studies in clay shrink-swell areas] | https://www.aube.gouv.fr/contenu/telechargement/25211/162954/file/200722_ARRETE_CONTENU_ETUDES.pdf | free |

- In France, 2013 version of the standard NF P 94-500, according to the Syntec-Ingénierie guide: G1 = site study followed by general construction principles; G5 = diagnosis, during a project or on an existing structure [V]. **G1, G2 and G4 are carried out on behalf of the project owner (maître d'ouvrage)** [V]. Consistent with the sheet.
- Under the same French standard, the G1, G2 and G3/G4 missions must follow one another and all be carried out (article 4.2); a G2 is done only after a G1, and it is recommended that they be entrusted to the same engineering firm; a mission may not cover only part of a set of interacting geotechnical structures [V].
- French design methods: pressuremeter-based (Ménard test) and penetrometer-based, for bearing capacity as well as for settlement [E].
- In France, Eurocode 7 applies with a national annex and six application standards, currently under revision [S].

## Not found

API product pages (520, 617, 650, 660); text of ASME B31.3; tables of Annex II of the pressure equipment directive (piping thresholds, modules); values of the cover tables of Eurocode 2; numerical criteria of DIN 4024; documents of the Union syndicale géotechnique [French geotechnical trade association]; in-situ testing standards; French guide on biocorrosion.
