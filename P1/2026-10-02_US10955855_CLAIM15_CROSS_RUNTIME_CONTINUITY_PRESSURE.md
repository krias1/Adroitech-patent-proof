# US 10,955,855 B1 — Claim 15 Cross-Runtime / Resume-Point Adversarial Pressure

Date reviewed: 2026-10-02
Operative claim source: krias1/Adroitech-Logic-Core blob `1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`
Priority boundary: frozen P1 filed 2026-09-16
Status: MATERIAL-INFORMATION CANDIDATE / ADVERSE COMPONENT REFERENCE / NO ANTICIPATION CONCLUSION

## Reference

US 10,955,855 B1, **Smart vehicle**, application 16/693,285, filed 2019-11-23, published/granted 2021-03-23. Public patent text reports a method for providing information or entertainment content for a person in which operation moves from a car environment to a building environment, a speech recognizer is transferred along with a current play state, and content resumes on a device in the building without interruption. The disclosure further states that transferred data may include a resume point for texting, social-network communication, email, chat, a word processor, a software application, augmented reality, or virtual reality, and describes alteration of system response based on detected human emotion/drowsiness/fatigue.

## Why this matters

This reference predates P1 by years and is adverse to any attempt to characterize **cross-device transfer of a person's current activity plus a resume point, followed by continuity on another device/environment**, as novel by itself. It also supplies older component teaching for adapting machine behavior to detected human state. It therefore increases §103 pressure when combined with AI-runtime/state references already preserved in MI-0004, MI-0006, and MI-0008.

It does **not** on the reviewed record facially anticipate operative Claim 15 as a whole.

## Operative Claim 15 limitation pressure

| Claim 15 limitation | US 10,955,855 B1 pressure | Adversarial assessment |
|---|---|---|
| operating a first AI runtime using person-specific durable state stored separately from private conversation state | Transfers person-associated activity/play state between environments; no reviewed teaching of the claimed AI-runtime/private-conversation-state separation | GAP remains |
| resolving an active person-specific namespace and an active workstream | Person/activity continuity is present, but no reviewed active namespace resolution and no claimed workstream-resolution architecture | GAP remains |
| handoff includes person/namespace identifier | Person-specific operation is inherent/contextual, but no reviewed mandatory serialized person/namespace identifier field | PARTIAL only |
| one or more resolved entity identifiers | No reviewed corresponding requirement | GAP remains |
| current Person State | Reference separately discusses detected human states and changing system response, but not the operative Claim 15 Person-State field in the handoff combination | COMPONENT PRESSURE; combination issue |
| workstream identifier | Transfers current activity/play state; no reviewed mandatory workstream identifier field | PARTIAL only |
| workstream resume point | Strong: expressly teaches transfer/resumption using current play state and describes resume points for multiple software/communication activities | STRONG COMPONENT TEACHING |
| additional state selected under permission/resource criterion | No reviewed corresponding selection requirement | GAP remains |
| storing/transmitting handoff independently of first runtime private conversation state | Transfer between car/building devices/environments is taught; independence from an AI runtime's private conversation state is not | PARTIAL only |
| supplying handoff to second AI runtime | Cross-environment/device transfer is taught, but not the claimed second AI runtime | PARTIAL only |
| reconstructing identified active workstream without first runtime private conversation state | Resume/continuation on another device is taught; reconstruction of an identified workstream from the recited handoff fields without private conversation state is not | PARTIAL only |

## §102 conclusion

No present anticipation conclusion. The reviewed disclosure does not establish the full operative Claim 15 combination, particularly the separation of person-specific durable state from runtime-private conversation state, active namespace/entity resolution, the mandatory multi-field handoff representation, permission/resource-scoped additional state, and transcript-independent reconstruction by a second AI runtime.

## §103 combination pressure

This reference materially weakens reliance on **device/environment transition + activity state + resume point + uninterrupted continuation** as a distinguishing concept. In an obviousness attack, an examiner could combine this old cross-device continuity teaching with:

- MI-0008 for serialized context objects, cross-agent transfer, reconstruction, workflow/task state and policy constraints;
- MI-0004 for stateful AI runtimes, serialized persistent state, checkpoint/suspend/rehydrate/resume and provider/backend abstraction; and
- MI-0006 for conversational-AI workflow persistence across devices plus user-state/behavior modeling that changes workflow behavior.

The strongest remaining Claim 15 defense must therefore be the **specific integrated architecture**, not generic handoff: active person-specific namespace resolution + resolved entity identifiers + current Person State + identified workstream/resume point + permission/resource-scoped additional state + person-specific durable state separated from runtime-private conversation state + reconstruction by another AI runtime without that private conversation state.

## Claim-drafting consequence

Do not amend Claim 15 from this reference alone. Do not argue that cross-device resume, transfer of current application state, or a resume point is independently inventive. Continue searching the remaining integrated field combination and test whether MI-0004 + MI-0006 + MI-0008 + this reference supplies a reasoned combination with predictable results.

## Candor / IDS control

Preserve as a material-information candidate. Formal IDS inclusion is a prosecution decision; do not suppress this reference merely because its strongest teachings are component-level rather than a facial anticipation of Claim 15.
