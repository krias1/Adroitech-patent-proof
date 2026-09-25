# Active Tasks — Examiner Zero-Reconstruction / Historical Proof Mission

**Effective:** 2026-09-25  
**Primary filing anchor:** `P1-2026-09-16`  
**Canonical source repository:** `krias1/Adroitech-Logic-Core`  
**Proof repository:** `krias1/Adroitech-patent-proof`

## Mission override

The patent-proof repository is not a forward activity log and is not a monitor for whatever Adroitech builds next.

Its first patent mission is the **Undeniable Strategy** in its operational sense:

> know the questions an examiner or patent reviewer can ask, answer each question before it becomes a surprise, and put the exact evidence route directly in front of the reviewer so the record requires as little archaeology as possible.

"Undeniable" is the preparation strategy. It is not a claim that issuance is guaranteed.

The patent lane is therefore **question-first and backward-looking from P1**.

## Patent evidence cutoff

For technical/conception support of P1, the relevant event or source must predate the actual P1 filing moment on 2026-09-16.

A source may be discovered, indexed, hashed, or added to this repository later. That later ingestion date does not change the historical source date.

Post-P1 material is permitted in the patent lane only when it is one of these:

- a formal USPTO filing receipt, certified copy, or other procedural record about P1;
- a later verification of exact pre-P1 bytes, hashes, commit ancestry, timestamps, or source-system metadata;
- a later-created proof/index record whose underlying evidence is pre-P1;
- later-discovered prior art whose own public-availability date is relevant to the effective filing date.

Do **not** use post-P1 technical development as if it proves what P1 disclosed, what existed before filing, or what deserves the P1 priority date.

Do **not** continuously ingest new Adroitech product work into this proof repo merely because it is new.

## Priority 1 — Examiner question database

Canonical front door:

- `P1/EXAMINER_FRONT_DOOR.md`
- `P1/EXAMINER_QUESTION_MATRIX.csv`

Every examiner-facing question gets:

1. a stable question ID;
2. controlling authority;
3. current answer status;
4. current answer/evidence route;
5. exact repository path/proof IDs when available;
6. missing answer;
7. next extraction or filing action.

The scraper/reviewer works from OPEN/PARTIAL rows first.

## Priority 2 — Fill answers from historical evidence

For each OPEN/PARTIAL examiner question:

1. search the pre-P1 source universe;
2. recover exact source identity and chronology;
3. create/update proof atoms;
4. update `P1/P1_SUPPORT_MATRIX.csv`;
5. update the examiner matrix;
6. update the material-information/prior-art register when needed;
7. record source disposition in coverage.

The goal is not "more files." The goal is fewer unanswered examiner questions.

## Priority 3 — Professional dossier extraction

During the same historical source pass, extract professionally relevant evidence into:

- `DOSSIER_EVIDENCE_MAP.csv`
- `PROFESSIONAL_DOSSIER.md`

This is secondary to the patent examiner matrix.

## Priority 4 — Thesis extraction

During the same source pass, extract thesis/research evidence into:

- `THESIS/THESIS_EVIDENCE_MAP.csv`
- `THESIS/README.md`

This is secondary to the patent examiner matrix.

## Immediate patent gap queue

1. final claim set / limitation list;
2. exact limitation-by-limitation P1 support;
3. formal P1 filing-receipt reconciliation;
4. §101 technical-eligibility mapping for each independent claim;
5. §102 single-reference novelty charts;
6. §103 combination / reason-to-combine pressure tests;
7. §112(a) written-description and full-scope enablement maps;
8. §112(b) term boundaries / definiteness;
9. §112(f) algorithm/structure mapping where implicated;
10. human inventorship mapped to actual claim limitations;
11. pre-P1 public-disclosure / public-use / offer-for-sale audit;
12. material-information / IDS candidate register completion;
13. best-mode confirmation;
14. restriction/election risk across claim families;
15. filing-package controls: ADS benefit claim, claims, abstract, drawings, declaration, fees, format.

## Completion standard

The patent proof mission is ready for a patent professional only when a reviewer can move:

**examiner question -> answer -> claim/limitation -> P1 coordinate -> pre-P1 proof -> exact source -> provenance -> prior-art response -> gap/action**

without rebuilding the history from memory.

A row may remain OPEN. It may not remain hidden.
