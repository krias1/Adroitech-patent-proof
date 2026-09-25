# Adroitech Patent Proof Repository

## Patent examiner front door

Primary patent-review surfaces:

- `P1/EXAMINER_FRONT_DOOR.md`
- `P1/EXAMINER_QUESTION_MATRIX.csv`
- `PROOF_SCRAPER_MISSION.md`

The patent lane is backward-looking from P1. It answers examiner/reviewer questions from pre-P1 evidence and does not operate as a forward feed of new Adroitech technical work. Later discovery of old evidence is allowed; later invention is not backdated.

> **AI agents / automated reviewers:** start with [`AGENTS.md`](AGENTS.md). It defines the evidence-review protocol, P1 routing, provenance rules, mutation rules, and standard review output contract.
>
> **Canonical living professional dossier:** [`PROFESSIONAL_DOSSIER.md`](PROFESSIONAL_DOSSIER.md) is maintained by this proof project, with [`DOSSIER_EVIDENCE_MAP.csv`](DOSSIER_EVIDENCE_MAP.csv) underneath it.
>
> **Canonical living thesis:** [`THESIS/README.md`](THESIS/README.md) is the evidence-backed Human Integration with AI thesis surface. [`THESIS/THESIS_EVIDENCE_MAP.csv`](THESIS/THESIS_EVIDENCE_MAP.csv) tracks which sources support each chapter, claim, hypothesis, limitation, and research gap.
>
> **Community early access:** [`COMMUNITY_EARLY_ACCESS.md`](COMMUNITY_EARLY_ACCESS.md) is the short front door for cultural and community reviewers invited before the broader professional rollout.
>
> **Public outreach / media kit:** [`PUBLIC_OUTREACH_KIT.md`](PUBLIC_OUTREACH_KIT.md) turns the AI-failure, correction, spreadsheeting, dignity, and receipt-driven provenance work into a public-facing story without overstating what the evidence proves.
>
> **Frozen cultural/intellectual originals:** [`ORIGINALS/CULTURAL_LINEAGE/README.md`](ORIGINALS/CULTURAL_LINEAGE/README.md) and [`ORIGINAL_SOURCE_MANIFEST.csv`](ORIGINALS/CULTURAL_LINEAGE/ORIGINAL_SOURCE_MANIFEST.csv) pin the original Human Condition / Poor Righteous Teacher / music-as-teaching source family without rewriting or academic normalization.

Public, reproducible evidence repository for the historical development of Adroitech Logic Core, Adroitech OS, its ethical runtime architecture, human-integration methods, skills, teaching practices, sovereignty mechanisms, correction patterns, and potentially patent-relevant implementation concepts.

## Purpose

This repository exists so a technically competent third party can independently inspect the source evidence, reproduce hashes, follow chronology, distinguish verified facts from interpretation, and challenge any conclusion without depending on private notes or trust in a summary.

It is an evidence corpus, not a claim that a hash by itself proves legal inventorship, patent priority, authorship, ownership, validity, novelty, or non-obviousness. Those are separate legal or scientific questions. The repository preserves and organizes evidence relevant to those questions.

## Current mission: exhaustive source coverage + P1 support mapping + living dossier + living thesis

The active mission is defined in:

`ACTIVE_TASKS.md`

The governing rule is **comprehensive coverage, not curated highlights**.

**Private upstream sources may be used by the maintainer to strengthen this corpus, but they are not reviewer dependencies.** Prior ChatGPT Library uploads, private chats, private email/cloud records, photographs, and other archives may help recover evidence during curation; public reviewers work from the repository and its public/commit-pinned references. See `SOURCE_BOUNDARY.md`.

Every recoverable artifact across the authorized source universe must receive a disposition. That includes Git history and preserved pre-repository / non-Git originals. Relevant evidence is mapped during extraction to the frozen P1 disclosure through:

- `P1/P1_FILING_ANCHOR.md`
- `P1/NONPROVISIONAL_READINESS.md`
- `P1/NONPROVISIONAL_CLAIM_READINESS.csv`
- `P1/P1_SUPPORT_MATRIX.csv`
- `P1/SKILL_SUPPORT_INDEX.md`
- `P1/MATERIAL_INFORMATION_REGISTER.csv`
- `P1/PUBLIC_DISCLOSURE_REGISTER.csv`

P1 linkage, nonprovisional-readiness control, professional-dossier enrichment, and thesis enrichment are part of the same evidence work. Every reviewed source is checked for patent relevance, professional-history relevance, and thesis relevance.

The nonprovisional control surface follows a strict rule: **every serious claim gets every patent checkbox; every checkbox gets evidence, an explicit gap, or a filing action.** The repository does not pretend an open legal or procedural issue is complete merely because supporting evidence exists.

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

`https://github.com/krias1/Adroitech-patent-proof`

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
SOURCE_BOUNDARY.md
THESIS/
  README.md
  THESIS_EVIDENCE_MAP.csv
P1/
  P1_FILING_ANCHOR.md
  NONPROVISIONAL_READINESS.md
  NONPROVISIONAL_CLAIM_READINESS.csv
  P1_SUPPORT_MATRIX.csv
  SKILL_SUPPORT_INDEX.md
  MATERIAL_INFORMATION_REGISTER.csv
  PUBLIC_DISCLOSURE_REGISTER.csv
data/
  proof_records.jsonl
coverage/
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

The target is **complete source disposition plus concept-level coverage plus P1 support mapping plus an evidence-backed living professional dossier and living thesis**. A persuasive sample is not considered completion.
