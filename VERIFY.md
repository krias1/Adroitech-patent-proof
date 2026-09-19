# Verification Guide

This repository is designed so a third party can independently reproduce the evidence chain.

## Verify one source artifact

Example: first foundational archive.

```bash
git clone https://github.com/krias1/Adroitech-Logic-Core.git
cd Adroitech-Logic-Core
git checkout 1cb4465c7287ad732e627781df33636eb9d20589

git rev-parse HEAD
git hash-object "AdroitechLogic/Canonical Concepts/Adroitech OS Logic Core Archive.md"
sha256sum "AdroitechLogic/Canonical Concepts/Adroitech OS Logic Core Archive.md"
wc -c < "AdroitechLogic/Canonical Concepts/Adroitech OS Logic Core Archive.md"
```

Expected values for that exact source snapshot:

- Git commit: `1cb4465c7287ad732e627781df33636eb9d20589`
- Git blob SHA-1: `b9c327c7f7aa7acea747e50e6acd44fb975745dd`
- SHA-256: `320cf5a9f5281d2dd226cda6d57d5b0a358e3e3a29a3eb46eb61d6af577a644c`
- byte length: `3027`

## Verify proof records

The machine-readable proof ledger is:

`data/proof_records.jsonl`

Each line is one independent concept-level proof record. Multiple records may point to the same source bytes because a single artifact can evidence many distinct concepts.

The coverage ledger is:

`coverage/ledger.csv`

Coverage status is deliberately separate from proof count. A source is not marked historically complete until its origin, all relevant touches, successor relationships, and any exclusions have been checked.

## Provenance classes

- `git_verified`: Git independently establishes the commit/path/blob fact.
- `source_stated`: the source itself states a date, place, title, origin, or other historical fact; this is not silently promoted to Git proof.
- `derived`: reproducibly computed from verified inputs.
- `inference`: analyst interpretation; never presented as a source fact.

## Important limitation

A SHA-256 digest proves exact-byte identity against the bytes being checked. Git history provides repository chronology. Neither one, standing alone, proves legal inventorship, authorship, patent priority, novelty, non-obviousness, or ownership.

The value of this repository is the combination of:

1. immutable source references;
2. exact-byte hashes;
3. Git chronology;
4. granular concept extraction;
5. explicit fact/inference separation;
6. preserved corrections and successor relationships;
7. reproducible public review.

## Adversarial review expectation

A reviewer should assume nothing and reproduce everything possible. If a record cannot currently be independently reproduced, it must carry an explicit uncertainty or incomplete status rather than being upgraded by narrative confidence.
