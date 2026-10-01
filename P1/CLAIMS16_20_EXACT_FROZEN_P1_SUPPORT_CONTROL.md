# Claims 16–20 Exact Frozen-P1 Support Control

**Parent:** Claim 15 — provider-independent handoff.  
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16.  
**Boundary:** exact frozen P1 specification/drawings only. Later implementation evidence cannot enlarge this priority boundary.

## Operative added limitations

- **Claim 16:** first and second runtimes use different model providers, or one runtime is local and the other remotely hosted.
- **Claim 17:** handoff further contains at least one correction record, source-provenance record, permission scope, evidence-confidence value, or do-not-repeat state.
- **Claim 18:** permission scope causes the second runtime to receive less than all person-specific durable state available to the first runtime.
- **Claim 19 (canonical wording after narrowing):** responsive to a device change, the second AI runtime executes on another authorized endpoint and reconstructs operational context from provider-independent durable state rather than treating endpoint-local state as authoritative.
- **Claim 20:** after reconstruction, a material state change produced by the second runtime is persisted to person-specific durable state so a subsequent authorized runtime receives updated state.

## Exact-frozen support findings

### Claim 16 — CONTROLLED
P1 §12 expressly states a handoff may occur when a **provider changes** or **device changes**, and a second authorized runtime reconstructs without the original transcript. P1's system embodiment further permits components across local and remote machines and identifies the inference engine as local, hosted, distributed, or replaceable. Claim 16 is supported if kept to those disclosed runtime/provider deployment alternatives; do not broaden `provider` into every unrelated service-provider relationship.

### Claim 17 — CONTROLLED
P1 §12's example handoff package expressly includes `corrections`, `evidence`, `permissions`, and `do_not_repeat`. P1 §8 expressly attaches source identity, timestamps, confidence, permission scope, and supersession status to material records. Accordingly the recited alternatives are directly disclosed individually and in the continuity-state architecture. `source-provenance record` should remain tied to the filed source/source_refs/provenance machinery rather than an undefined generic audit record.

### Claim 18 — CONTROLLED
P1 §8 states that permission filtering can operate **before information is placed into the current world slice**, and that shared objects may coexist with restricted subgraphs **without automatically exposing them to every runtime or user**. P1 §10 retrieves required permission records and applies permission gates before emitting the bounded world slice. This supports a permission-scoped handoff in which the receiving runtime receives less than all available person-specific durable state. Avoid implying that every implementation must disclose the existence or count of withheld records.

### Claim 19 — CONTROLLED AFTER CANONICAL NARROWING
The earlier candidate wording recited a replacement endpoint `enrolled after loss, replacement, or retirement of a first endpoint`; that complete lifecycle was not established by the frozen P1 and was therefore rejected for priority purposes. The canonical claim was subsequently narrowed to the supported architecture: **responsive to a device change**, the second runtime executes on **another authorized endpoint** and reconstructs operational context from **provider-independent durable state rather than treating endpoint-local state as authoritative**.

That narrowed combination is supported by the frozen disclosure: P1 §12 expressly contemplates `device changes` and reconstruction by a second authorized runtime; the mobile/rugged endpoint has a durable-state interface to the customer-controlled store; third-party/platform-local state is subordinate rather than root authority; material changes are written to authoritative durable state; and updated state becomes available to other authorized interfaces. The rejected `loss, replacement, or retirement` enrollment lifecycle remains outside the P1 priority boundary and must not be reintroduced as though entitled to P1 priority.

### Claim 20 — CONTROLLED IN COMBINATION
P1 §11 says that after inference or action the system identifies material changes and writes them back, including completed work, blockers, corrections, evidence, entity resolution, checkpoints, and Person State transitions. P1 §12 establishes second-runtime reconstruction; §18 states that a material change is written to authoritative durable state and made available to other authorized interfaces. Read together, the filed disclosure supports the continuity loop recited by Claim 20. Keep `subsequent authorized runtime receives the updated state` tied to authorized-interface/runtime retrieval of the authoritative durable state; do not imply unsolicited push delivery if not otherwise disclosed.

## Disposition

Claims **16, 17, 18, 19, and 20** now have exact-frozen-P1 written-description/priority support controlled, subject to their separate enablement, §101, §102/§103, §112(b)/(f), inventorship, best-mode, disclosure/candor, drawing and final-QA gates.

For Claim 19, clearance applies only to the **narrowed canonical wording**. The rejected endpoint-loss/replacement/retirement enrollment lifecycle is expressly excluded from the P1 priority boundary unless independently claimed as later matter without P1-priority attribution.