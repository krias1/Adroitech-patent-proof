# Adversarial Claim Chart — US 12,717,623 B1 vs. Operative Claim 15

**Review date:** 2026-10-02  
**Operative claim source:** `krias1/Adroitech-Logic-Core/.../NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`, blob `1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`  
**Reference:** US 12,717,623 B1, application 19/427,038, filed 2025-12-19, granted/published 2026-08-25, *Systems for and methods of context-preserving agent routing with thread-level context serialization*.  
**Status:** MATERIAL PRIOR-ART CANDIDATE / IDS REVIEW REQUIRED / NO ANTICIPATION CONCLUSION YET

## Why this reference matters

The reference is materially closer to operative Claim 15 than generic memory art. It expressly teaches a persistent serialized context object, transfer among software agents, durable storage, reconstruction/deserialization, policy/access constraints, workflow state/task metadata, and updates from agent outputs. Those concepts therefore must not be presented as the novelty of Claim 15 standing alone.

## Limitation chart

| Operative Claim 15 limitation | US 12,717,623 teaching | Adversarial result |
|---|---|---|
| Operating a first AI runtime using person-specific durable state stored separately from private conversation state of the first runtime | Persistent thread-level context object is stored durably and may contain conversational state, workflow variables, intermediate results, policy metadata and task dependencies. | **PARTIAL / PRESSURE.** Durable externalized state is taught. The reviewed disclosure does not facially establish the claimed separation of *person-specific durable state* from the first runtime's *private conversation state* as two distinct state classes. |
| Resolving an active person-specific namespace and an active workstream | Reference associates context with a conversation thread and can store workflow state/task metadata. | **PARTIAL.** Thread/workflow association is taught; no reviewed teaching establishes resolution of both a person-specific namespace and an active workstream in the claimed sense. |
| Generating a handoff representation containing at least person/namespace ID, resolved entity ID(s), current Person State, workstream ID, and workstream resume point | Serialized context representation may include conversational state, intent, intermediate results, task metadata, policy constraints, timestamps/versioning and other state, and is transferable among agents. | **STRONG PARTIAL / KEY GAP.** Generic serialization and task metadata are taught. The mandatory claimed field combination was not found in the reviewed reference, particularly resolved entity identifiers + separately maintained current Person State + workstream resume point. |
| Additional state selected according to permission or resource-selection criterion | Policy constraints/access limitations are expressly taught; portions of context may be provided to selected agents. | **TAUGHT/PRESSURE.** Do not rely on generic permission-scoped context transfer as distinguishing. Resource-selection criterion requires separate mapping. |
| Storing or transmitting the handoff independently of private conversation state of first runtime | Serialized context can be persisted and transmitted across process boundaries and remote execution environments. | **PARTIAL / PRESSURE.** Independent persistence/transmission is taught; independence from the first runtime's *private conversation state* as claimed remains a factual distinction requiring exact mapping. |
| Supplying handoff representation to a second AI runtime | Context object is supplied/shared among selected software agents, including remote environments. | **TAUGHT/PRESSURE.** Generic cross-agent supply is not distinguishing. |
| Reconstructing at second runtime the identified active workstream from handoff without requiring private conversation state of first runtime | Serialized context is reconstructed/deserialized so subsequent agent operations use coherent state. | **STRONG PARTIAL / PRESSURE.** Reconstruction is taught. The reviewed disclosure does not facially establish reconstruction of the specifically identified active workstream from the claimed field set *without requiring the first runtime's private conversation state*.

## §102 assessment

On the reviewed record, **do not assert anticipation** of operative Claim 15 by this reference alone. Several high-level mechanics are plainly taught, but the presently identified gaps are substantive: the claimed separation of durable person-specific state from runtime-private conversation state; active person-specific namespace resolution; the mandatory handoff field combination (person/namespace identifier + resolved entity identifier(s) + current Person State + workstream identifier + resume point); and transcript/private-conversation-independent reconstruction of that identified workstream.

This is a provisional legal/technical assessment for drafting control, not a final patentability opinion. Full text and prosecution history should be checked before any filing representation about novelty.

## §103 combination pressure

**HIGH.** MI-0004 supplies stateful AI workflow checkpoint/rehydration/provider abstraction; MI-0006 supplies cross-device workflow persistence plus changing user-state/context behavior; US 12,717,623 supplies serialized persistent context transfer/reconstruction among agents with policy constraints. A predictable-combination argument can therefore attack much of Claim 15's architecture.

The strongest presently visible resistance is not generic persistence, serialization, handoff, permission scope, provider independence, or reconstruction. It is the *specific integrated state model and required handoff semantics*: person-specific durable state separate from runtime-private conversation state; resolved namespace/entity identity; separately current Person State; identified resumable workstream and resume point; and reconstruction of that workstream without the originating private conversation state.

That combination must now be tested against additional pre-P1 references rather than assumed nonobvious.

## Filing control

1. Add/reference this document from `P1/MATERIAL_INFORMATION_REGISTER.csv` as MI-0008.
2. Preserve US 12,717,623 for IDS/materiality review.
3. Do not draft the specification as though serialization, persistent context, cross-agent handoff, access-scoped context, or deserialization/reconstruction are themselves the inventive advance.
4. Keep Claim 15 unchanged for now; this reference alone does not justify deleting the narrower mandatory field/separation limitations.
5. Next search should target the missing combination directly: person/user namespace + entity resolution + dynamic/current user operational state + resumable workflow checkpoint + transcript-independent cross-runtime reconstruction.
