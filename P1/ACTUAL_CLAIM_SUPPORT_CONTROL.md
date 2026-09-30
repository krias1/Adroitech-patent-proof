# Actual Claim Support Control

**Control date:** 2026-09-30

## Purpose

This file prevents the obsolete `CLAIM-A` through `CLAIM-F` rows in `P1_SUPPORT_MATRIX.csv` from being mistaken for the operative nonprovisional claim set.

The operative candidate claim-control surface is `P1/NONPROVISIONAL_CLAIM_READINESS.csv`, which now contains claims 1-20. Until `P1_SUPPORT_MATRIX.csv` is migrated to limitation-level rows for those claims, its `CLAIM-A` through `CLAIM-F` rows are **QUARANTINED / NON-OPERATIVE** and must not be used to close written-description, enablement, priority, figure-support, novelty, obviousness, or filing-readiness gates.

This control does not promote any claim to READY and does not infer P1 support from historical evidence. Frozen-P1 support must be established from the exact filed P1 specification/drawings.

## Operative candidate claims

| Claim | Working title | Dependency | Support-control status |
|---|---|---|---|
| 1 | Integrated runtime resolution | independent | limitation-level P1 mapping required |
| 2 | Provenance evidence correction freshness permission filtering | claim 1 | limitation-level P1 mapping required |
| 3 | Inference-resource budget | claim 1 | limitation-level P1 mapping required |
| 4 | Event lifecycle relevance | claim 1 | limitation-level P1 mapping required |
| 5 | Correction supersession and preserved provenance | claim 1 | limitation-level P1 mapping required |
| 6 | Model-independent durable reconstruction | claim 1 | limitation-level P1 mapping required |
| 7 | Physical identifier namespace resolution and write-back | claim 1 | exact-filed-page verification required |
| 8 | Offline capture and authoritative reconciliation | claim 7 | exact-filed-page verification required |
| 9 | Workstream continuity under Person State change | independent | mutable checkpoint/resume-state P1 mapping required; no static resume-point invariance |
| 10 | Person State fields and field-specific freshness | claim 9 | limitation-level P1 mapping required |
| 11 | Newer evidence correction or supersession before resume | claim 9 | limitation-level P1 mapping required |
| 12 | Do-not-repeat state | claim 9 | limitation-level P1 mapping required |
| 13 | Mobile or voice feasibility transition | claim 9 | limitation-level P1 mapping required |
| 14 | Bounded resume package | claim 9 | exact resume-point and permission-information boundaries require mapping |
| 15 | Provider-independent handoff | independent | limitation-level P1 mapping required |
| 16 | Different provider or local-cloud runtime transfer | claim 15 | limitation-level P1 mapping required |
| 17 | Handoff correction provenance permission evidence do-not-repeat | claim 15 | each alternative requires individual support verification |
| 18 | Permission-scoped reduced handoff | claim 15 | limitation-level P1 mapping required |
| 19 | Replacement endpoint restore | claim 15 | exact-filed-page verification required |
| 20 | Post-reconstruction durable write-back | claim 15 | limitation-level P1 mapping required |

## Migration rule

The next support-matrix revision must replace the six illustrative claim rows with the actual 20-claim set and then decompose each claim into limitation-level support rows. Each limitation row must identify, at minimum:

- exact frozen-P1 specification coordinate(s);
- exact frozen-P1 figure(s), where applicable;
- written-description status;
- enablement status;
- priority status;
- any later-matter exclusion;
- linked pre-P1 provenance evidence only as corroboration, never as a substitute for P1 disclosure;
- unresolved ambiguity or support gap.

No claim may be marked P1-supported merely because the same concept appears in pre-filing Git history. The frozen filed P1 remains the priority-support boundary.

## Claim 9 architecture control

For Claim 9 and its dependents, preserve the distinction between **persistent workstream identity** and **mutable checkpoint/resume state**. The earlier static resume-point-invariance formulation is not operative. Any stronger authority/priority reconciliation mechanism must be separately mapped to the frozen P1 before receiving the 2026-09-16 priority date; otherwise it is later matter.

## Readiness effect

This control removes an examiner/reviewer ambiguity in the proof surface, but it does **not** close the P1-support gate. Overall filing status remains `NOT_READY` until the operative claims receive limitation-level frozen-P1 mapping and the other filing-critical gates close.
