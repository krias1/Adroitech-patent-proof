# Examiner Matrix Reconciliation — 2026-09-30

## Purpose

This control prevents stale statements in `P1/EXAMINER_QUESTION_MATRIX.csv` from being treated as current filing facts during the nonprovisional perfection sprint.

## Authoritative current state

1. The operative candidate claim-control surface is `P1/NONPROVISIONAL_CLAIM_READINESS.csv` and contains Claims 1–20.
2. The current claim architecture contains 20 total claims and 3 independent claims (Claims 1, 9, and 15).
3. `P1/P1_SUPPORT_MATRIX.csv` has been migrated from the obsolete CLAIM-A–CLAIM-F placeholder model to the operative Claims 1–20.
4. Claim 9 written-description / P1-priority text reconciliation has reached `EXACT_TEXT_COORDINATES_RECONCILED`; frozen FIGS. 4 and 8 remain a separate visual-inspection gate.
5. The formal USPTO Filing Receipt remains unreconciled. Preserved acknowledgement evidence does not substitute for that still-open formal-record gate.
6. Prior-art review remains open. `P1/MATERIAL_INFORMATION_REGISTER.csv` now includes high-priority adverse references requiring claim-level charting, including the stateful-AI-runtime reference tracked as MI-0004 and entity-resolution component art tracked as MI-0005.
7. No claim is filing-cleared merely because a support coordinate or candidate claim exists. §101, §102, §103, §112(a), §112(b), §112(f) where implicated, inventorship, best mode, material-information, public-disclosure, drawings, formalities, fees, and exact-file QA remain independent gates until affirmatively closed.

## Stale examiner-matrix statements — do not rely on these literally

The following rows in `P1/EXAMINER_QUESTION_MATRIX.csv` predate the operative 20-claim migration and contain stale statements that the final/actual claim set is absent or that claims cannot yet be evaluated because claims do not exist:

- EQ-001 — claim set absent.
- EQ-002 — final claims absent.
- EQ-004 — cannot classify until final claims exist.
- EQ-008 — actual claim limitations not mapped.
- EQ-011 — actual final limitations absent.
- EQ-014 — final claim language not fixed.
- EQ-023 — final dependent claim tree not present.
- EQ-029 — cannot evaluate until final claims exist.

Those statements are superseded only to the extent they assert **absence of an operative candidate claim set**. They are **not** converted into closed statutory or filing-readiness findings. The correct current question is whether each operative candidate claim has passed the applicable gate.

## Current routing rule

For any conflict:

1. use `P1/NONPROVISIONAL_READINESS.md` for sprint/readiness state;
2. use `P1/NONPROVISIONAL_CLAIM_READINESS.csv` for claim-level gate state;
3. use `P1/P1_SUPPORT_MATRIX.csv` for P1 support state;
4. use `P1/MATERIAL_INFORMATION_REGISTER.csv` for adverse-art/material-information state;
5. use the frozen P1 specification/drawings identified by `P1/P1_FILING_ANCHOR.md` as the priority-support boundary.

No later evidence may be used to backfill P1 support.

## Required follow-up

The examiner matrix itself should be rewritten row-by-row against Claims 1–20 after the current limitation-level support and adverse-art charting pass. Until then, this reconciliation control is mandatory whenever the matrix is used.
