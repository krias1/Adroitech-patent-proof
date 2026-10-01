# Claim 5 Exact Frozen-P1 Support Control

**Claim:** Claim 5 — correction, supersession, preserved provenance, and later context suppression.  
**Parent:** Claim 1 — integrated runtime resolution.  
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16.  
**Boundary:** exact frozen P1 specification/drawings only. Later implementation evidence cannot enlarge this priority boundary.

## Operative added limitation

Claim 5 depends from Claim 1 and further requires receiving a correction to a stored interpretation, preserving the prior interpretation as provenance, marking or relating the prior interpretation as superseded, and reducing or excluding the superseded interpretation from a later current world slice unless historical context calls for the prior interpretation.

## Exact-frozen support finding — CONTROLLED

The frozen P1 discloses this correction lifecycle as a concrete state-management mechanism:

- The Brief Description of FIG. 7 states that a prior interpretation is preserved as provenance while a corrected state becomes active and future retrieval suppresses the superseded interpretation.
- Detailed Description §2 provides Correction objects and record fields including source references, current status, and historical status, supplying concrete stored-record structure for current-versus-historical state.
- Detailed Description §4 states that records may be historical or superseded and that reduced current relevance does not require deletion because records remain preserved for history and provenance.
- Detailed Description §8 states that, when a correction is received, the system may create a Correction object linked to the prior record, mark the prior record superseded or historical, update the active interpretation and dependent relevance, and prevent stale interpretation from repeated reintroduction while preserving history.
- Detailed Description §§9–10 make correction/supersession status a current-world-slice selection variable and expressly apply correction gates before emitting the bounded current world slice.

Together these passages support the complete added combination: correction receipt; retention of the prior interpretation; explicit correction/supersession relationship or status; reduced/suppressed later activation; and retained historical/provenance availability.

## Breadth fences

1. `stored interpretation` is limited to an interpretation represented in the disclosed durable person/world-state machinery; the claim does not reach every transient model thought or token-level intermediate state.
2. `preserving ... as provenance` means retaining the prior record/history/source relationship rather than deleting or silently overwriting it. It does not require a particular cryptographic provenance scheme.
3. `marking or relating ... as superseded` is supported by Correction objects, supersession status, historical status, and linked prior records. It is not a claim to arbitrary source-control/version-control systems.
4. `reducing or excluding` is selection/activation behavior. P1 does not require physical deletion of the superseded record and in fact teaches preservation of history.
5. `unless historical context calls for the prior interpretation` is bounded by P1's express preservation of historical records/provenance plus dynamic relevance/current-world-slice selection. It does not require superseded information to be reactivated in every historical query.
6. This control clears written-description/priority mapping only. It does not clear enablement, §101, §102, §103, §112(b), §112(f), inventorship, best mode, material-information, public-disclosure, drawing-wide QA, or final filing QA.

## Disposition

Claim 5 is **EXACT_FROZEN_P1_SUPPORT_CONTROLLED** for §112(a) written-description mapping and P1 priority, subject to Claim 1's parent limitations and all remaining independent statutory and filing gates.