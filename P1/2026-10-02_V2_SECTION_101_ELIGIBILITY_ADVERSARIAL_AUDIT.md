# Operative V2 — 35 U.S.C. §101 Eligibility Adversarial Audit

**Date:** 2026-10-02
**Anchor:** U.S. Provisional Application No. 64/155,744
**Operative claim source:** `krias1/Adroitech-Logic-Core`, `NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`, blob `1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`
**Claim surface:** 20 total / 3 independent (1, 9, 15)
**Scope:** Filing-draft eligibility review only. This does not establish novelty, nonobviousness, enablement, definiteness, inventorship, or allowance.

## Current USPTO framework applied

The current USPTO framework evaluates statutory category at Step 1 and then Alice/Mayo Step 2A/2B. Step 2A Prong Two asks whether any recited judicial exception is integrated into a practical application. Current USPTO guidance emphasizes evaluation of the claim as a whole and technological/computer-functionality improvements; §§102, 103, and 112 remain separate patentability requirements.

## Adversarial abstraction attack

The strongest foreseeable abstraction is not “AI” itself. It is that the independent claims could be characterized at a high level as organizing/retrieving information about a person and work, adapting activity to circumstances, or transferring information between software runtimes. Those characterizations can resemble mental processes or methods of organizing human activity if the claims are stripped of their machine-state limitations.

The filing position must therefore rest on the limitations actually recited, not on novelty, philosophy, personalization, social benefit, or merely saying that a computer/AI performs the idea.

## Claim 1

### Concrete claimed machinery

Claim 1 requires, in combination: computer-readable storage; a person-specific namespace containing entity and relationship records; a separately maintained Person State with freshness metadata; multiple independently resumable workstream records with identifiers and checkpoints; entity/alias resolution; machine-enforced resource-limited selection from durable person-specific world state using resolved entity/alias + Person State + selected workstream; construction of a current world slice; supply of that slice to an AI inference engine; and persistence of enumerated durable state changes separately from conversational transcript data.

### Technical effect

The claimed combination changes how machine state is selected, bounded, supplied to inference, and persisted across inference operations. It does not merely ask an AI to remember or reason about a person. It defines a storage/selection/runtime architecture in which transient transcript state is separated from durable structured state, current inference context is machine-bounded from that durable state, and post-inference changes are persisted in enumerated durable-state classes.

### Eligibility conclusion

**PASS for filing-draft §101 posture.** Even assuming Prong One abstraction, the claim has a strong Step 2A Prong Two practical-application position because the recited exception is embedded in a specific computer-state architecture and machine-enforced context-construction process. Do not weaken the claim/specification into generic “personalized AI” language.

## Claim 9

### Concrete claimed machinery

Claim 9 requires a stored workstream identifier, last verified state and stored resume point; separately stored Person States; machine state in which a workstream remains paused/frozen; evidence of a Person-State change; evaluation of stored operational constraints; selection of a different action executable under the changed stored constraints while preserving the paused workstream; and later resumption from the stored resume point when a Person State permits execution.

### Technical effect

The claimed mechanism preserves execution continuity while runtime-operating conditions change, without discarding or advancing the frozen workstream state. The machine uses separately stored operational-state data to prevent an unavailable execution path from corrupting or replacing the stored resume point and later resumes from that persisted point.

### Eligibility conclusion

**PASS for filing-draft §101 posture, with higher abstraction pressure than Claim 1.** An examiner could characterize the concept as scheduling/adapting work to a person's circumstances. The answer is the claimed persisted machine-state mechanism: separate Person State, frozen workstream record, stored operational constraint evaluation, preserved resume point, and state-dependent resumption. Specification drafting must describe this as runtime/execution-state continuity, not merely human productivity management.

## Claim 15

### Concrete claimed machinery

Claim 15 requires durable person-specific state stored separately from a first runtime's private conversation state; resolution of active namespace/workstream; generation of a handoff representation with required machine-readable fields; independent storage/transmission of that representation; supply to a second AI runtime; and reconstruction of the identified active workstream without requiring the first runtime's private conversation state.

### Technical effect

The claimed mechanism removes runtime/provider-local conversation state as a prerequisite for operational continuity. It serializes specified durable continuity state and uses that representation to reconstruct an identified workstream in another runtime. Dependent claims reinforce provider/device independence, permission-limited state transfer, and subsequent durable-state persistence.

### Eligibility conclusion

**PASS for filing-draft §101 posture.** Even if information transfer is abstracted at Prong One, the ordered combination is directed to a concrete cross-runtime state-transfer/reconstruction mechanism rather than communicating information for its own sake.

## Dependent claims

No dependent claim presently introduces an eligibility defect that negates the independent claim's practical-application posture. Several strengthen it, particularly machine-enforced budgets (3), lifecycle-state selection (4), provider-independent reconstruction (6, 16, 19), offline capture/reconciliation (7-8), concrete Person-State fields (10), correction/supersession processing (11), enumerated resume-package fields (14), permission-limited handoff (17-18), and post-reconstruction durable persistence (20).

## Drafting controls before filing

1. Specification should expressly identify the computer/runtime problems addressed: transcript-bound state, uncontrolled context growth, stale/current-state mixing, loss of resumable execution state, and provider/endpoint-local continuity loss — but only to the extent supported by frozen P1.
2. Tie asserted improvement to the mechanisms actually claimed: separate durable state and Person State, resource-bounded world-slice construction, resumable workstream checkpoints, machine-evaluable operational constraints, and serialized cross-runtime handoff/reconstruction.
3. Do not state that eligibility depends on novelty or unconventionality. Step 2A practical-application analysis is distinct from §§102/103.
4. Do not rely on “AI,” “computer,” “authorized human,” or physical endpoints standing alone as eligibility hooks.
5. Avoid characterizing the inventive core as a business workflow, personal assistant service, memory service, or human productivity method.
6. Preserve technical implementation explanation in the specification sufficient to support any asserted computer-functionality/technical improvement.

## Gate disposition

**§101 filing-draft gate: PASS for Claims 1, 9, and 15 and their current dependents, subject to final specification conformity.** This is not a prediction that no §101 rejection will issue. The strongest vulnerability is Claim 9 if its runtime-state mechanism is described too abstractly in the final specification. No claim amendment is presently justified solely by §101.

## Next filing-critical work

Proceed to adversarial §102/§103 searching and claim charts against the exact current combinations. Preserve adverse references and combination theories in `P1/MATERIAL_INFORMATION_REGISTER.csv`. Claim wording should remain frozen unless prior art or another filing-critical review exposes a concrete defect.