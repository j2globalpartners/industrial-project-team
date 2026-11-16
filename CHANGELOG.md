# Changelog

Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/); versions follow [SemVer](https://semver.org/).

## [1.1.0] — 2026-11-13

Thirty generic roles, and documentary sources behind the sheets.

- **Three roles added** (27 → 30): Project insurance (`insurance`, under Project management & controls), Site & stakeholder engagement (`site-stakeholders`) and Supply & offtake (`supply-offtake`, both under Cross-cutting & interfaces). Catalogue, sector template and the five example profiles carry the three new headings.
- **Four "Senior level — the expert's eye" sections added** where they were missing: document control, financing & FID, interface manager, risk manager. The financing sheet now separates project finance from corporate (balance-sheet) financing.
- **"Sector-specific" pointer completed** in the five sheets that lacked it: contract manager, cost controller, geotechnical engineer, planner, procurement.
- **Correction — domino threshold.** The HSE and technical safety sheets gave 300 mbar as the domino-effect threshold of the French set they quote. The French order of 29 September 2005 has domino effects examined from 200 mbar overpressure and 8 kW/m² thermal; 300 mbar is the threshold of very severe structural damage. Both sheets corrected, values kept as a labelled example of the French set.
- **Points aligned with their source**: AACE 18R-97 accuracy shown as a range of ranges, the table values being typical points (estimator); FIDIC 2017 claim periods — 28 days for the Notice of Claim, both Parties, 84 days for the fully detailed Claim (42 in 1999), 14 days for the Engineer's notice of lateness (contract manager); EEMUA 191 4th edition, 2024 (DCS); Incoterms 2020 — eleven rules, risk passing at delivery, seller's insurance obligation under CIP and CIF only (procurement).
- **France country card**: a list of reference points checked at source on 13 November 2026 (appeal periods, environmental authorisation procedure, hazard-study effect thresholds, prevention plan and safety coordination, connection offer validity, geotechnical missions), to be re-checked at project date.
- **Documentary sources** under `references/sources/` (five files: project controls, engineering, safety & environment, delivery & operations, external sectors). Each fact carries its confirmation level: [V] was read in the document itself; the others were only located through a search engine and must be re-read at source before being quoted in a deliverable.

Stated plainly: the three new role sheets and the documentary sources are **unreviewed by practitioners**. They were written in one working session, not from field review as the original sheets were; treat them as drafts open to correction.

## [1.0.0] — 2026-09-11

First public edition.

- 27 generic role sheets (project management & controls, engineering, safety & environment, procurement-construction-quality-operations, cross-cutting), each with reading grid, indicative anchors, decision trees, red flags and a "Senior level" section.
- Three-layer architecture: generic roles × sector profile × countries. No sector shipped; fallback profile `generic` with express mini-profile; profile template with a density example.
- "Creating the specifics of a sector" protocol (framing by questions, writing, installation, keeping the profile alive) and sector-specific roles created on demand.
- Country layer, worldwide: nine-axis method, a map of technical standards regimes by discipline across 24 regimes (EU, UK, US, Canada, Australia/NZ, Gulf, India, China, Japan, Brazil, South Africa, international oil & gas, Norway, Switzerland, Turkey, Egypt, francophone and anglophone Africa, Singapore, Malaysia, Indonesia, South Korea, Mexico, Chile) so that every role adapts its codes once the project country is defined, five example country cards (FR · BE · PL · ES · DE), substance / permanent-establishment risk, country card template.
- Per-project configuration (`project-team.json`, `CLAUDE.md` block) and profile selection cascade (conversation > project > default > detection > generic).
- `examples/sample-answers.md`: three sample answers showing the layers in use.
- Repository furniture: banner, issue and pull-request templates, `SECURITY.md`, `VERSION`.
- Five example sector profiles under `examples/sectors/` (solar PV, hydrogen, refining & petrochemicals, thermal power, manufacturing plant), explicitly unreviewed, kept out of the shipped `references/sectors/`.
- `scripts/team.py` tool: `list`, `profile`, `check`, `init`, `new-sector`, `new-role [--sector-specific]`, `new-country`; `check` also verifies that no sector content enters the generic sheets.

Origin: generalisation of a biomethane project-team skill (28 roles, sheets reviewed one by one with practitioners), whose sector content was removed for this edition. The English wording of this first edition has not been proofread by a native speaker, and the regime map entries are reference points to be confirmed locally: both are open to correction.
