# MI-0015 — Notion AI State-Resume Prior Art Control

**Review date:** 2026-10-03
**Reference:** US20250217116A1, *Data model for artificial intelligence assistant*
**Applicant/assignee:** Notion Labs, Inc.
**Earliest claimed priority:** 2023-12-29 (U.S. Provisional 63/616,450)
**U.S. filing:** 2024-05-03 (US18/654,977)
**Publication:** 2025-07-03
**Source:** https://patents.google.com/patent/US20250217116A1/en

## Why this is material

This pre-P1 reference directly pressures broad continuity/resume formulations in operative Claims 9 and 15 and generic durable AI-state formulations in Claim 1. It describes an AI assistant that stores representations of interaction states so past interactions can be resumed or modified without losing the corresponding environment context. Its disclosed process stores transcript states corresponding to tasks, accesses a selected stored state, and executes code associated with that state using the environment context corresponding to that state to reperform a task. The specification also describes persistent/source-of-truth records and structured digital-environment context.

The reference therefore removes any safe novelty refuge based merely on: (1) storing AI-assistant interaction/task state; (2) persisting context associated with a task; (3) selecting a prior stored state; (4) resuming or replaying an earlier AI-assisted task from stored context; or (5) generic persistence of AI workflow state.

## Adverse claim pressure

### Claim 9

Strong component pressure exists for persisted task/workstream state and later resumption from a stored prior state/context. This reference should be combined adversarially with MI-0011 (interruption/resumption under changing user/situation state), MI-0013 (separately tracked user state and task state with candidate-action selection), and MI-0014 (verified/in-progress workflow recovery state).

The reference does **not facially establish** operative Claim 9's full combination: separately maintained Person State; a Person-State operational constraint that prevents the stored-resume-point execution action; selection of a different executable action while the workstream remains paused/frozen/non-advanced; and later resumption when a subsequent Person State permits the stored-resume-point action. No §102 anticipation conclusion is recorded.

### Claim 15

The reference pressures generic state preservation and reconstruction/resumption concepts. Its principal disclosed resume mechanism, however, is transcript-state-centered: stored states include portions of a transcript and associated code/context. That is materially different from relying on this reference alone for Claim 15's complete provider-independent handoff representation supplied to a second AI runtime independently of the first runtime's private conversation state. Combination analysis remains required, especially with MI-0008 and other cross-agent/provider handoff references.

### Claim 1

The reference pressures generic durable state, context persistence, and AI task execution from stored context. It does not facially establish Claim 1's complete entity/alias resolution, machine-enforced bounded current-world-slice selection, and transcript-independent durable write-back combination.

## Material-information disposition

**Materiality status:** HIGH_PRIORITY_CANDIDATE_REVIEW
**IDS review:** NOT_YET_DETERMINED
**Claim chart:** CLAIM_LEVEL_CHART_REQUIRED

Preserve this reference even if it forces narrower claims. It is adverse evidence, not promotional literature. The safe inventive center must be tested against the actual combinations, not against generic AI memory/resume language.

## Register synchronization

This control is the evidence record for `MI-0015`. `P1/MATERIAL_INFORMATION_REGISTER.csv` must include a corresponding MI-0015 row before final READY/IDS review; if the centralized CSV has not yet been synchronized, that is an explicit filing-control gap rather than grounds to omit this reference.
