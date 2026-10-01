# Claims 7–8 — Exact Frozen-P1 Support Control

## Scope
This control addresses only §112(a) written-description mapping and entitlement to the Sep. 16, 2026 P1 priority boundary for candidate Claims 7 and 8. It does not clear enablement, §101, §102, §103, §112(b), §112(f), inventorship, best mode, material-information/public-disclosure, drawing, or final filing QA.

## Canonical claim limitations

### Claim 7
Claim 7 depends from Claim 1 and requires: (1) current input comprising a machine-readable physical-world identifier; (2) capture by an enrolled endpoint; (3) resolution of the identifier to an entity in the person-specific namespace; and (4) persistence of an asset-related material state change with operator or endpoint provenance.

### Claim 8
Claim 8 depends from Claim 7 and requires: (1) capture of the asset-related material state change while the enrolled endpoint lacks network connectivity; and (2) subsequent reconciliation with authoritative durable state when connectivity becomes available.

## Frozen-P1 written-description mapping
The frozen Sep. 16 specification expressly discloses an enrolled mobile/rugged endpoint as a persistent field interface, including operator and endpoint identity authentication, physical identifier readers, and a durable-state interface. It further discloses that endpoint state can include network reachability and scanner/camera/NFC availability.

For Claim 7, the frozen specification's physical-asset flow expressly teaches capture of QR, barcode, NFC, camera-derived, typed, serial-number, asset-tag, or other physical identifiers; resolution to an Entity object within an authorized person/business namespace; receipt of an asset material update; attachment of operator/device identity and provenance; and write of the material change to authoritative durable state. The enrolled-endpoint provenance mechanism is also expressly described as permitting later reconstruction of which enrolled endpoint generated a change.

For Claim 8, the frozen specification expressly teaches that when connectivity is unavailable the endpoint may queue material changes with target entity, proposed change, operator identity, endpoint identity, timestamp, permission scope and provenance. When connectivity returns, the reconciliation engine compares queued changes with current durable state and may commit, merge, apply an authority rule, preserve versions, or request narrow conflict resolution. A reconciliation receipt may identify authoritative pre-state and accepted post-state.

## Breadth controls
1. `machine-readable physical-world identifier` is controlled by the filed physical-identifier-reader/asset-resolution embodiment. It must not be expanded to an arbitrary abstract identifier unrelated to a physical entity or field capture.
2. `enrolled endpoint` is tied to the filed authorized mobile/rugged endpoint and endpoint-identity architecture; this control does not imply every generic client device is enrolled.
3. Claim 7's provenance is satisfied by operator **or** endpoint provenance as claimed; the frozen disclosure supports attaching both, but the claim must not be represented as requiring both unless amended.
4. Claim 8's offline behavior concerns queued **material state changes**, not a claim that the entire AI/runtime necessarily performs all inference offline.
5. `reconciled with authoritative durable state` is controlled by the filed queue/reconciliation mechanism. It does not require blind last-write-wins behavior and does not imply every queued change must be accepted unchanged.
6. Later implementation receipts may corroborate reduction to practice but are not used to backfill P1 priority.

## Control conclusion
Claims 7 and 8 have direct frozen-P1 written-description support for their recited combinations and may be marked `EXACT_FROZEN_P1_SUPPORT_CONTROLLED` for §112(a) written description and P1 priority, subject to the breadth controls above. Figure support and all other statutory/filing gates remain separately open until independently cleared.
