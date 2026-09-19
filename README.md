# Adroitech Patent Proof Repository

Public, reproducible evidence repository for the historical development of Adroitech Logic Core, Adroitech OS, its ethical runtime architecture, human-integration methods, skills, teaching practices, sovereignty mechanisms, correction patterns, and potentially patent-relevant implementation concepts.

## Purpose

This repository exists so a technically competent third party can independently inspect the source evidence, reproduce hashes, follow Git chronology, distinguish verified facts from interpretation, and challenge any conclusion without depending on private notes or trust in a summary.

It is an evidence corpus, not a claim that a hash by itself proves legal inventorship, patent priority, authorship, ownership, validity, novelty, or non-obviousness. Those are separate legal or scientific questions. The repository preserves and organizes evidence relevant to those questions.

## Canonical source

Source repository:

`https://github.com/krias1/Adroitech-Logic-Core`

Proof repository:

`https://github.com/krias1/Adroitech-patent-proof.`

The trailing period is part of the GitHub repository name.

## Evidence rules

Every proof record should preserve, where available:

1. Stable proof ID.
2. Exact source path.
3. Source commit SHA.
4. Git blob SHA.
5. Independent SHA-256 of the exact retrieved bytes.
6. Exact byte length.
7. Origin commit SHA and UTC author/committer timestamps.
8. Latest-touch commit and timestamp when different.
9. Commit message.
10. Source-stated historical date/time/place only when explicitly present.
11. Provenance classification separating:
   - `git_verified`
   - `source_stated`
   - `derived`
   - `inference`
12. Exact concept atom.
13. Ethical significance.
14. Teaching-method significance.
15. IP / implementation significance.
16. Relationships to earlier and later evidence.
17. Reproduction instructions.
18. Uncertainty, conflict, omission, or missing support.

## Non-negotiable provenance discipline

- Git SHA values and SHA-256 digests are not interchangeable.
- A source-stated historical date is not silently promoted to a Git-verified date.
- An inference is never recorded as a source fact.
- No missing date, place, motive, authorship claim, or event context is invented.
- One source file may generate many proof atoms.
- Every processed source is entered in the coverage ledger.
- Every intentional exclusion is logged with a reason.
- Corrections append provenance; they do not silently erase earlier evidence.
- Evidence records should be reproducible from public source commits whenever possible.

## Repository layout

```text
README.md
SCHEMA.md
VERIFY.md
data/
  proof_records.jsonl
  proof_records.csv
coverage/
  ledger.csv
records/
  000000-000999/
receipts/
```

## Scientific / adversarial review standard

The corpus is designed for hostile verification, not persuasion. A reviewer should be able to ask:

- What exact bytes existed?
- At what Git commit?
- When does Git actually establish their presence?
- Is an earlier date merely stated inside the source?
- What is directly supported by the source?
- What is interpretation?
- What later artifact develops the same idea?
- Can the digest be reproduced?
- Can the source commit be checked out?
- Are contradictions and revisions preserved?

If the repository cannot answer those questions for a record, the record is incomplete.

## Status

Long-running chronological extraction is in progress from the earliest available Adroitech Logic Core evidence forward. The target is comprehensive concept-level coverage, not a small curated sample.
