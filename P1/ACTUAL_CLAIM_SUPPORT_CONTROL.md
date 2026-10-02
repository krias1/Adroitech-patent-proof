# Actual Claim Support Control

**Control date:** 2026-10-02

## Purpose

This file identifies the operative nonprovisional claim-support surface and prevents stale migration or reconciliation instructions from being mistaken for current work.

The operative candidate claim-control surface is `P1/NONPROVISIONAL_CLAIM_READINESS.csv`, which contains Claims 1-20. `P1/P1_SUPPORT_MATRIX.csv` is a routing matrix and must not override a later claim-specific exact-frozen-P1 support control.

The exact frozen P1 specification/drawings remain the priority boundary. Historical evidence and later implementation evidence may corroborate conception or implementation but cannot repair or enlarge P1 priority.

## Current claim-support disposition

| Claim | Working title | Dependency | Frozen-P1 written-description / priority disposition |
|---|---|---|---|
| 1 | Integrated runtime resolution | independent | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 2 | Provenance evidence correction freshness permission filtering | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 3 | Inference-resource budget | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 4 | Event lifecycle relevance | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 5 | Correction supersession and preserved provenance | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 6 | Model-independent durable reconstruction | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 7 | Physical identifier namespace resolution and write-back | claim 1 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 8 | Offline capture and authoritative reconciliation | claim 7 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 9 | Workstream continuity under Person State change | independent | EXACT_TEXT_COORDINATES_RECONCILED; frozen FIGS. 4/8 still require inspection |
| 10 | Person State fields and field-specific freshness | claim 9 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 11 | Newer evidence correction or supersession before resume | claim 9 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 12 | Do-not-repeat state | claim 9 | SUPPORT_GAP_REQUIRES_NARROWING |
| 13 | Mobile or voice feasibility transition | claim 9 | SUPPORT_GAP_REQUIRES_NARROWING_OR_EXACT_PDF_VERIFICATION |
| 14 | Bounded resume package | claim 9 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 15 | Provider-independent handoff | independent | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 16 | Different provider or local-cloud runtime transfer | claim 15 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 17 | Handoff correction provenance permission evidence do-not-repeat | claim 15 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 18 | Permission-scoped reduced handoff | claim 15 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |
| 19 | Replacement endpoint restore | claim 15 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED to narrowed canonical wording |
| 20 | Post-reconstruction durable write-back | claim 15 | EXACT_FROZEN_P1_SUPPORT_CONTROLLED |

## Claim 12 adverse control

Current Claim 12 is not P1-cleared in its present wording. The frozen P1 establishes persistent `do_not_repeat` state and its checkpoint/resume/handoff carriage, but the presently reconciled frozen disclosure does not establish the full later taxonomy tying that state to both completed **or rejected** operations and the complete suppression wording. Filing-safe disposition: narrow Claim 12 to the actually disclosed persistent do-not-repeat/checkpoint-resume machinery unless stronger exact frozen-P1 support is independently located. Do not use later implementation evidence to cure this gap.

## Claim 13 adverse control

Current Claim 13 is not P1-cleared in its present alternative wording. Exact frozen-P1 reconciliation supports the mobile + discussion/planning + deferred workstation/physical-access embodiment. The `voice interface` and `retrieval` alternatives remain outside the currently established exact-P1 support boundary unless exact frozen-PDF coordinates are independently located. Filing-safe disposition: narrow to the reconciled mobile embodiment or separately verify the disputed alternatives before asserting P1 priority.

## Claim 9 architecture control

For Claim 9 and its dependents, preserve the distinction between **persistent workstream identity** and **mutable checkpoint/resume state**. The earlier universal static resume-point-invariance formulation is not operative. Claim 14's `exact resume point` refers to the operative resume point represented in the bounded resume package, not an immutable pointer that can never change after reconciliation.

## Control precedence

Where `P1/P1_SUPPORT_MATRIX.csv` still contains an older routing status such as `exact_filed_pdf_reconciliation_required`, the later claim-specific control document and `P1/NONPROVISIONAL_CLAIM_READINESS.csv` govern. The routing matrix should be synchronized, but stale matrix text must not reopen a completed control or erase an adverse support finding.

## Remaining gate consequence

Closing written-description/priority control does **not** make a claim filing-ready. Enablement, best mode, §101, §102, §103, §112(b), §112(f) where relevant, figure inspection, inventorship, material-information/public-disclosure review, specification/claim drafting, filing papers, fee calculation, exact-file QA, and submission-packet QA remain separate gates.

Overall filing status remains `NOT_READY`. The immediate claim-drafting blockers are Claims 12 and 13: narrow them to the frozen-P1-supported embodiments or independently establish exact frozen-PDF support for the disputed limitations before finalizing the filing claim set.
