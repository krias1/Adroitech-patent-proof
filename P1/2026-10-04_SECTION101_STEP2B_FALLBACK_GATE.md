# §101 Step 2B Fallback Gate — Operative Claims 1, 9, and 15

Date: 2026-10-04
Status: PASS_EVIDENCE / FINAL-SPEC-AND-CLAIM QA PENDING
Operative claim source blob: `49fefff7d2d241b2d74e93a567ffbf47f6e6f63c`
Claim surface: 20 total / 3 independent (1, 9, 15)

## Scope

This is the fallback eligibility control if an examiner concludes at Step 2A that an operative claim is directed to an abstract idea. It does not establish novelty, nonobviousness, enablement, definiteness, or allowance. It does not use later matter to strengthen the frozen P1 disclosure.

## Current USPTO control

MPEP §2106.05(d) confines the well-understood/routine/conventional (WURC) inquiry to Step 2B. A specific limitation or combination that is not WURC can favor eligibility. A factual determination is required to support a conclusion that additional elements are WURC. Mere disclosure in prior art—even anticipation or obviousness—is not by itself enough to establish WURC. Elements individually conventional can still amount to significantly more when arranged in a non-generic combination. MPEP §§2106.05(f)-(h) additionally require scrutiny for mere instructions to apply an exception, insignificant extra-solution activity, and field-of-use limitations.

Authoritative controls:
- https://www.uspto.gov/web/offices/pac/mpep/s2106.html
- https://www.uspto.gov/sites/default/files/documents/memo-berkheimer-20180419.PDF

## Claim 1 family

Assumed exception for fallback purposes: collecting/storing person or world information, resolving identities, and selecting information for AI processing.

Additional-elements/combination theory: durable person/world state plus namespace/entity resolution; construction of a machine-bounded current-world slice; runtime use of that bounded slice; and durable material-state write-back outside private conversational state.

Step 2B disposition: PASS_EVIDENCE as a defensible significantly-more fallback theory. The filing position relies on the ordered combination and changed runtime/state boundary, not on generic storage, generic retrieval, or generic AI invocation in isolation. Final specification and claims must preserve the relied-upon architecture. A WURC assertion against this combination must be treated as a factual issue and must not be conceded merely because individual storage/retrieval/AI operations were known.

## Claim 9 family

Assumed exception for fallback purposes: remembering project circumstances, determining feasibility, or choosing what task to do next.

Additional-elements/combination theory: persistent machine-maintained workstream state/resume point maintained separately from mutable Person State; evidence-driven Person-State update; evaluation of operational constraints; and feasible-next-action recomputation while the durable workstream checkpoint is preserved rather than falsely advanced.

Step 2B disposition: PASS_EVIDENCE as a defensible significantly-more fallback theory. The filing position rests on separated persistent state domains with different update semantics and resulting machine-control behavior, not the human concept of task resumption. Final-text QA must confirm that these mechanics remain claimed and technically described.

## Claim 15 family

Assumed exception for fallback purposes: transferring information or remembering a user/workstream across services.

Additional-elements/combination theory: provider-independent durable handoff representation containing resolved person/entity/workstream/current-state/resume information and reconstruction by another AI runtime without requiring the originating runtime's private conversation state.

Step 2B disposition: PASS_EVIDENCE as a defensible significantly-more fallback theory. The filing position rests on the structured reconstruction architecture and changed runtime dependency boundary, not merely sending data between computers. Final-text QA must preserve those mechanics.

## Adversarial controls

1. Do not equate §102/§103 prior-art evidence with WURC. A reference can anticipate or render a feature obvious without proving that the feature or ordered combination was widely prevalent/common industry practice for Step 2B.
2. Do not concede generic components as defeating the claim when the asserted inventive concept is their non-generic ordered combination.
3. Do not rely on generic data gathering, generic storage, generic network transfer, generic AI execution, output/display, or field-of-use language as the inventive concept.
4. Do not make unsupported factual claims that the ordered combinations were unconventional at the relevant time. Preserve adverse evidence and test any WURC assertion against the evidentiary standard.
5. Reopen this gate if final drafting removes or materially weakens the state-boundary, separated-state-domain, or structured-handoff mechanics.
6. Dependent claims remain subject to final claim-specific eligibility QA; they inherit no automatic PASS merely from dependency.
7. This control does not convert the existing Step 2A Prong Two evidence into a novelty argument. Eligibility remains analytically separate from §§102 and 103.

## Filing disposition

`SECTION101_STEP2B_FALLBACK = PASS_EVIDENCE / FINAL-SPEC-AND-CLAIM QA PENDING`

Combined with the existing Step 2A Prong Two control, the independent-claim §101 architecture now has both primary and fallback eligibility theories. Final §101 clearance still requires comparison against the exact final specification and exact final claims, including dependent-claim review.