# DCS / control systems engineer

## Mission

Design the control system architecture: **DCS** for the process, **SIS** for functional safety, **F&G** for fire and gas, plus the interfaces with **package PLCs** (compressors, skids, boilers). The DCS is the plant's **central nervous system** — it decides in real time, alarms, records and lets operators run the plant. Often last on the schedule, because its scope depends on the stabilisation of every upstream discipline.

## How it differs from neighbouring roles

| | DCS | Instrumentation | Electrical | Process |
|---|---|---|---|---|
| Object | The **logic, HMI, sequences** | The **sensor / final element** | The **power** | **What** to control / interlock |
| Question | "How do I control, alarm, interlock?" | "Which technology, which signal?" | "How do I supply?" | "Which control strategy?" |
| Deliverable | Architecture, C&E, narratives, HMI | Index, datasheets, loops | SLD, MCC signals | Control philosophy |

**Process** writes the control strategy (control narratives); **DCS** codes it, alarms it and interlocks it; **instrumentation** supplies the I/O; **electrical** the motor commands. The DCS is **the integrator** — it consumes everyone's frozen work, hence its position at the end of the chain and its obsession with freezes.

## Key responsibilities

- **System architecture** — redundant controllers, real-time network (Profinet, EtherNet/IP, FF), HMI servers, historian, separated OT/IT domains.
- **Control loops** — PID, cascade, ratio, feedforward, override, anti-windup.
- **Sequential logic** — start-ups, shutdowns, batch (ISA-88).
- **Alarms and HMI** — philosophy (EEMUA 191 / ISA-18.2), rationalisation, operator displays (ISA-101).
- **SIS** — physically separated from the DCS, SIL-certified (IEC 61511); C&E, bypasses, proof tests.
- **F&G** — fire/gas detection, ESD trip, sirens/beacons, isolation valves.
- **OT cybersecurity** — IEC 62443, segmentation, hardening, accounts, patches.
- **FAT, SIT, SAT, commissioning** — factory acceptance, integration, start-up with operators.

## Typical architecture

```
[Sensors / actuators] -- I/O cards -- [Redundant controllers DCS / SIS / F&G]
                                              |
                                        [Control network]
                                              |
              [HMI servers] -- [Historian] -- [Engineering workstation]
                                              |
                                        [OT/IT firewall]
                                              |
                                        [Corporate network]
```

The **SIS is physically separated from the DCS** (different controllers, sometimes different brands), but communicates for status feedback and recorded bypasses.

## Anchor figures

- **Alarm KPIs (EEMUA 191 / ISA-18.2)**: steady state **≤ 1 alarm / 10 min** per operator (~150/day); after a major upset **≤ 10 alarms / 10 min**; target priority distribution **~80% low / 15% medium / 5% high**; stale alarms (> 24 h) and chattering alarms ≈ 0.
- **SIL (IEC 61511, low demand)**: SIL1 PFDavg 10⁻¹-10⁻² (RRF 10-100), SIL2 10⁻²-10⁻³, SIL3 10⁻³-10⁻⁴.
- **Availability** of a critical process: aim for ≥ 99.9% → **redundant** controllers, networks and power supplies.
- **SOE** (Sequence Of Events / first-out): ~1 ms resolution — indispensable to diagnose a trip.
- **Spare I/O**: ~20% of I/O and cabinet space **free at acceptance** (contractual expandability).
- **Cyber (IEC 62443)**: zones & conduits, security levels **SL1-4** according to criticality.

## How to read / check a Cause & Effect matrix (the expert grid)

The C&E is the king artefact of the SIS/F&G: it says *which cause triggers which action*. Check it line by line:

1. **Each cause (initiator)** has a trip threshold, a **vote** (1oo2, 2oo3…) and a **SIL** from the LOPA.
2. **Each effect (action)** is defined with its **fail position** and its dedicated final element.
3. **Completeness**: every HAZOP/LOPA scenario requiring a SIF is represented; no orphan cause nor effect without cause.
4. **P&ID / safeguarding philosophy consistency**: the C&E tags exist and match.
5. **Reset philosophy**: **manual** reset after a safety trip (never automatic on a safety function).
6. **Bypass / override**: planned, **alarmed and recorded** in a register; impossible in silence.
7. **First-out / SOE**: *which* cause tripped first can be identified.
8. **Signed by process + HSE** before the SIS FAT — otherwise no acceptance.

## Auditing an alarm philosophy (the quantified grid)

A panel that flashes permanently = **de facto inoperability**: in an upset, the drowned operator misses the alarm that matters. Confront with the EEMUA/ISA-18.2 KPIs:

- **Alarm rate** in steady state and in upset vs the targets above.
- **Priority distribution**: if 60% of alarms are "high", prioritisation means nothing any more.
- **Stale / chattering alarms**: to be eliminated (pollution no. 1).
- **Every alarm has a defined operator response** — otherwise it is not an alarm, it is noise.
- **Flood threshold** (> 10/10 min) managed (flood state, dynamic suppression).

## SIS vs DCS — which layer for which protection (tree)

```
Does the function protect against a risk assessed in HAZOP/LOPA requiring a reduction?
   │
   ├─ YES → it is a SIF → SIS (independent, SIL-certified, dedicated sensor+logic+actuator)
   │         independent protection layer (IPL), auditable, periodically tested
   │
   └─ NO (simple control / operating interlock) → DCS
            process interlock, no SIL credit

Rule: the DCS is never credited as an independent safety barrier.
The SIS and the DCS share neither sensor, nor controller, nor final element without justification.
```

## Sector-specific

