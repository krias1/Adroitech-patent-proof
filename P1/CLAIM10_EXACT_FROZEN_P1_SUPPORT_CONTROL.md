# Claim 10 Exact Frozen-P1 Support Control

**Control date:** 2026-10-01
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16
**Exact specification:** `ADROITECH_PERSON_SPECIFIC_AI_RUNTIME_PROVISIONAL_SPECIFICATION_2026-09-16.pdf`
**Exact specification SHA-256:** `267628a51cc938dbcbd724af4f7f9b0a1ad58532f32b738b12a36490c2cff00e`
**Exact specification byte length:** `35,893`

## Operative Claim 10

Claim 10 depends from Claim 9 and recites that Person State comprises at least one of interface type, endpoint identity, input modality, movement state, network state, available tools, resource constraints, physical constraints, or an intended transition, and that at least one Person State field has a freshness rule different from a durable world-state field.

## Exact frozen-P1 support

The frozen filing defines Person State as a current or time-bounded representation of operational circumstances including interface, device, location when authorized, time, movement, available tools, network reachability, input modality, physical constraints, resource constraints, intended transition, and freshness/confidence metadata.

Detailed Description §5 provides an example `PersonStateSnapshot` containing `interface_type`, `endpoint_id`, `input_modality`, `movement_state`, `network_state`, `available_tools[]`, `resource_constraints[]`, `physical_constraints[]`, `intended_transition`, confidence, and `field_freshness{}`.

Section 5 further states that different Person State fields may have different staleness behavior and gives concrete examples: exact location may expire within minutes; interface identity may expire when a session changes; a business role may persist until explicit change. It identifies absolute expirations, decay functions, freshness classes, source-specific refresh rules, or combinations thereof as implementations.

The Background independently contrasts a durable fact such as operating a business with current location, stating that the two should not expire at the same rate. This supplies the durable-world-state comparison recited by Claim 10 rather than merely establishing different freshness among Person State fields.

FIGS. 4-5 are candidate corroborating drawings and remain subject to frozen-drawing visual QA; textual support is direct and does not depend on those drawings.

## Limitation disposition

| Limitation | Frozen-P1 coordinate | Disposition |
|---|---|---|
| Person State field alternatives | Definitions; DD §5 | DIRECT |
| field-level freshness metadata/rules | Definitions; DD §5 | DIRECT |
| different staleness behavior among fields | DD §5 | DIRECT |
| Person State freshness differs from durable world-state field | Background plus DD §§4-5 | DIRECT |

## Breadth controls

1. `endpoint identity` is controlled to the filed device/endpoint identity concepts; it does not imply an undisclosed hardware-rooted identity mechanism.
2. `freshness rule` includes the filed expiration, decay, freshness-class, and source-specific refresh mechanisms; no particular mathematical decay function is required unless separately supported.
3. The durable-world-state comparison is lifecycle/staleness differentiation. Claim 10 does not require every durable field to be permanent or every Person State field to expire rapidly.
4. Later ethical-runtime or implementation documents may corroborate development history but do not expand the P1 priority boundary.

## Readiness effect

Claim 10 is controlled for frozen-P1 §112(a) written-description and priority support. This does not close enablement, §101, §102/§103, §112(b)/(f), inventorship, best mode, material-information/public-disclosure, drawing, or final filing-artifact QA gates.
