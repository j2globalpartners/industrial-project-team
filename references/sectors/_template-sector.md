# Sector profile — <Sector name> (template)

> Copy as `sectors/<slug>.md` (or `python scripts/team.py new-sector <slug>`, which pre-fills one `###` per role). The profile does not rewrite the role sheets: it states **what changes** for each role in this sector. An empty insert is better than an invented one — write "— nothing specific —" when the generic sheet is enough. Expected density of an insert, as an example (Cost controller, fictional sector "continuous production with offtake"):
>
> ```
> ### Cost controller
> - Structuring cost items: licensed process core (35–45% of CAPEX, indicative), utilities, HV grid connection.
> - Long-lead items to commit before FID: main reactor, compressors — their payment schedule drives the cash curve.
> - Contingency: consumed first by tie-ins and piping rework, rarely by the licensed core.
> - Red flag (sector): VOWD of the licensed package reported pro rata to payments, not to physical progress.
> - Senior eye (sector): an EAC that does not move during erection hides an overdue change-order review.
> ```

## Sector identity card

Twelve lines; this is what the skill reads first to calibrate itself.

- **Object**: what the installation produces or transforms, and its usual variants.
- **Typical scale**: capacity (MW, t/yr, Nm³/h…), CAPEX (order of magnitude), development → commissioning duration, team size.
- **Dominant contract models**: lump-sum EPC / EPCM / multi-package / BOT / process licence / supply + erection; non-EPC contracts that carry the economics (offtake, PPA, feedstock supply, O&M).
- **Life cycle & gates**: the sequence of phases and decision milestones specific to the sector, with the estimate classes alongside.
- **Regulatory framework and permits**: categories, regimes, building permit, major-hazard and pressure / hazardous-area rules — *what drives the calendar* — stated by regime family, the country deciding the actual set (`countries/standards-regimes.md`); fill in "Country × sector notes" per country of operation.
- **Key external counterparts**: network operators, authorities, offtakers, licensors, financiers, neighbours.
- **FID locks / long poles**: the 2 to 4 subjects outside the project's control that condition the decision and the date.
- **Economics & revenue**: remuneration mechanism (tariff, tender, PPA, industrial margin, service contract), dominant sensitivities.
- **Roles to activate / deactivate / rename**: sector-specific roles (defined below or in `roles/`), generic roles without object here, roles whose title changes (e.g. DCS → SCADA).
- **Phase skills and references available**: the user's skills that carry the substantive detail for this sector (if there are none, say so: the skill must not invent any).
- **Common units & ratios**: the quantities the team handles and 5 to 10 indicative orders of magnitude.
- **Key vocabulary**: 15 to 30 terms.

## Sector-specific roles

### <Specific role>
Compact sheet (10 to 20 lines) or reference to a full sheet in `roles/`: **Mission** · **Reading grid** (in order) · **Anchor figures** (indicative) · **Red flags** · **Senior eye**.

## Role inserts

One `###` per role, **with exactly the short title from the catalogue in `SKILL.md`** (that is the matching key; a subtitle after " — " is free). Each insert: 3 to 10 bullets on what the sector changes — structuring cost items, long-lead items, dominant hazards, references, milestones, red flags, senior eye. Refer to the sector's skills rather than copying their thresholds.

### Project manager
### Estimator
### Cost controller
### Planner
### Contract manager
### Risk manager
### Financing & FID
### Project insurance
### Process engineer
### Mechanical engineer
### Materials & corrosion engineer
### Piping engineer
### Civil / structural engineer
### Geotechnical engineer
### Electrical engineer
### Instrumentation engineer
### DCS / control systems engineer
### HSE
### Technical safety
### Environment & permitting
### Procurement
### Construction manager
### Quality (QA/QC)
### Commissioning
### O&M (operations & maintenance)
### Grid & utility connection
### Interface manager
### Document control
### Site & stakeholder engagement
### Supply & offtake

## Country × sector notes (optional)

Per country of operation: support mechanism, permit categories / regime specific to the sector, product specifications of the network operator or offtaker, market particularities. What depends only on the country stays in `countries/country-cards.md`.

## Cross-cutting red flags of the sector

- 5 to 8 signals that, in this sector, almost always announce a project in trouble.
