# P1-Safe Terminology Control — Operative Nonprovisional Claims

**Date:** 2026-10-03  
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16  
**Purpose:** narrow the remaining §112(b) terminology surface without adding post-P1 subject matter. This control governs drafting only to the extent each construction remains consistent with the exact frozen P1 specification. It is not permission to backfill later implementation details.

## Governing rule

Where the frozen P1 already supplies an objective contextual meaning, preserve that meaning in the nonprovisional specification. Do not manufacture numerical thresholds, certification procedures, immutable pointers, physical-storage separation, secrecy requirements, or activity thresholds that P1 did not disclose. If final claim language cannot be reconciled to the frozen disclosure on that basis, narrow the claim rather than enlarge P1 by definition.

## 1. Person State

**P1-safe construction:** `Person State` is durable state representing the person's current operational circumstances used by the runtime when selecting or constraining an action, together with freshness/time information where disclosed. It is maintained separately as logical state from a Context VM/workstream record.

**Do not imply:** a mandatory exhaustive field list, a medical diagnosis, a subjective psychological assessment, or a numerical freshness threshold unless expressly recited and supported.

**Frozen-P1 basis:** Detailed Description §§5–6 and the Claim 9 exact-frozen support control.

## 2. Independently resumable workstream / Context VM

**P1-safe construction:** a workstream/Context VM is independently resumable when durable workstream identity and checkpoint/resume state permit that workstream to be continued without requiring preservation of the originating conversational transcript as the continuity authority.

**Do not imply:** that every checkpoint is immutable, that a resume pointer can never be superseded, or that execution of another compatible action can never produce a later valid checkpoint.

**Frozen-P1 basis:** Detailed Description §§6, 8, 11–12; Example 2; Claim 9 exact-frozen support control.

## 3. State maintained separately from conversational transcript data

**P1-safe construction:** `separately` denotes logical and continuity-authority independence: the durable person/workstream state is persisted in a form usable for runtime reconstruction or continuation without requiring the conversational transcript itself as the authoritative continuity record.

**Do not imply:** mandatory separate disks, databases, files, physical hosts, encryption domains, or that facts learned during conversation cannot later be persisted into durable state.

## 4. Last verified state

**P1-safe construction:** `last verified state` refers to the accepted/persisted workstream state represented by the applicable Context VM checkpoint before the subsequent resume/reconciliation operation. `Verified` does not require an undisclosed external certification protocol or numerical confidence threshold.

**Drafting consequence:** this phrase is supportable only in that checkpoint/state context. If final claim wording makes `verified` perform additional technical work beyond the disclosed accepted/persisted checkpoint semantics, replace it with a narrower stored/checkpoint-state formulation rather than inventing a verification mechanism.

**Frozen-P1 basis:** Detailed Description §6 expressly identifies the Context VM as including `last verified state`; §§8 and 11 use active/latest Context VM checkpoint state in bounded reconstruction/resume.

## 5. Paused / frozen workstream state

**P1-safe construction:** for the operative Claim 9 embodiment, `paused` and `frozen` identify a condition in which the workstream/Context VM is preserved for later continuation while Person State may change. The terminology does not establish immutable checkpoint invariance. A later valid checkpoint may supersede an earlier checkpoint when the workstream actually advances.

**Do not imply:** that `paused` and `frozen` create two undisclosed lifecycle protocols or two different storage formats. If the final specification elects to distinguish them, that distinction must come from frozen P1 rather than later implementation.

**Frozen-P1 basis:** Detailed Description §11; Example 2; frozen FIG. 8 only if filing receipt/content evidence ultimately establishes that drawing as filed P1 disclosure. Text support is sufficient for the preserved-workstream/changed-Person-State concept and remains the controlling safe basis while drawing receipt is unresolved.

## 6. Private conversation state

**P1-safe construction:** provider/runtime-specific conversational or session state of the originating AI runtime that is not required as the durable authority for reconstruction or continuation by the receiving/replacement runtime.

**Do not imply:** secrecy from the user, confidentiality classification, inability to export a transcript, or prohibition on persisting durable facts that were initially learned during a conversation.

**Frozen-P1 basis:** Detailed Description §12 and Example 3's cross-provider continuation from durable/bounded workstream state without dependence on the original transcript/history.

## 7. Active namespace / active workstream

**P1-safe construction:** `active` identifies the person-specific namespace or workstream selected/resolved for the current handoff, reconstruction, or continuation operation.

**Do not imply:** a numerical activity score, minimum recent-use interval, background process execution, or a requirement that only one namespace/workstream can exist.

## §112(b) consequence

These constructions remove the remaining terminology ambiguity identified by the 2026-10-03 operative-V2 re-audit **at the specification-definition level**, subject to final exact-text propagation and whole-claim review. They do not by themselves make §112(b) PASS. Before PASS, the final specification and claims must be compared word-for-word against this control, dependency/antecedent basis must remain clean, and no later-added definition may enlarge the P1 priority boundary.

## Priority/candor safeguard

This document is a drafting control, not new priority evidence. Priority rests only on the exact frozen P1 disclosure. Any broader later implementation belongs in later-matter/continuation/CIP analysis and must not be represented as September 16, 2026 support.
