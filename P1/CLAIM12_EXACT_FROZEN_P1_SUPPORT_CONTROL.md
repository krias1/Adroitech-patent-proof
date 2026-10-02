# Claim 12 Exact Frozen-P1 Support Control

**Claim:** 12 — do-not-repeat state.  
**Parent:** Claim 9 — workstream continuity under Person State change.  
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16.  
**Boundary:** exact frozen P1 specification/drawings only. Later implementation evidence cannot repair or enlarge P1 priority.

## Current canonical wording reviewed

> The method of claim 9, wherein the workstream record further comprises a do-not-repeat state identifying an already completed or rejected operation, and wherein resuming the workstream suppresses repetition of the identified operation.

## Exact-frozen support findings

The frozen P1 directly discloses a Context VM/workstream record containing **do-not-repeat state 560** and an example `do_not_repeat[]` field. The same workstream record contains last verified state, exact resume point, next executable action, blockers/dependencies, source records, pending decisions, status, confidence, and checkpoint time. P1 §7 retrieves the latest Context VM checkpoint, identifies the exact resume point and currently feasible actions, creates a bounded resume package, and preserves the workstream if execution remains deferred. P1 §12 also places `do_not_repeat` directly into the bounded cross-session/cross-provider handoff package. P1 §11 separately identifies **completed work** as a material state change eligible for durable write-back.

Those disclosures establish the existence, persistence, checkpoint/handoff carriage, and resume-time availability of do-not-repeat state. They also establish completed-work write-back.

## Adversarial priority finding — current wording is not yet cleared

The exact frozen P1 text presently reconciled does **not** expressly state the full additional semantic limitation now recited by Claim 12: that the do-not-repeat state specifically identifies an **already completed or rejected operation**, and that resuming the workstream **suppresses repetition of that identified operation**.

The term `do-not-repeat` strongly implies non-repetition, and completed work is separately disclosed as durable write-back, but a priority claim should not depend on silently importing every semantic detail of the later claim into the field label. More importantly, the currently reconciled frozen text does not expressly tie **rejected operations** to `do_not_repeat[]`. Later repository implementations cannot cure that P1 gap.

Accordingly Claim 12 remains **NOT CLEARED** for exact-frozen-P1 §112(a)/priority in its current wording.

## Filing-safe route

A narrower dependent claim can remain inside the established frozen-P1 boundary by claiming the disclosed state itself and its carriage into resume/handoff context without adding the unsupported completed-or-rejected taxonomy. A filing candidate should be drafted around the combination actually disclosed, for example: a workstream record comprising do-not-repeat state, with that state included in the checkpoint/resume or bounded handoff information used by an authorized runtime.

If suppression behavior is retained, it should be tied only to support that can be established from the exact frozen artifact or separately treated as later matter. `Rejected operation` must not be attributed to P1 unless exact frozen-P1 support is independently located.

## Gate consequence

Claim 12 is **SUPPORT_GAP_REQUIRES_NARROWING** for §112(a) written description and P1 priority. This is a deliberate adverse finding, not a drafting defect to hide. Claims 13–14 remain to be reconciled separately. All other statutory, prior-art, inventorship, best-mode, disclosure/candor, drawing, and final filing-QA gates remain open.