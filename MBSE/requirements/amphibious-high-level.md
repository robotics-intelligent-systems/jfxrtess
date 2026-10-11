# Amphibious concept requirements and traceability

Review: 2026-10-10. Source repository baseline: `74df5ba75c6cb1b90dc581ba9a2feb848edf0a3d`.

The three CAD-directory assets are concept JPEGs, not dimensioned CAD or measured prototypes. They establish visual intent for AM-S (roadster), AM-U6 (utility vehicle) and AM-B (motorcycle). No geometry, speed, load capacity, electrical architecture or real-time deadline is inferred from pixels. Requirements below are proposals awaiting owner-approved parameter baselines and verification.

The existing car diagram's autonomy, hydrofoils, wheel retraction, combustion-drive choice, <2 s switching, <10 ms rendering/real-time bound, <1 ms controller, Java 17 and IP68 assertions are superseded by explicit decisions D01–D12. The named STEP files and parser directory in that diagram do not exist in this baseline and are no longer shown as available assets. AM-B's original AM-01–AM-16, P01–P18 and V01–V16 identifiers are retained; its electric-drive and numerical timing/telemetry proposals remain provisional, not family-wide specifications.

## CAD sources

| Variant | Source asset | Git blob | Interpretation |
|---|---|---|---|
| AM-S | [amphibious-sport-roadster.jpg](../CAD/amphibious-sport-roadster.jpg) | `bacdc5130772ae916d46ab5625f61b2b49701873` | Visual design intent only; dimensions and physical verification absent. |
| AM-U6 | [deeper-vehicle-immersion-in water-mode.jpg](../CAD/deeper-vehicle-immersion-in%20water-mode.jpg) | `f0585fc25a9e59fd6bb3803453cdba7cd0afa8c9` | Visual design intent only; dimensions and physical verification absent. |
| AM-B | [amphibious-motorcycle-concept.jpg](../CAD/amphibious-motorcycle-concept.jpg) | `76f4d432fb1597ee936cccc1c2860456522b484b` | Visual design intent only; dimensions and physical verification absent. |

## Proposed high-level requirements

[Machine-readable traceability](amphibious-traceability.csv) includes acceptance criteria, owners, verification methods and AM-B links. All verdicts are **not executed**. RT IDs are shared; S/U6/B IDs are variant-specific.

| ID | Requirement | Owner | Verification | Acceptance |
|---|---|---|---|---|
| RT-01 | The project shall identify concept variant, source hash, geometry, mass and CG baseline for each accepted load case. | CAD / configuration | Inspection | Every model and run resolves to the same approved variant, source and load baseline. |
| RT-02 | Each variant shall demonstrate operator-controlled steering, traction and braking within its approved land envelope. | Vehicle dynamics | Analysis + controlled test | Stopping distance, grade and handling meet approved load/surface/speed criteria; values remain TBD. |
| RT-03 | Each hull shall meet approved loaded freeboard, stability and defined flooded-condition criteria. | Naval / mechanical | Hydrostatic analysis + supervised test | Measured mass/CG and geometry satisfy approved heel, trim, reserve buoyancy and flooding criteria. |
| RT-04 | Marine propulsion shall be enabled only within its validated immersion and actuator-availability envelope. | Marine / controls | MIL + bench + supervised test | Invalid, stale or contradictory immersion evidence invokes the approved inhibit/limit policy. |
| RT-05 | A local supervisor shall authorize LAND, TRANSITION and WATER using operator intent and validated guards. | Controls | MIL / SIL / controller-HIL | Allowed transitions are covered; ambiguous guards, timeout and bounded drive overlap follow the approved policy. |
| RT-06 | The design shall define energy isolation, thermal limits, ingress monitoring and charge/service propulsion interlocks. | Electrical | Inspection + bench fault injection | Approved electrical/thermal/ingress profiles and charge/service inhibits pass; ratings and thresholds remain TBD. |
| RT-07 | The supervisor shall meet allocated execution deadlines and mode-specific hazard-derived fault-response times. | Embedded / safety | SIL / target controller-HIL | Timing and fault traces meet the approved load profile and response budgets; no deadline claimed from tool choice. |
| RT-08 | Essential control and fault handling shall remain local during loss of engineering, cloud or telemetry connections. | Embedded / integration | Disconnect and permission test | Local operation follows approved loss policy; remote analytics, UI and AI cannot publish actuator commands. |
| RT-09 | Land and water models shall share configuration, SI units, frames and a declared clock/solver owner for each coupled state. | Simulation | Interface test + model comparison | No duplicate state integration; handover, unit/frame and validity-domain checks meet approved error budgets. |
| RT-10 | Test records shall preserve timestamps, validity, source versions, configuration and requirement/test references. | Data / verification | Schema + replay + audit | Mandatory fields and approved rate/buffer profiles pass; stale/reordered data are flagged and no verdict lacks evidence. |
| RT-11 | Each variant shall define service isolation, hull/drivetrain access, drainage and post-service integrity checks. | Service / mechanical | Inspection + demonstration | Required service tasks and integrity checks are demonstrated against an approved procedure. |
| RT-12 | Each stage shall close critical design decisions and approve operating envelope, configuration and verification dispositions. | Systems engineering | Review | No stage-critical TBD or failed criterion remains without an accepted disposition; no physical verification inferred from an image. |
| S-01 | The AM-S baseline shall define occupant/restraint space and enclosure/hull packaging from a dimensioned design. | AM-S / mechanical | CAD inspection | Occupancy, access, clearances and loaded geometry are approved; image appearances are not measurements. |
| S-02 | AM-S shall document separate land/marine drive allocation and transition clearances for its selected configuration. | AM-S / controls | Analysis + MIL | Approved drive allocation and hull openings are traceable; retraction, hydrofoils and autonomy are not assumed. |
| U6-01 | AM-U6 shall define secured cargo and occupant load cases and their effect on mass, CG and waterline. | AM-U6 / mechanical | CAD + hydrostatic analysis | Every approved cargo case satisfies restraint and stability criteria; payload capacity remains TBD. |
| U6-02 | AM-U6 shall define six-wheel steering, braking, traction and load-sharing for the selected running-gear proposal. | AM-U6 / vehicle dynamics | Analysis + MIL | Wheel/axle loads and control behavior satisfy approved land cases; wheel count is concept intent, dimensions remain TBD. |
| B-01 | AM-B shall define rider posture, low-speed land balance and rider/vehicle stability through land-water transition. | AM-B / vehicle dynamics | Analysis + controlled test | Rider-load and balance criteria are approved and verified for each relevant mode. |
| B-02 | AM-B shall define rider exposure, immersion-sensitive components and service access for the selected hull/propulsor design. | AM-B / mechanical | Inspection + ingress/immersion test | Wet-volume, isolation and service criteria pass for the approved configuration; image does not establish a rating. |

