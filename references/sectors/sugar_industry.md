# Sugar industry

> Copy as `sectors/<slug>.md` (or `python scripts/team.py new-sector <slug>`, which pre-fills one `###` per role). The profile does not rewrite the role sheets: it states \\\\\\\\\\\\\\\*\\\\\\\\\\\\\\\*what changes\\\\\\\\\\\\\\\*\\\\\\\\\\\\\\\* for each role in this sector. An empty insert is better than an invented one — write "— nothing specific —" when the generic sheet is enough. Expected density of an insert, as an example (Cost controller, fictional sector "continuous production with offtake"):
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

* **Object**: This sector card is about the beet sugar industry. It includes beet reception, beet washing, slicing, extraction, juice purification, evaporation, crystallization, drying. It includes the final step in the service center consisting of storing the dried sugar, milling it (optional), bagging (from 1 kg over 10 to 25 kg bag, big bags and bulk) as well as specialties products. Thick Juice storage to expand sugar house operation is the usually way of increasing profits by increasing utilization. Most know how on cane sugar processing can be used as source for knowledge but never without clearly highlighting the source. Auxiliary operations such as boiler and turbine (steam and gas) operation and waste water treatment are also covered but considered utilities.
* **Typical scale**: processing capacity is from 5.000 t/d to 20.000, world scale outside northern Europe is up to about 35.000 t/d. tons per day is a common indicator for capacity, even on equipment level. Project scale is usually 0,5 up to 15 Mio. € or equivalent currencies for northern and east Europe.
* **Dominant contract models**: nearly all projects are multi-package projects managed by the owner's team. EPC contracts are very rare. Usually the highest risk lies in the interfaces for any project. As anywhere resources on owner's side are limited. Quite often projects are dominated by one single large equipment and small other packages. Electrical is most often done by owner, same for programming and field instrumentation.
* **Life cycle \& gates**: Project are driven by the maintenance and campaign periods. Skipping quality checks or pass project gates by default is not rare because of the common perception that speed is most important criterion due to the low operation time - generally not supported by project outcomes. Campaign usually starts in September and ends in January, but deviations are common.
* **Regulatory framework and permits**: regulatory differs a lot between projects, from projects without any demand to projects which only require an approval notice to formal approval applications depending on the local regulations. Sugar production generally is a food manufacturing process and has to follow hygienic rules.
* **Key external counterparts**: depends on location and project scope. Some sites are very close to neighbors or already have issues with smell. Network operators are not relevant except for specific projects (e.g. expansion of grid connection or biogas production)
* **FID locks / long poles**: campaign start in September, end in January. Approval of projects in September for the following year. Delay of campaign start due to delay of project execution is very expensive and therefore not an option. If in doubt, a start up without project should be investigated thoroughly as part of the project's design. Operation is driven by the beet quality which is out of any control due to their characteristic as crop. Beet quality differs by region, from year to year and during campaign from beginning to end and heavily depends on weather (before, during and after harvest) which requires a lot of flexibility. Breakdowns in the beginning and during campaign are common and require quick action.
* **Economics \& revenue**: remuneration mechanism (tariff, tender, PPA, industrial margin, service contract), dominant sensitivities.
* **Roles to activate / deactivate / rename**: select by project's scope
* **Phase skills and references available**: the user's skills that carry the substantive detail for this sector (if there are none, say so: the skill must not invent any).
* **Common units \& ratios**: Common public benchmarking figures rely on "% o.b." (percent on beet) or "% WS" (percent on white sugar (as product)). Volume flows of up to 2.000 m³/h water (beet washing) or up to >1.000 m³/h in evaporation are common. Heat transfer area in evaporation station ranges from few 1.000's m² up to >12.000 m³/h.Residence time is few to several hours from washing to final storage. Centrifuges have about 1,8 to 2,2 t/filling and >20 cycles per hour. Sugar silos range from few 100 m³ for specialties up 80.000 t.
* **Key vocabulary**: WV - white value, DS - dry substance, purity (ratio of sucrose to overall solids), footing, A- B- and C-sugar, % o.b. - percent on beet, TJ thick juice, SC - service center (handling of sugar as powder, dust, crystal), fugal - centrifugal, centrifuge

## Sector-specific roles

## Role inserts

