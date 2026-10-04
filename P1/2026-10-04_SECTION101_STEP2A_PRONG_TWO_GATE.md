# §101 Step 2A Prong Two Gate — Operative Claims 1, 9, and 15

Date: 2026-10-04
Status: PASS_EVIDENCE / FINAL-SPEC-AND-CLAIM QA PENDING
Operative claim source blob: `49fefff7d2d241b2d74e93a567ffbf47f6e6f63c`
Claim surface: 20 total / 3 independent (1, 9, 15)

## Scope

This filing-critical control applies current USPTO Step 2A Prong Two improvement/practical-application guidance to the three operative independent claim families. It does not establish novelty, nonobviousness, enablement, definiteness, or allowance. It does not manufacture a technical effect from later matter. The asserted improvements remain bounded by frozen P1 disclosure and must be reflected in final filing claims.

## Current authoritative rule

Current USPTO MPEP §2106.04(d) requires evaluation of the claim as a whole. A recited judicial exception can be integrated into a practical application where additional elements impose a meaningful limit, including an improvement in computer functionality or another technology/technical field. Under §2106.04(d)(1), the specification must provide sufficient technical detail for a skilled artisan to recognize the asserted technological improvement, and the claim itself must reflect the components or steps producing that improvement. A conclusory assertion of improvement is insufficient. Step 2A Prong Two does not turn on whether the elements are well-understood, routine, and conventional; that issue belongs to Step 2B.

The USPTO's December 5, 2025 eligibility update reemphasizes whole-claim treatment of technological advances and distinguishes eligibility from §§102, 103, and 112.

Authoritative controls:
- https://www.uspto.gov/web/offices/pac/mpep/s2106.html
- https://www.uspto.gov/subscription-center/2025/uspto-updates-subject-matter-eligibility-guidance-mpep

## Claim 1 family — integrated durable-state runtime architecture

Adverse abstraction: collecting/storing information about a person or world, resolving names/identities, and selecting information for an AI.

Prong-Two mechanism: the claim's eligibility position rests on the combination of durable person/world state, namespace/entity resolution, construction of a machine-bounded current-world slice from that durable state, runtime use of that bounded slice, and durable material-state write-back outside merely private conversational state.

Technical effect: changes the computer/runtime state boundary used for inference and later authorized reuse. The runtime is supplied a resolved bounded machine-consumable state representation rather than treating an unbounded/provider-private transcript as the operative continuity authority; material resulting state persists outside the originating private conversation.

Disposition: PASS_EVIDENCE for a concrete technological-improvement theory, subject to final comparison proving that the filed specification technically explains this architecture and the final Claim 1 family actually recites the steps/components relied upon. Do not substitute personalization, better answers, or user benefit for the technical mechanism.

## Claim 9 family — separated state domains and resume control

Adverse abstraction: project management, remembering circumstances, deciding what task can be done next, or scheduling human activity.

Prong-Two mechanism: persistent machine-maintained workstream state/resume point is maintained separately from mutable Person State; evidence of Person-State change triggers evaluation of operational constraints and recomputation/selection of feasible next action while the underlying workstream state remains preserved rather than falsely advanced.

Technical effect: changes runtime state-transition/control behavior by applying different update semantics to two persistent state domains. Changed feasibility state can alter machine action selection without destroying or automatically advancing the durable workstream checkpoint.

Disposition: PASS_EVIDENCE for a concrete technological-improvement theory, subject to final specification/claim comparison. Do not reduce the filing argument to the human concept of remembering or resuming a task.

## Claim 15 family — provider-independent structured reconstruction

Adverse abstraction: transferring information, remembering a user, or handing a task between services/devices.

Prong-Two mechanism: another AI runtime reconstructs an identified workstream from a defined provider-independent durable handoff representation containing resolved person/entity/workstream/current-state/resume information without requiring the originating runtime's private conversation state.

Technical effect: changes the dependency boundary between runtimes and provider-private session state. Operative context can be reconstructed from durable structured state across a runtime/provider boundary rather than requiring the first runtime's private transcript/session as continuity authority.

Disposition: PASS_EVIDENCE for a concrete technological-improvement theory, subject to final specification/claim comparison. Provider independence is not asserted as policy or consumer preference; the eligibility theory is the claimed structured state representation and reconstruction operation.

## Adversarial conclusions

1. The three independent families each have a concrete computer/runtime/storage mechanism capable of supporting Step 2A Prong Two; none is being justified merely by novelty, philosophy, social benefit, or generic AI use.
2. This is not a final §101 PASS. The final filing specification must technically explain each asserted improvement and each final independent claim must reflect the steps/components producing it.
3. If final drafting strips out the state-boundary, separated-state-domain, or structured-handoff mechanics relied upon here, this gate reopens and the affected claim cannot inherit this disposition.
4. Dependent claims require final claim-by-claim review because USPTO eligibility analysis is claim-specific; a dependent limitation may alter the analysis.
5. Step 2B remains a separate fallback analysis if an examiner concludes a claim is directed to an abstract idea after Step 2A.
6. No Rule 132 declaration can be used to supply a technical explanation absent from the filed specification.

## Filing disposition

`SECTION101_STEP2A_PRONG_TWO = PASS_EVIDENCE / FINAL-SPEC-AND-CLAIM QA PENDING`

Overall §101 remains unresolved until final specification/claim QA and Step 2B fallback review are completed. This control narrows the remaining eligibility work; it does not declare the application READY.