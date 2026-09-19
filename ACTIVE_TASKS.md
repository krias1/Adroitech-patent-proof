# Active Tasks — Patent Proof / P1 Support / Living Dossier Mission

**Effective:** 2026-09-19  
**Primary filing anchor:** `P1-2026-09-16`  
**Canonical source repository:** `krias1/Adroitech-Logic-Core`

## Mission

Build a comprehensive, reproducible evidence record for the complete historical development of Adroitech OS, continuously map that evidence to the technical disclosure already contained in P1, and maintain the canonical living professional dossier from the same exhaustive source sweep.

This is not a curated highlights project. The proof stream is responsible for **every recoverable source artifact** across the available source rails. Every artifact that can be retrieved must receive a disposition: relevant proof, protected-personalization proof, mirror/export, duplicate, superseded material, or documented exclusion with a reason.

No source is skipped merely because it looks ordinary, repetitive, pre-repository, founder-specific, nontechnical at first glance, or inconvenient to classify. The point of the sweep is to discover the concepts, chronology, implementation history, teaching methods, ethical runtime rules, personalization mechanisms, and technical downflows that become visible only when the whole record is reviewed.

## Source-rail execution order

**Phase 0 starts with the ChatGPT Library.** The Library contains months of directly uploaded documents, images, screenshots, scans, PDFs, records, and prior generated artifacts and must be exhaustively inventoried before the wider rail sweep is considered complete.

Operational order:

1. ChatGPT Library — first exhaustive pass; see `source-rails/CHATGPT_LIBRARY.md` and `coverage/chatgpt-library-ledger.csv`.
2. Canonical Git history.
3. Google Drive originals.
4. Gmail / business-Gmail originals and attachments.
5. Gemini / Six chats and exports.
6. Dropbox originals.
7. Other preserved local/external source systems.

This order controls the sweep, not evidentiary weight. Cross-rail reconciliation still determines which artifact is original, earliest, strongest, duplicate, or mirror.

## Source rails in scope

The sweep includes, when preserved and authorized:

- **ChatGPT Library / prior ChatGPT-uploaded files and images as the first source rail;**

- every commit, path, historical version, run receipt, build record, skill, policy, architecture document, test, code artifact, drawing, PDF, and implementation record in the canonical Git repository;
- original Google Drive / Docs / Sheets / Slides records;
- preserved Gemini / Six chats and exports;
- Gmail and business-Gmail messages and attachments;
- Dropbox originals;
- local PDFs, decks, documents, screenshots, logs, receipts, build outputs, device records, and exported archives;
- other preserved source systems that materially extend the chronology.

Repository mirrors and exports do not replace an independent original rail. Preserve the source-system metadata and classify the relationship.

## P1 support rule

Every relevant proof atom must be evaluated for its relationship to P1.

Use these support dispositions:

- `direct_p1_support` — directly evidences a technical mechanism, embodiment, figure concept, or claim concept disclosed in P1;
- `implementation_of_p1` — later or parallel implementation/testing of a mechanism disclosed in P1;
- `historical_conception_support` — evidence predating P1 that shows the development path of subject matter disclosed in P1;
- `p1_context_only` — useful context but not relied on as technical support;
- `possible_new_matter` — technically relevant material that should not be silently characterized as already disclosed by P1;
- `not_p1_relevant` — reviewed and not materially related to P1.

Every `direct_p1_support`, `implementation_of_p1`, or `historical_conception_support` record should identify the closest P1 coordinates: specification section, figure, illustrative claim concept, or combination.

The proof repository does **not** amend P1. It builds the traceable evidence map around the frozen filing.

## Active priorities

1. **P0-A — Exhaustive ChatGPT Library sweep.** Start with the user's ChatGPT Library. Exhaust the Library inventory cursor, enter every item into `coverage/chatgpt-library-ledger.csv`, classify duplicates/protected items, and route relevant evidence into proof atoms, the P1 matrix, and the living dossier.
2. **P0-B — Freeze the P1 filing anchor.** Maintain `P1/P1_FILING_ANCHOR.md` with the exact filed-artifact identities, canonical commit, blob IDs, independent hashes, and receipt status.
3. **P0 — Populate the P1 support matrix.** `P1/P1_SUPPORT_MATRIX.csv` must contain every material P1 disclosure coordinate and accumulate linked proof IDs as the historical sweep proceeds.
4. **P0 — Exhaustive source inventory.** Every recoverable artifact from every authorized source rail receives a coverage/disposition record.
5. **P0 — Living dossier enrichment.** Every reviewed source is also checked for professional-history significance. Update `DOSSIER_EVIDENCE_MAP.csv` during the same pass and strengthen `PROFESSIONAL_DOSSIER.md` when the evidence materially confirms, expands, corrects, or sharpens the professional record.
6. **P0 — Chronological extraction.** Continue commit-by-commit and source-by-source review from the earliest evidence forward; do not skip low-drama records.
7. **P0 — Skill support mapping.** Maintain `P1/SKILL_SUPPORT_INDEX.md` so each personalized/modular skill is tied to P1's skill architecture and to its own conception, implementation, test, and receipt evidence.
8. **P1 — Backfill existing proof atoms.** Existing records created before the P1-support fields were added must be mapped to P1 where applicable.
9. **P1 — External-rail reconciliation.** Tie pre-Git and non-Git originals into the same concept chronology without falsely converting source-system dates into Git dates.
10. **P1 — Operational evidence.** Where possible, connect design/conception records to builds, tests, successful runs, field use, device deployment, receipts, and material write-back.
11. **P1 — Independent verification.** Preserve exact bytes, Git object identities, SHA-256, byte lengths, immutable URLs, and reproduction instructions.
12. **P1 — Gap register.** Any P1 disclosure coordinate with weak, incomplete, conflicting, or not-yet-linked evidence stays explicitly visible until resolved.

## Completion standard

The proof mission is not complete when a persuasive sample exists.

It is complete only when:

- every recoverable source artifact in the authorized source universe has a disposition;
- every relevant concept has traceable provenance and chronology;
- every material P1 disclosure coordinate has an evidence status in the support matrix;
- every personalized/modular skill has a support record or a documented reason why it is outside P1;
- every material professional-dossier section has an evidence trail in `DOSSIER_EVIDENCE_MAP.csv` and the living narrative reflects the strongest established record without exposing private evidence mechanics;
- predecessor/successor relationships and corrections are preserved;
- protected personal evidence is represented by safe provenance rather than exposed content;
- unresolved gaps remain explicit rather than being buried by narrative confidence.

## Operating rule

As the archive is combed, the P1 support map **and the professional dossier evidence map** are updated during the same proof work. P1 linkage and dossier enrichment are not later cleanup exercises. Evidence extraction, P1-support classification, and professional-history reconstruction are one integrated mission.