One `###` per role, **with exactly the short title from the catalogue in `SKILL.md`** (that is the matching key; a subtitle after " — " is free). Each insert: 3 to 10 bullets on what the sector changes — structuring cost items, long-lead items, dominant hazards, references, milestones, red flags, senior eye. Refer to the sector's skills rather than copying their thresholds.

### Piping engineer

File: `references/roles/piping\\\\\\\_engineer.md`

**Anchor figures**

* **campaign operation**: operation is about September to January, reliability is key
* **velocity**: liquids for water, condensate and raw juice 3 to 4 m/s, thin and thick juice 1,5 m/s, magma and slurries 0,2 m/s to prevent crystal damage, de-dusting and air minimum 18 m/s, preferred >20 m/s to prevent dust accumulation in pipes to prevent explosion risks, vapor (<3 barg) about 20 to 40 m/s, vapor (< \~1 bar abs) <10 m/s
* **fluid category** (PED): usually there is no fluid category 1 fluids (in the relevant diameter / pressure range) from the PED, eventually though for potential edge cases

**Red flags**

* **condensate pots**: local low points accumulation  which cannot be drained
* **slurry, magma, liquid lines with sugar crystals without slope >3%**
* **dew point:** biogas lines (H2S), compressed air especially as working air because not dried
* **valves without insulation**: propose other solutions e.g. insulation mattresses or jackets for quick dismounting. Do not accept uninsulated parts where temperature is above 50°C

### HSE (Health, Safety, Environment)

File: `references/roles/hse.md`

**Anchor figures**

* fine dust <250 µm usually present
* circumferential speed in screws and conveyors >1 m/s -> increased ATEX risk
* belt speed >1 m/s -> ATEX risk
* < \~1 mm layers of dust -> ATEX risk
* dedusting >18 m/s, better >20 m/s
* >4 % of <20 µm are enough to create a combustible mixture

**references**

* **Leitfaden zur Vermeidung von Staubexplosionen bei der Gewinnung und Verarbeitung von Zucker** 03/2021 published by  Berufsgenossenschaft Rohstoffe und chemische Industrie der DGUV

**senior eye**

* **blocking by sugar lumps (dry) or clumps in slurry lines** - will that valve operate under any condition if required to?
* **Strecker Degradation**: long residence times (dead legs, bypass, low flow zones), high temperature (process heating, trace heating, hot water or steam to solve blockings), blocked volumes, presence of amino acids, presence of invert sugar, risk of color formation
* **factories and equipments are often old** and moved between factories / countries several times, often there is a lack of documentation and reliability of documentation
* **PID are often very complex,** reliability and validity are to be questioned

### Technical safety (process safety engineering)

File: `references/roles/technical\\\_safety.md`

**Paragraph F\&G mapping \& fire protection is usually not relevant,** special cases might deviate

**dominant hazards:**

* **safety valves often to surrounding environment** -> blow down area
* **in service center: explosion venting** to outside of the building -> protect blow down area
* Lots of equipmens only are designed for **atmospherical pressure** but require regular cleaning with steam with eventually critical **pressure** and blockings are often removed with **pressurized hot water or steam** (Strecker Degradation)

**senior eye**

* supports a **reliable operation** with using knowledge on failure frequencies
* **ensure mutual understanding of terms, use traceable terms** from norms (e.g. as defined by Art. 2 PED PS (8) and TS (9))
* **always mark pressure indications** as absolute (a or abs) or overpressure (g, regional terms from the country profile), only differential pressure holds a pressure unit without such

### Procurement

File: `references/roles/procurement.md`

**Red flags - the hunt**

* **Food contact material not mentioned / specified** material needs to be specified in RFQ including certifications required

### Quality

File: `references/roles/quality.md`

**Red flags - the hunt**

* **Material spec included** - even in food mild steel is acceptable, IF a risk assessement is done, material needs to be specified in RFQ

**Standards / references**

* **Food contact material (all materials):** 1935/2004/EC and 2023/2006/EC
* **Food contact material (plastics):** 2011/10/EU
* exclude: API standards

## Cross-cutting red flags of the sector

* Long lead items not ordered until christmas will most certainly give delivery dates which leave no room for mistakes to start up campaign in September
* lack of detailed construction schedules for constraint spaces with several vendors leads to clashes (time and space)
* lack of as-built documentation and plausibility check on site before start of design will probably lead to troubles when design becomes construction

