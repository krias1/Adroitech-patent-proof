# Operative V2 Claim-Source Integrity — RESOLVED

**Date:** 2026-10-03  
**Anchor:** U.S. Provisional Application No. 64/155,744  
**Status:** SOURCE-INTEGRITY BLOCKER RESOLVED / OTHER FILING GATES REMAIN

## Resolution

The previously reported inability to retrieve the operative V2 claim artifact was a search/indexing failure, not loss of the canonical claim source.

The exact canonical source is presently retrievable on the default `main` branch at:

`krias1/Adroitech-Logic-Core/AdroitechLogic/Projects/Adroitech Logic Core Product/IP/Patent Workspace/NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`

Current Git blob SHA:

`1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`

The same byte-identifiable blob is directly retrievable through the Git blob endpoint. The path history shows commit `5128cc779fca92e9d1dd57bc8a5993764f3473ff` (`patent: narrow Claim 1 selection to P1-supported resource limit`) and predecessor `b91aa3d7bf3ed9b573eba828edc560b186f45a24` (`patent: propagate objective 112(b) cures into operative claim set`).

The recovered artifact itself states 20 total claims and 3 independent claims (1, 9, 15). Existing filing controls identify this same blob SHA as the operative source for the V2 §101 and prior-art reviews.

## Correction to prior blocker

`P1/2026-10-03_OPERATIVE_V2_SOURCE_INTEGRITY_BLOCKER.md` remains preserved as an audit record of the earlier failed search, but its factual blocker is superseded by this resolution. Do not treat the prior search miss as evidence that the operative claim source is absent.

## Filing consequence

The following work is unblocked:

- byte-identifiable claim-source reconciliation;
- final dependency / antecedent-basis QA against the exact V2 text;
- exact 20-total / 3-independent claim-count control;
- final claim/specification comparison;
- later DOCX generation and final-file hashing after substantive statutory gates pass.

This resolution does **not** itself mark the claim set final or the application READY. The V2 artifact expressly requires remaining §112(a), §112(b), §112(f), §101, §102, §103, inventorship, material-information, public-disclosure, specification, drawing, filing-paper, fee, and exact-file QA before filing.

## Undeniability rule

For all further V2 review, cite the full canonical path and blob `1658ecd4fe7664ae6fe6e83f9b58de4c0652eee0`. Search-index misses do not override direct Git object/path retrieval.