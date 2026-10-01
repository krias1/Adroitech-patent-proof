# Claim 15 Exact Frozen-P1 Support Control

**Claim family:** Claim 15 — Provider-independent handoff (independent); Claims 16–20 dependent.  
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16.  
**Frozen specification:** `AdroitechLogic/01_ADROITECH_OS_PROVISIONAL_SPECIFICATION_2026-09-16.pdf`, SHA-256 `267628A51CC938DBCBD724AF4F7F9B0A1AD58532F32B738B12A36490C2CFF00E`.  
**Frozen drawings:** `AdroitechLogic/02_ADROITECH_OS_PROVISIONAL_DRAWINGS_2026-09-16.pdf`, SHA-256 `D27C4FE6FD3D39CACB15C3268DCB74BC8A31E2AE96474A04336D3439E55CD9E5`.  
**Status:** EXACT_FROZEN_P1_SUPPORT_CONTROLLED for Claim 15 written-description/priority mapping; enablement, §101, §102/§103, §112(b)/(f), inventorship, best mode, material-information, public-disclosure, drawings-wide QA, and final filing QA remain separate gates.

## Operative Claim 15

A computer-implemented method for transferring person-specific operational continuity between artificial-intelligence runtimes, comprising:

1. operating a first artificial-intelligence runtime using person-specific durable state stored separately from private conversation state of the first artificial-intelligence runtime;
2. resolving an active person-specific namespace and an active workstream;
3. generating a bounded handoff representation comprising at least a person or namespace identifier, one or more resolved entity identifiers, current Person State, a workstream identifier, and a workstream resume point;
4. storing or transmitting the bounded handoff representation independently of the private conversation state of the first artificial-intelligence runtime;
5. supplying the bounded handoff representation to a second artificial-intelligence runtime; and
6. reconstructing, at the second artificial-intelligence runtime, operational context sufficient to resume the active workstream without requiring the private conversation state of the first artificial-intelligence runtime.

## Exact frozen-P1 limitation chart

| Claim 15 limitation | Exact frozen-P1 support | Disposition / breadth control |
|---|---|---|
| first AI runtime uses person-specific durable state separately from private conversation state | Spec p.2 Summary: material state is persisted in customer-controlled durable representation so another authorized runtime/provider can reconstruct without original conversation. Spec p.4 DD §1: person-specific context is maintained independently from any one AI model's internal weights or conversation context and may reside in customer-controlled storage. | **DIRECT.** `private conversation state` should be construed/drafted consistently with the filed concepts `conversation context` / `original conversation history`; do not broaden this into every form of provider-private internal state. |
| resolve active person-specific namespace and active workstream | Spec p.2 Summary: resolves active person namespace; Context VM records are independently resumable workstreams. Spec p.4 DD §2: identifies active person/role and resolves referenced entities in active person's namespace. Spec p.5 DD §6: Context VM is bounded workstream/mission and input may be bound to a Context VM. | **DIRECT in combination.** P1 uses `Context VM` as the workstream construct; avoid implying an undisclosed generic provider session identifier. |
| bounded handoff representation containing person/namespace ID, resolved entity IDs, current Person State, workstream ID, resume point | Spec p.3 definition of Current World Slice: bounded subset/summary/representation/subgraph/record set/serialized context package. Spec p.5 DD §6: Context VM includes identifier and exact resume point. Spec p.5 DD §8: bounded current world slice may include identity information, resolved entity records, Person State fields and active Context VM resume state. Spec p.6 DD §12: serialized state package may include person identifier, resolved entities, Person State and Context VM state. | **DIRECT/NECESSARILY COMBINED.** P1 does not use the exact phrase `bounded handoff representation`; support comes from the disclosed bounded serialized context/state-package machinery. Keep the claim tied to that machinery rather than an arbitrary message between models. |
| store or transmit handoff representation independently of first runtime private conversation state | Spec p.2 Summary: durable representation reconstructable by another runtime/provider without original conversation. Spec p.4 DD §1: context stored independently from model conversation context. Spec p.6 DD §§12–13: first runtime serializes state package; customer-controlled serialized model/durable store remains portable and model is replaceable. | **DIRECT.** The filed disclosure establishes independent durable/serialized state and cross-runtime portability; avoid claiming that no conversation-derived information can ever contribute to the state package. |
| supply representation to second AI runtime | Spec p.2 Summary: representation can be used by another authorized AI runtime/model/session/device/endpoint/provider. Spec p.6 DD §12: second AI runtime may ingest the package. | **DIRECT.** |
| second runtime reconstructs operational context sufficient to resume active workstream without first private conversation state | Spec p.2 Summary: another runtime/provider can reconstruct person-specific operational state without original conversation. Spec p.5 DD §11: resume operation retrieves Context VM checkpoint, exact resume point and supplies bounded resume package to current AI runtime. Spec p.6 DD §12: second runtime ingests package and continues operation without original conversation history. | **DIRECT in combination.** `sufficient to resume` is supported by the resume-package/continue-operation disclosure; final §112(b) review should retain an objective workstream/checkpoint boundary. |

## Frozen drawing reconciliation — FIG. 6

Frozen drawings p.7, FIG. 6 expressly depicts `AI Runtime A / Provider A` connected through `230 Handoff Interface` to `210 Customer-Controlled Durable State`, whose listed contents include `person namespace`, `person state`, `context VM`, `corrections`, and `evidence`; a second `230 Handoff Interface` connects that durable state to `AI Runtime B / Provider B`, followed by `Reconstruct Current World Slice`. The figure caption states: `Provider-independent serialization and reconstruction of person-specific continuity state.`

FIG. 6 therefore corroborates the cross-provider transfer architecture and the reconstruction side of Claim 15. It does **not**, standing alone, establish every textual field in the Claim 15 handoff representation; those fields are supplied by frozen specification pp.5–6 as charted above.

## Priority/breadth findings

1. **Provider independence is actually in P1.** The frozen text and FIG. 6 both disclose cross-provider continuity, and p.6 says the AI model is replaceable while accumulated operational context remains portable.
2. **Transcript independence is actually in P1, but use the filed boundary.** P1 repeatedly states reconstruction/continuation without the `original conversation` or `original conversation history`, and separately maintains person context from model `conversation context`. This supports Claim 15's architecture. It does not support a categorical rule that serialized state can never contain facts originally learned from conversation.
3. **The bounded handoff is a disclosed combination, not a magic phrase.** P1 discloses a bounded serialized current-world/context representation, a state package with person/resolved-entity/Person-State/Context-VM content, and Context VM exact resume points. Claim drafting should preserve that concrete combination.
4. **Resume sufficiency must remain technical.** Tie it to workstream identity/checkpoint/resume state and reconstruction of operational context; do not substitute a subjective assertion that a model merely `understands` the user.
5. **No later matter was used to establish P1 support.** This control relies on the exact frozen specification and frozen FIG. 6. Later implementation evidence may corroborate reduction to practice but cannot expand this priority boundary.

## Dependent claims

This control clears only the Claim 15 support mapping. Claims 16–20 inherit Claim 15 but each added limitation still requires its own exact-frozen-P1 support and breadth review before receiving priority clearance.

## Remaining gates

Claim 15 is **not filing-ready merely because its P1 support mapping is controlled**. Remaining review includes enablement commensurate with breadth; §101 technical-effect framing; element-level §102/§103 and combination analysis; §112(b) review of `bounded handoff representation`, `private conversation state`, and `operational context sufficient to resume`; §112(f) review; inventorship; best mode; material-information/public-disclosure review; final drawing consistency; and exact-file filing-package QA.
