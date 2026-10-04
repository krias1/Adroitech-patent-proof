# §101 Statutory-Category Gate — Operative 20-Claim Set

**Date:** 2026-10-04  
**Anchor:** U.S. Provisional Application No. 64/155,744  
**Exact operative claim source:** `krias1/Adroitech-Logic-Core/AdroitechLogic/Projects/Adroitech Logic Core Product/IP/Patent Workspace/NONPROVISIONAL_OPERATIVE_CLAIMS_V2_2026-10-02.md`  
**Operative claim blob:** `49fefff7d2d241b2d74e93a567ffbf47f6e6f63c`  
**Claim surface:** 20 total / 3 independent (1, 9, 15)  
**Disposition:** PASS_EVIDENCE / FINAL-TEXT QA PENDING

## Question controlled

This control addresses only Step 1 of the USPTO §101 subject-matter-eligibility analysis: whether each operative claim is to a statutory category. It does not resolve Alice/Mayo Step 2A or Step 2B, utility, novelty, nonobviousness, disclosure, definiteness, inventorship, or priority.

## Current authoritative rule

USPTO MPEP §2106 states that 35 U.S.C. §101 recognizes four statutory categories: process, machine, manufacture, and composition of matter. MPEP §2106.03 explains that a process defines actions or a series of acts and that 35 U.S.C. §100(b) makes `process` synonymous with `method` for this purpose.

Authoritative controls:
- https://www.uspto.gov/web/offices/pac/mpep/s2106.html
- https://www.uspto.gov/web/offices/pac/mpep/s2104.html

## Exact operative-claim audit

The exact controlled V2 claim text was re-read from the canonical repository.

- Claim 1 begins `A computer-implemented method comprising:` and recites a series of maintaining, receiving, resolving, selecting, constructing, supplying, and persisting acts. It is a process/method claim.
- Claims 2–8 each depend from Claim 1 and further limit that method. They remain process/method claims.
- Claim 9 begins `A computer-implemented method for preserving execution continuity across changing human operating conditions, comprising:` and recites a series of storing, placing, receiving, determining, selecting, obtaining, and resuming acts. It is a process/method claim.
- Claims 10–14 each depend from Claim 9 and further limit that method. They remain process/method claims.
- Claim 15 begins `A computer-implemented method for transferring person-specific operational continuity between artificial-intelligence runtimes, comprising:` and recites operating, resolving, generating, storing/transmitting, supplying, and reconstructing acts. It is a process/method claim.
- Claims 16–20 each depend from Claim 15 and further limit that method. They remain process/method claims.

No operative claim is drafted as data per se, a signal per se, a bare information compilation, or a machine-readable-medium claim whose broadest reasonable interpretation raises the transitory-signal category problem. No claim presently mixes statutory and nonstatutory categories at Step 1.

## Adversarial boundary

Passing statutory category does **not** establish overall §101 eligibility. Software methods may satisfy Step 1 and still require full judicial-exception analysis. The separate `P1/2026-10-03_SECTION101_TECHNICAL_EFFECT_CONTROL.md` remains controlling for the technical-effect/Step-2 analysis of independent Claims 1, 9, and 15.

Any later amendment that changes a claim from the current method form, adds a medium claim, or broadens a limitation to encompass a transitory signal requires this gate to be reopened.

## Filing disposition

**§101 statutory category: PASS_EVIDENCE / FINAL-TEXT QA PENDING for Claims 1–20.**

Before READY, compare the final filing claims byte-for-byte/limitation-for-limitation to the controlled operative source. If the final claim set preserves the present method categories, this gate can advance to final PASS without substantive re-analysis. Overall §101 eligibility remains separately unresolved.