# Operative V2 Claim-Source Integrity Blocker

**Date:** 2026-10-03  
**Anchor:** U.S. Provisional Application No. 64/155,744  
**Status:** FILING-CRITICAL BLOCKER / SOURCE INTEGRITY

## Finding

The filing controls identify the operative claim source as `krias1/Adroitech-Logic-Core/.../NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`, and the proof repository contains analyses that state they reviewed that V2 text. On the current default branch of `krias1/Adroitech-Logic-Core`, however, repository code search does not locate a file named `NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md` or the exact named source.

This is not proof that the V2 text never existed. It is proof that the filing record currently lacks a directly retrievable canonical claim-source path on the stated source repository/default branch. A filing-grade packet cannot depend on an ellipsis path or on secondary summaries of claim wording.

## Consequence

Until cured, do not mark the following final gates PASS based solely on the secondary V2 controls:

- final claim freeze;
- word-for-word §112(b) claim/specification comparison;
- final dependency and antecedent-basis QA;
- exact claim count / independent-claim count certification;
- final DOCX generation and hashing;
- zero-reconstruction upload packet.

The existing V2 analyses remain useful evidence of prior review, but they are not a substitute for preserving the exact operative claims as a canonical source artifact.

## Required cure

1. Locate the exact V2 claim text that was reviewed.
2. Preserve it at a stable canonical path in `krias1/Adroitech-Logic-Core` (or identify the existing stable path if search indexing/path assumptions were wrong).
3. Record its Git commit SHA and blob SHA.
4. Compare that exact text against the claim text used by the V2 §112(b), P1-support, §101, prior-art, dependency/antecedent, and claim-readiness controls.
5. If any wording differs, rerun the affected limitation-level reviews; do not silently treat the secondary summaries as the final claim text.
6. Freeze the final filing claim artifact only after that reconciliation, then compute the final file hash/byte length during exact-file QA.

## Undeniability rule

For filing purposes, the operative claims must be reproducible byte-for-byte from a named source artifact. A review record saying what a claim contained is not the claim itself.