## Decision register

All entries are OPEN until value, rationale, owner, revision and acceptance method are approved. TBD values block affected tests/releases. Dependency priorities P0–P3 are separate from AM-B proposed target status.

| ID | Decision | Owner | Trace | Required closure |
|---|---|---|---|---|
| D01 | Mission, operator and autonomy scope | Systems | RT-12 | Operator-controlled study baseline; autonomy requires separate scope. |
| D02 | Occupancy and cargo allowance | Mechanical | RT-01,S-01,U6-01,B-01 | TBD persons/kg/distribution; AM-B single-rider baseline is provisional. |
| D03 | Dimensions, mass and CG | CAD | RT-01,RT-03 | TBD m/kg and CG by load case; create actual CAD. |
| D04 | Land envelope | Dynamics | RT-02 | TBD speed/grade/surface/braking distance. |
| D05 | Water envelope and stability | Naval | RT-03,RT-04 | TBD wind/waves/current/depth/freeboard/heel/trim. |
| D06 | Drive architecture and transitions | Controls | RT-04,RT-05,S-02,U6-02 | TBD power, drive overlap, immersion guards; no assumed retraction. |
| D07 | Energy, isolation and ingress | Electrical | RT-06 | TBD power/voltage/energy, enclosure profile and isolation limits. |
| D08 | Deadlines and fault response | Embedded / safety | RT-07 | TBD by task/hazard. AM-B 20 ms is an existing review target only. |
| D09 | Model coupling and fidelity | Simulation | RT-09 | TBD FMI profile, step size, frames and per-variable error budgets. |
| D10 | Telemetry and offline retention | Data | RT-10 | TBD by stream. AM-B 5 Hz / 30 min are existing review targets only. |
| D11 | Service and environment | Service | RT-11 | TBD corrosion, temperatures, inspection and integrity procedures. |
| D12 | Release evidence and applicable approval scope | Systems | RT-12 | TBD stage owners and approvals; no certification inferred. |

## Interface baseline

| ID | Interface | Proposed contract |
|---|---|---|
| I-01 | Operator → local supervisor | Validated mode intent, brake/enable state and explicit acknowledgement; no cloud dependency. |
| I-02 | Sensors → supervisor | SI units, coordinate frame, timestamp, validity/age, calibration and diagnostic state; implausible/stale guards invoke policy. |
| I-03 | Supervisor → drive adapters | Mode-scoped enable/limit commands with local interlocks and approved deadline/fault policy. |
| I-04 | Model ↔ co-simulation runner | Configuration digest, FMI version/profile, step ownership, units/frames, state handover and capability validation. |
| I-05 | Controller bench ↔ real-time plant | Pinned I/O mapping, clock/load configuration, latency/jitter capture and safe bench limits. |
| I-06 | Telemetry → registry/analytics | Read-only selected-state projections, source versions and ordered evidence; no actuator authority. |

## Verification and delivery

G0 fixes scope, CAD/load decisions and acceptance thresholds. G1 verifies a reproducible MIL plant/controller slice. G2 compares production software in SIL. G3 evaluates controller-HIL timing, I/O and fault handling on an isolated bench. G4 permits qualified, controlled physical trials only within the accepted envelope. Controller-HIL (CHIL) is a HIL configuration, not a separate level with automatically stronger evidence.

Each run links requirement ID → parameter/interface baseline → CAD/model/firmware revisions → test procedure → inputs/results → verdict → reviewer/disposition. MIL/CFD output does not establish flotation or physical safety. CFD-derived coefficients need a validity domain and calibration; a separate reduced model must meet the real-time deadline before a HIL claim.

## Editable diagrams

- [AM-S / AM-U6 family requirements](../CAS/jfxrtess-amphibian-car-cad-architecture.drawio): six pages covering CAD context, shared requirements, variant allocation, interfaces, verification and open decisions.
- [AM-B requirements](../CAS/OpenTwin_AM-B_Requirements_Engineering.drawio): original six pages preserved and revised, plus family/dependency crosswalk.

The drawings are native mxGraph cells with uncompressed XML, not flattened screenshots. Diagram exports and source validation do not constitute engineering-test results.

[Project architecture and dependency priorities](../../README.md)
