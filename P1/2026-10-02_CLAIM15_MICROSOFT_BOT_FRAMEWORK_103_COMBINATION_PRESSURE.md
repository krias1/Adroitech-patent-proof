# Claim 15 — Microsoft Bot Framework §103 Combination Pressure

Date: 2026-10-02
Status: ADVERSARIAL PRIOR-ART CONTROL / NOT A CONCLUSION OF INVALIDITY
Operative claim source: krias1/Adroitech-Logic-Core `NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`, blob `1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`.

## Material finding

Pre-P1 Microsoft Bot Framework state-management teachings materially weaken any attempt to distinguish operative Claim 15 merely on the proposition that person/user state is stored separately from conversation-private state.

Public Bot Framework materials predating P1 describe three separately keyed state scopes: User State, Conversation State, and Private Conversation State. User State persists for a user across conversations on a channel; Private Conversation State is scoped to the particular user and conversation. Durable storage implementations include Blob/Cosmos/Azure storage. Bot Framework also had cross-channel/agent handoff architecture. Accordingly, the general architectural idea of durable user-specific state existing separately from conversation/private-conversation state is old and should not be presented as the novelty center.

## Operative Claim 15 pressure map

Claim 15 limitation | Bot Framework pressure | Present assessment
---|---|---
first AI runtime | conversational bot/runtime | taught generally
person-specific durable state | User State persisted via durable storage | materially taught
stored separately from private conversation state | distinct User State and Private Conversation State scopes/keys | materially taught
resolve active person-specific namespace | user/channel identity keys exist, but P1 namespace/entity-resolution mechanism not shown by this evidence | gap remains
resolve active workstream | dialog/conversation state exists; exact independently resumable active-workstream construct not established here | partial only
handoff person/namespace identifier | handoff/user/channel identifiers create pressure | partial
resolved entity identifiers | not established by this evidence | gap remains
current Person State | ordinary user/profile state is not the claimed current operational Person State mechanism | gap remains
workstream identifier + resume point | dialog state creates pressure; exact required handoff pair not established here | partial
permission/resource-selected additional state | access/scoping concepts exist; exact claimed selection combination not established here | partial
store/transmit independently of first runtime private conversation state | separate state scopes plus handoff create combination pressure | partial/material
second AI runtime | bot/agent handoff concepts create pressure | partial/material
reconstruct identified active workstream without first runtime private conversation state | not established as the full claimed reconstruction combination by this evidence | principal gap

## §103 consequence

This finding materially strengthens the combination case already created by the preserved serialized-context/handoff and cross-device-resume references. A plausible examiner combination can now source: (1) durable user state separated from conversation/private-conversation state from Bot Framework; (2) serialized cross-agent context transfer/reconstruction from MI-0008; and (3) cross-device activity/resume-point continuity from MI-0009.

Therefore Claim 15 should not rely for nonobviousness on any one of these generic concepts: persistent user state, separation from conversation state, handoff, serialization, device change, or resume point. The defensible center must remain the integrated P1-supported combination, particularly active person-specific namespace/entity resolution + current operational Person State + identified resumable workstream + mandatory handoff fields + reconstruction of that workstream at a different AI runtime without requiring the originating runtime's private conversation state.

## Filing action

No amendment is justified from this source family alone. Preserve the source family as material-information / §103 combination evidence and continue searching for a single pre-P1 reference or tighter two-reference combination that supplies the remaining namespace/entity-resolution + operational-Person-State + resumable-workstream reconstruction elements.

Do not characterize Microsoft Bot Framework as anticipating Claim 15 on the present evidence.