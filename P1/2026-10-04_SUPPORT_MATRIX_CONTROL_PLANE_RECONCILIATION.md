# P1 Support-Matrix Control-Plane Reconciliation — 2026-10-04

## Purpose

Prevent stale `P1/P1_SUPPORT_MATRIX.csv` row labels from being mistaken for the current filing-readiness state. This is a control-plane reconciliation only; it does not create new P1 disclosure, enlarge priority, or clear any statutory gate.

## Frozen priority boundary

Priority remains limited to the exact frozen P1 specification/drawings associated with U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16. Later implementation evidence and later control documents may corroborate or audit the mapping but cannot backfill disclosure into P1.

## Reconciliation finding

`P1/NONPROVISIONAL_CLAIM_READINESS.csv` and the dedicated exact-frozen-P1 controls have advanced beyond several stale row labels in `P1/P1_SUPPORT_MATRIX.csv`. The stale matrix labels are therefore not authoritative where a later dedicated control and the readiness table agree.

Current controlled written-description / P1-priority dispositions are:

- Claim 1 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIM1_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claims 2–5 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed respectively by `CLAIM2_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`, `CLAIM3_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`, `CLAIM4_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`, and `CLAIM5_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claim 6 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; `FIG6_RECONCILED`; governed by `CLAIM6_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claims 7–8 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIMS7_8_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claim 9 — `EXACT_TEXT_COORDINATES_RECONCILED`; frozen FIGS. 4/8 inspection remains separate; governed by `CLAIM9_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claim 10 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIM10_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claim 11 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIM11_EXACT_FROZEN_P1_SUPPORT_CONTROL.md` and the antecedent-basis cure control.
- Claims 12–13 — `P1_PRIORITY_WORDING_CURED_BY_NARROWING`; governed by `CLAIMS12_13_FILING_NARROWING_CONTROL.md`. Removed broader alternatives are not restored.
- Claim 14 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIM14_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claim 15 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; `FIG6_RECONCILED`; governed by `CLAIM15_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`.
- Claims 16–20 — `EXACT_FROZEN_P1_SUPPORT_CONTROLLED`; governed by `CLAIMS16_20_EXACT_FROZEN_P1_SUPPORT_CONTROL.md`. Claim 19 clearance applies only to its narrowed canonical wording; rejected endpoint-lifecycle matter remains outside P1 priority.

## Important non-clearances

These dispositions concern §112(a) written-description/P1-priority mapping only. They do **not** by themselves clear enablement, best mode, §101, §102, §103, §112(b), §112(f), inventorship, material-information review, public-disclosure review, drawings-wide QA, filing papers, fees, Patent Center validation, or exact-file QA.

## Control rule until CSV synchronization

For claim-support status, use this precedence order:

1. exact frozen P1 itself;
2. dedicated claim-specific frozen-P1 support/narrowing control;
3. `P1/NONPROVISIONAL_CLAIM_READINESS.csv`;
4. `P1/P1_SUPPORT_MATRIX.csv` row label.

A stale lower-precedence label must never reopen a limitation already reconciled by a higher-precedence control, and it must never be used to broaden a limitation beyond the higher-precedence control.

## Required follow-through

Synchronize the claim rows in `P1/P1_SUPPORT_MATRIX.csv` to the dispositions above without altering the SPEC/FIG historical-evidence rows or implying that historical conception evidence establishes filed disclosure. After synchronization, re-run exact-file/final-claim QA so the matrix, operative claim text, and final specification remain identical at the filing boundary.

## Disposition

**CONTROL-PLANE DRIFT IDENTIFIED AND BOUNDED.** The stale matrix labels are now expressly subordinated to the dedicated exact-frozen-P1 controls and the current claim-readiness table. This is a filing-record integrity improvement, not a READY determination.