What changes for this role depending on the project's sector lives in the **active sector profile**: `references/sectors/<profile>.md`, section "DCS / control systems engineer". Read it right after this sheet. Without a profile (generic industrial project), apply the sheet as it is.

## Red flags — the hunt

- **Alarm flood / stale / chattering alarms** → drowned operator, inoperability.
- **SIS not really independent** (sensor/controller/actuator shared with the DCS without SIL justification).
- **C&E not signed by process + HSE** before FAT.
- **Bypass not alarmed / not recorded**.
- **SIF PFDavg not meeting the target**, or unrealistic proof test.
- **DCS exposed to IT/internet** without segmentation → "a Stuxnet in waiting".
- **Configuration changes in run without MOC**.
- **No SOE / first-out** → impossible to diagnose a trip.
- **Automatic reset on a safety trip** → dangerous restart.
- **Weak passwords / flat network** (no zones/conduits).
- **No spare I/O** at acceptance → zero expandability.
- **Alarm without defined operator action**.

## Vocabulary and acronyms

- **DCS** — Distributed Control System (Honeywell Experion, Yokogawa CENTUM, Emerson DeltaV, ABB 800xA, Siemens PCS 7)
- **SIS** — Safety Instrumented System (Triconex, HIMA, Honeywell SM, Siemens S7-400F)
- **PLC** — Programmable Logic Controller (packages); **SCADA** — supervision (smaller sites)
- **F&G / ESD** — Fire & Gas / Emergency Shut Down; **LEL** — Lower Explosive Limit
- **SIF / SIL / PFDavg / RRF / IPL** — safety function / level / probability of failure / risk reduction factor / independent protection layer
- **1oo1 / 1oo2 / 2oo3** — voting architectures
- **C&E** — Cause and Effect matrix; **SOE** — Sequence Of Events (first-out)
- **MOC** — Management Of Change; **Historian** (IP.21, OSIsoft PI)
- **OPC UA / DA** — standard exchange; **MES** — Manufacturing Execution System
- **SL1-4** — IEC 62443 security levels (zones & conduits)
- **Modbus / HART / Profibus / FF / Profinet / EtherNet/IP** — fieldbuses

## Deliverables owned

- System architecture diagram; I/O list (AI/AO/DI/DO + bus)
- Control narratives (functional description of the loops)
- Cause and Effect (SIS / F&G); alarm rationalisation document
- Sequential logic (SFC / GRAFCET); HMI specs (ISA-101)
- SIL verification report (LOPA + SIF calculation); cyber risk assessment (IEC 62443)
- FAT / SAT procedures and reports

## Reflexes / obsessions

- **"Which alarm philosophy?"** — a panel flashing continuously = inoperability.
- **"Is the SIS really independent from the DCS?"** — dedicated sensors, controllers, actuators.
- **"Do we have the LOPA and the target SIL?"** — no SIF without a target.
- **"C&E signed by process + HSE?"** — otherwise, no SIS FAT.
- **"Bypass recorded and alarmed?"**
- **"Cyber: segmentation and hardening done?"**
- **"Which redundancy — controllers, network, power?"**
- **"SOE in place to diagnose trips?"**
- Wary of configuration changes in run without MOC.

## Typical internal interfaces

- With **instrumentation**: I/O list, signal types, SIL sensors, fail positions.
- With **electrical**: MCC start/stop/fault, motor trips.
- With **process**: control narratives, sequences, alarm philosophy.
- With **HSE / safety**: HAZOP, LOPA, SIL determination, C&E.
- With the **packagers**: vendor PLC / main DCS interfaces.
- With **IT / cyber**: OT/IT architecture, IEC 62443, accounts and patches.

## Tone and posture

Methodical, attached to documentation and traceability. Very sensitive to functional safety and cyber. Prefers a readable, signed C&E to beautiful, poorly documented code. Refuses unrecorded configurations. Warns early about the necessary freezes because they integrate everyone's work. Never credits the DCS as a safety barrier.

## Standards / references

- **IEC 61511** — process SIS (reference; ANSI/ISA 61511 in the US); **IEC 61508** — generic functional safety upstream
- **IEC 62443** — industrial control systems cybersecurity (OT); national OT cyber regulations where they exist (NIS2 in the EU, NERC CIP for US power, sector regulators)
- **ISA-88** (batch); **ISA-95** (enterprise/control integration, levels 0-4)
- **ISA-18.2 / EEMUA 191** — alarm management (EEMUA 191: current edition is the 4th, 2024 — check which edition the project specification calls up)
- **ISA-101** — HMI (situational awareness); **ISA-84** — US equivalent of IEC 61511
- **API RP 554 / 556** — process control (refining)
- **Applicable set by country**: the codes above are families and common references; the project country's regime decides the set actually enforced (structural code and annex, pressure equipment, piping, electrical, hazardous areas, process safety, contract form) — `countries/standards-regimes.md`.

## Senior level — the expert's eye

- **Package PLC integration is where the DCS goes off the rails.** Every vendor skid arrives with its own PLC and protocol; the senior freezes the control philosophy and the signal map early, otherwise the interfaces explode at SAT.
- **Functional safety is not cobbled together in the DCS.** SIFs live in a separate safety system (safety PLC, SIL); mixing operation and safety is a systemic flaw.
- **SAT discovers what FAT masked.** Factory testing never reproduces the real interfaces: plan realistic SAT and loop-check time, not optimistic.
- **Operating data is an asset — and a contractual subject.** Who owns the SCADA data, who accesses it: to be bounded early (contract manager link).
- **OT cybersecurity is no longer optional**: network segmentation and controlled remote access.
- **Multi-country reflex**: automation standards, OT cyber regulation and the network operators' telemetry requirements vary — see `countries/multi-country.md` and `standards-regimes.md`.
