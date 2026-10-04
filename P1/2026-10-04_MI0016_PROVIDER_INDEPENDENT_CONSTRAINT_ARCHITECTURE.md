# MI-0016 — Provider-Independent Hierarchical Constraint Enforcement Architecture

**Review date:** 2026-10-04
**Reference:** US20260228755A1, “Provider-Independent Hierarchical Constraint Enforcement Architecture for Artificial Intelligence Systems”
**Reported filing date:** 2026-03-23
**Reported publication date:** 2026-08-06
**P1 date:** 2026-09-16
**Disposition:** HIGH_PRIORITY_CANDIDATE_REVIEW / IDS_MATERIALITY_REVIEW_REQUIRED / CLAIM15_COMBINATION_PRESSURE

## Why preserved

This reference predates P1 and expressly describes a provider-independent architecture around AI processing pipelines, deployer-owned persistent state maintained independently of the AI-processing-pipeline provider, and persistence through provider substitution. Reported claim 35 recites a deployer-owned persistent state store independent of both middleware and third-party AI processing pipeline providers; reported claim 36 recites substitution of the third-party AI processing pipeline without affecting the constraint layer and substitution of the middleware provider without loss of constraint state/history/audit records.

Those teachings create material component pressure against any argument that provider independence, provider substitution, or externally/durably maintained state independent of an AI provider is itself a safe novelty refuge for operative Claim 15 or its dependents.

## Claim-family pressure

### Claim 15

Potentially overlapping components:
- provider-independent architecture surrounding an AI runtime/pipeline;
- persistent state maintained outside the provider-specific AI processing pipeline;
- continued operation despite provider substitution;
- state/history surviving substitution.

Not facially established from the reviewed material:
- the exact operative Claim 15 bounded handoff package;
- reconstruction by a second AI runtime from that package/state sufficient to resume the claimed workstream;
- the exact independence from the originating runtime's private conversation state as presently controlled;
- the full ordered combination of Claim 15.

Therefore **no §102 anticipation conclusion is recorded**.

### Claims 16–20

The reference increases §103 pressure particularly for provider/runtime substitution (Claim 16), permission/governance-related handoff content (Claims 17–18), endpoint/provider independence concepts (Claim 19), and durable state surviving or following runtime substitution (Claim 20). Each operative limitation still requires element-level comparison; this control does not collapse distinct limitations into generic “provider independence.”

## Combination analysis

Adversarially combine this reference with existing MI-0008 (serialized context / cross-agent handoff), MI-0004 (stateful runtime/checkpoint persistence), and MI-0015 (persisted AI task/context state and resumption). The principal risk is that an examiner could use MI-0016 to supply the provider-independent/deployer-owned-state motivation and use another reference to supply bounded serialized handoff/reconstruction/resumption mechanics.

The prosecution-safe response is not to deny those teachings. The claim analysis must continue to test whether the exact ordered combination—especially bounded handoff construction, second-runtime reconstruction sufficient for resumption, and independence from originating private conversation state—is taught or would have been obvious in combination.

## Candor / IDS control

Preserve this reference in the material-information lane. Final IDS/materiality treatment must be decided against the exact final claims and the complete reference, not merely the surfaced abstract/claim excerpts. Do not suppress it because it narrows the available distinction.

## Source integrity

Initial discovery was from public patent-index material on 2026-10-04. Before final IDS citation data is frozen, reconcile bibliographic data and the complete publication against an authoritative patent record/PDF. This file records an adverse-search finding; it is not a substitute for the final IDS bibliographic record.

## Register synchronization

This control is assigned **MI-0016**. `P1/MATERIAL_INFORMATION_REGISTER.csv` must be physically synchronized with this record before READY. Until that write occurs, this file is the controlling preservation record for MI-0016 and the front-door material-information gate remains IN_PROGRESS.
