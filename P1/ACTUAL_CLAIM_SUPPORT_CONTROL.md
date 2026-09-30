# Actual Claim Support Control

**Control date:** 2026-09-30

## Purpose

This file identifies the operative nonprovisional claim-support surface and prevents stale migration instructions from being mistaken for current work.

The operative candidate claim-control surface is `P1/NONPROVISIONAL_CLAIM_READINESS.csv`, which contains Claims 1-20. `P1/P1_SUPPORT_MATRIX.csv` has now been migrated from the obsolete illustrative `CLAIM-A` through `CLAIM-F` rows to actual `CLAIM-1` through `CLAIM-20` rows. Therefore, the former instruction that the support matrix still contains six illustrative claim rows is **SUPERSEDED**.

The migrated matrix is not yet the final limitation-level §112/priority chart. Except for Claim 9's completed exact-text-coordinate reconciliation, the claim rows remain candidate-coordinate controls requiring exact frozen-file reconciliation at the limitation level. Claims 7, 8, and 19 retain heightened exact-filed-page verification requirements.

This control does not promote any claim to READY and does not infer P1 support from historical evidence. Frozen-P1 support must be established from the exact filed P1 specification/drawings.

## Operative candidate claims

| Claim | Working title | Dependency | Support-control status |
|---|---|---|---|
| 1 | Integrated runtime resolution | independent | exact filed-PDF limitation reconciliation required |
| 2 | Provenance evidence correction freshness permission filtering | claim 1 | exact filed-PDF limitation reconciliation required |
| 3 | Inference-resource budget | claim 1 | exact filed-PDF limitation reconciliation required |
| 4 | Event lifecycle relevance | claim 1 | exact filed-PDF limitation reconciliation required |
| 5 | Correction supersession and preserved provenance | claim 1 | exact filed-PDF limitation reconciliation required |
| 6 | Model-independent durable reconstruction | claim 1 | exact filed-PDF limitation reconciliation required |
| 7 | Physical identifier namespace resolution and write-back | claim 1 | exact-filed-page verification required |
| 8 | Offline capture and authoritative reconciliation | claim 7 | exact-filed-page verification required |
| 9 | Workstream continuity under Person State change | independent | exact text coordinates reconciled; frozen FIGS. 4/8 and remaining legal gates open |
| 10 | Person State fields and field-specific freshness | claim 9 | exact filed-PDF limitation reconciliation required |
| 11 | Newer evidence correction or supersession before resume | claim 9 | exact filed-PDF limitation reconciliation required |
| 12 | Do-not-repeat state | claim 9 | exact filed-PDF limitation reconciliation required |
| 13 | Mobile or voice feasibility transition | claim 9 | exact filed-PDF limitation reconciliation required |
| 14 | Bounded resume package | claim 9 | exact resume-point and permission-information boundaries require reconciliation |
| 15 | Provider-independent handoff | independent | exact filed-PDF limitation reconciliation required |
| 16 | Different provider or local-cloud runtime transfer | claim 15 | exact filed-PDF limitation reconciliation required |
| 17 | Handoff correction provenance permission evidence do-not-repeat | claim 15 | each alternative requires individual exact-P1 support verification |
| 18 | Permission-scoped reduced handoff | claim 15 | exact filed-PDF limitation reconciliation required |
| 19 | Replacement endpoint restore | claim 15 | exact-filed-page verification required |
| 20 | Post-reconstruction durable write-back | claim 15 | exact filed-PDF limitation reconciliation required |

## Current matrix rule

`P1/P1_SUPPORT_MATRIX.csv` is now an operative **claim-level routing matrix**, not an obsolete illustrative-claim matrix. Its `CLAIM-1` through `CLAIM-20` rows may be used to route exact-P1 review, but—unless a row expressly records completed reconciliation—they must not be treated as proof that every limitation is supported.

The next refinement is limitation-level decomposition for each claim. Each limitation row must identify, at minimum:

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

For Claim 9 and its dependents, preserve the distinction between **persistent workstream identity** and **mutable checkpoint/resume state**. Claim 9's exact frozen-P1 text coordinates have been reconciled in `CLAIM9_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`; frozen FIGS. 4/8 still require visual inspection. The earlier universal static resume-point-invariance formulation is not operative. A narrower preserved-checkpoint embodiment may be used only to the extent confirmed by the exact frozen filing. Any stronger authority/priority reconciliation mechanism must be separately mapped to frozen P1 or treated as later matter.

## Readiness effect

This reconciliation removes a stale control-plane contradiction: the repository no longer instructs reviewers to migrate a matrix that has already been migrated. It does **not** close the P1-support gate. Overall filing status remains `NOT_READY` until the operative claims receive required limitation-level frozen-P1 reconciliation and the remaining filing-critical gates close.
