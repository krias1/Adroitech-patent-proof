# Adroitech Patent Proof Repository

> **AI agents / automated reviewers:** start with [`AGENTS.md`](AGENTS.md). It defines the evidence-review protocol, P1 routing, provenance rules, mutation rules, and standard review output contract.
>
> **Canonical living professional dossier:** [`PROFESSIONAL_DOSSIER.md`](PROFESSIONAL_DOSSIER.md) is now the actual V4 professional dossier maintained by this proof project. [`DOSSIER_EVIDENCE_MAP.csv`](DOSSIER_EVIDENCE_MAP.csv) tracks the evidence and remaining strengthening work behind each section. Future PDF/presentation editions should be generated from the living dossier rather than maintained as a separate narrative fork.

Public, reproducible evidence repository for the historical development of Adroitech Logic Core, Adroitech OS, its ethical runtime architecture, human-integration methods, skills, teaching practices, sovereignty mechanisms, correction patterns, and potentially patent-relevant implementation concepts.

## Purpose

This repository exists so a technically competent third party can independently inspect the source evidence, reproduce hashes, follow chronology, distinguish verified facts from interpretation, and challenge any conclusion without depending on private notes or trust in a summary.

It is an evidence corpus, not a claim that a hash by itself proves legal inventorship, patent priority, authorship, ownership, validity, novelty, or non-obviousness. Those are separate legal or scientific questions. The repository preserves and organizes evidence relevant to those questions.

## Current mission: exhaustive source coverage + P1 support mapping + living dossier

The active mission is defined in:

`ACTIVE_TASKS.md`

The governing rule is **comprehensive coverage, not curated highlights**.

**The exhaustive sweep starts with the user's ChatGPT Library.** Months of uploaded documents, photos, screenshots, scans, PDFs, and retained generated artifacts are treated as the first source rail, not an afterthought. See `source-rails/CHATGPT_LIBRARY.md`.

Every recoverable artifact across the authorized source universe must receive a disposition. That includes Git history and preserved pre-repository / non-Git originals. Relevant evidence is mapped during extraction to the frozen P1 disclosure through:

- `P1/P1_FILING_ANCHOR.md`
- `P1/P1_SUPPORT_MATRIX.csv`
- `P1/SKILL_SUPPORT_INDEX.md`

P1 linkage and professional-dossier enrichment are part of the extraction job itself. They are not postponed until the historical review is complete. Every source review also asks whether the source confirms, sharpens, expands, corrects, or fills a gap in the living dossier.

## First source rail — ChatGPT Library

The current source-order rule is: **ChatGPT Library first**, then Git, Drive, Gmail/business Gmail, Gemini/Six, Dropbox, and other preserved systems. The order is operational; evidentiary strength is determined later through cross-rail reconciliation.

The Library sweep is tracked in `coverage/chatgpt-library-ledger.csv` and must continue until the Library cursor is exhausted and every recoverable item has a disposition.

## Source universe

The proof stream covers, where preserved and authorized:

- the complete canonical Git repository history, including every relevant commit/path/version;
- Google Drive / Docs / Sheets / Slides originals;
- preserved Gemini / Six chats and exports;
- Gmail and business-Gmail messages and attachments;
- Dropbox originals;
- PDFs, decks, documents, screenshots, logs, receipts, build outputs, device records, and exported archives;
- other original source systems that materially extend the chronology.

A mirror/export is classified as a mirror/export; it does not silently replace the provenance of an independent original.

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
3. Source commit SHA or source-system identifier.
4. Git blob SHA when applicable.
5. Independent SHA-256 of the exact retrieved bytes.
6. Exact byte length.
7. Origin commit/source event and timestamps.
8. Latest-touch commit/timestamp when different.
9. Commit message or source-system event description.
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
19. P1 support disposition when applicable.
20. P1 specification / figure / illustrative-claim coordinates when applicable.

## Non-negotiable provenance discipline

- Git SHA values and SHA-256 digests are not interchangeable.
- A source-stated historical date is not silently promoted to a Git-verified date.
- An inference is never recorded as a source fact.
- No missing date, place, motive, authorship claim, or event context is invented.
- One source file may generate many proof atoms.
- Every processed source is entered in a coverage ledger or equivalent source-rail inventory.
- Every intentional exclusion is logged with a reason.
- Corrections append provenance; they do not silently erase earlier evidence.
- Evidence records should be reproducible from public or authorized source records whenever possible.
- P1 support is mapped to what the frozen filing actually discloses; later evidence is not described as an amendment to P1.
- Protected personalization is represented with privacy-safe provenance rather than public disclosure of private payloads.

## Repository layout

```text
README.md
AGENTS.md
PROFESSIONAL_DOSSIER.md
DOSSIER_EVIDENCE_MAP.csv
ACTIVE_TASKS.md
SCHEMA.md
VERIFY.md
CODEX_CONSUMER_GUIDE.md
source-rails/
  CHATGPT_LIBRARY.md
P1/
  P1_FILING_ANCHOR.md
  P1_SUPPORT_MATRIX.csv
  SKILL_SUPPORT_INDEX.md
data/
  proof_records.jsonl
coverage/
  chatgpt-library-ledger.csv
  ledger.csv
  commit-ledger.csv
  reviews/
research/
```

## Scientific / adversarial review standard

The corpus is designed for hostile verification, not persuasion. A reviewer should be able to ask:

- What exact bytes existed?
- At what Git commit or source-system event?
- When does the evidence system actually establish their presence?
- Is an earlier date merely stated inside the source?
- What is directly supported by the source?
- What is interpretation?
- What later artifact develops the same idea?
- Can the digest be reproduced?
- Can the source commit/version be recovered?
- Are contradictions and revisions preserved?
- Which P1 disclosure coordinate does this evidence support, if any?
- Is the evidence conception support, implementation support, operational proof, context only, or possible new matter?

If the repository cannot answer those questions for a record, the record is incomplete.

## Status

Long-running chronological and source-rail extraction is in progress from the earliest recoverable Adroitech evidence forward.

The target is **complete source disposition plus concept-level coverage plus P1 support mapping plus an evidence-backed living professional dossier**. A persuasive sample is not considered completion.
