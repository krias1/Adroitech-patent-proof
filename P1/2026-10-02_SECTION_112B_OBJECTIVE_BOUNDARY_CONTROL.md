# §112(b) Objective-Boundary Control — Operative Nonprovisional Claims

**Date:** 2026-10-02  
**Anchor:** U.S. Provisional Application No. 64/155,744, filed 2026-09-16  
**Operative claim surface:** 20 claims / 3 independent claims (1, 9, 15)  
**Status:** FILING-CRITICAL DRAFTING CONTROL / NOT FINAL CLAIM FREEZE

## Purpose

This control converts the previously located relative/result-oriented §112(b) risks into concrete filing routes without adding post-P1 substance or pretending that later implementation evidence enlarges the frozen P1 priority boundary.

## Independent Claim 1

### `bounded subset` / `current world slice`

**Disposition: OBJECTIVE P1-SUPPORTED BOUNDARY AVAILABLE.**

Use the disclosed machine-enforced resource limits as the objective boundary. The frozen disclosure identifies token, byte, node, edge, record, cost, and latency budgets and describes selection of a machine-readable current world slice. Claim 3 already supplies an objective dependent fallback.

**Filing treatment:** preserve `bounded` only with an express specification definition tying the boundary to one or more machine-enforced resource/relevance limits. Do not invent a numerical threshold.

### `material state change`

**Disposition: HIGH-RISK TERM; ENUMERATED PERSISTENCE ROUTE PREFERRED.**

The frozen disclosure gives concrete persisted state classes, including entity/alias resolution, relationship change, correction, event/state transition, workstream checkpoint, completed action, failure/blocker/dependency, and authoritative-source update. `Material` standing alone remains relative.

**Preferred claim-hardening route:** replace result-oriented `material state change` in Claims 1, 7, and 20 with P1-supported enumerated persisted state classes appropriate to each claim, or expressly define the term as a persistence-policy selection among those disclosed durable state classes. No post-P1 threshold may be introduced and attributed to P1.

## Independent Claim 9

### `exact resume point`

**Disposition: REPLACE `exact` UNLESS FINAL EXACT-PDF REVIEW ESTABLISHES AN OBJECTIVE ADDITIONAL BOUNDARY.**

The frozen architecture supports a stored checkpoint/resume state identifying where a workstream continues. It does not support treating the resume point as an immutable byte/instruction pointer. Persistent workstream identity and mutable checkpoint/resume state are distinct.

**Preferred filing wording:** `stored resume point` or `identified resume point`, consistently throughout Claims 9 and 14. Any adopted replacement must be propagated through the specification and support matrix.

### `feasible` / `not presently feasible`

**Disposition: OBJECTIVE P1-SUPPORTED BOUNDARY AVAILABLE.**

Tie execution eligibility to stored Person-State fields such as endpoint/interface, network state, available tool, movement state, resource constraint, or physical constraint. Claim 10 supplies the dependent fallback.

**Filing treatment:** the independent claim should make clear that feasibility is determined from at least one stored Person-State operational constraint, not subjective convenience.

## Independent Claim 15

### `bounded handoff representation`

**Disposition: OBJECTIVE P1-SUPPORTED BOUNDARY AVAILABLE.**

The handoff representation already enumerates minimum state classes: person/namespace identifier, resolved entity identifiers, current Person State, workstream identifier, and resume point. Permission/resource filtering may reduce other transferred state.

**Filing treatment:** define `bounded` by selected required fields plus disclosed permission/resource selection, not by an invented numerical limit.

### `operational context sufficient to resume`

**Disposition: RESULT-ORIENTED WORDING SHOULD BE REMOVED FROM THE INDEPENDENT CLAIM.**

Claim 15 already recites the concrete reconstruction inputs. The stronger §112(b) formulation is to recite reconstructing the identified active workstream at the second runtime from the handoff representation, without requiring the first runtime's private conversation state. `Sufficient` adds avoidable uncertainty.

### `authoritative` / `authoritative source of truth`

**Disposition: DO NOT USE AS AN UNDEFINED TRUTH STANDARD.**

Where the concept remains necessary, use P1-supported designated durable state/system-of-record semantics: durable person-specific state used for reconstruction rather than endpoint-local state. Claim 19 should not depend on metaphysical or subjective `authoritative` correctness.

## Dependent-claim terms requiring propagation review

- Claim 5: replace or objectively constrain `historical context calls for` using the disclosed historical-query/context selection condition if retained.
- Claim 7: apply the Claim 1 enumerated persistence treatment to `material state change`.
- Claim 8: define reconciliation against designated durable state rather than undefined `authoritative` truth.
- Claim 11: chronology/version evidence does not automatically override higher-authority state; preserve the disclosed correction/supersession semantics.
- Claim 14: propagate `stored`/`identified resume point` if Claim 9 is changed; tie `selected relevant durable state` to disclosed namespace/Person-State/workstream/permission/resource selection criteria.
- Claim 19: replace `authoritative source of truth` with designated/provider-independent durable-state language already supported by the frozen architecture.
- Claim 20: apply the Claim 1 enumerated persistence treatment.

## §112(f) posture

The operative independent claims remain method-act claims and intentionally avoid `means for` language and nonce module/manager/mechanism elements. No current limitation is intentionally drafted to invoke §112(f). This is not a categorical safe harbor: any later system/apparatus claim using functional nonce structure must receive a fresh §112(f) screen and corresponding algorithm/structure mapping.

## Filing gate

This control **does not mark §112(b) PASS**. It does materially reduce the drafting ambiguity by fixing the permissible cure route for each high-risk term. Before READY:

1. propagate adopted objective wording into the canonical operative claims;
2. rerun limitation-level frozen-P1 support on every changed limitation;
3. rerun dependency/antecedent-basis review;
4. synchronize the nonprovisional terminology section;
5. compare final filing text byte-for-byte against the controlled claim set.

No later implementation detail may be used to manufacture P1 support for a cure.