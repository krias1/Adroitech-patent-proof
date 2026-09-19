# ChatGPT Library — First Source Rail

**Priority:** Phase 0 / first exhaustive source sweep  
**Rail:** ChatGPT Library / prior uploaded files and images available to the authorized user  
**Status:** ACTIVE — initial inventory started 2026-09-19

## Directive

The exhaustive proof-and-dossier sweep begins with the user's **ChatGPT Library** before expanding to the other source rails.

This is deliberate. Months of documents, photographs, screenshots, PDFs, receipts, transcripts, letters, business records, technical artifacts, generated drafts, and other files were supplied directly through ChatGPT. Those materials are not a secondary convenience source. They are a first-class evidence rail and may contain originals or earlier copies that predate later Git ingestion, Drive reconciliation, or repository summaries.

The first-pass job is therefore:

**ChatGPT Library → full inventory → file-by-file disposition → concept extraction → dossier relevance → P1 relevance → cross-rail reconciliation**

## Scope

Review every recoverable Library item, including:

- user-uploaded PDFs;
- images and photographs;
- screenshots;
- scans;
- Word/text documents;
- spreadsheets;
- presentations;
- exported emails/chats;
- receipts and letters;
- resumes and professional records;
- educational and institutional records;
- military/service records;
- business formation and operating records;
- technical diagrams and device records;
- generated documents retained in Library;
- duplicates, mirrors, and superseded versions.

Do not assume a generated file is irrelevant. It may preserve a dated presentation state or a previously consolidated evidence set. Classify it correctly rather than skipping it.

## Required disposition for every Library item

Every item must end in one of these states:

- `relevant_proof`
- `dossier_support`
- `p1_support`
- `implementation_or_receipt`
- `protected_personalization`
- `duplicate_or_mirror`
- `superseded`
- `context_only`
- `irrelevant_reviewed`
- `incomplete_review`

One item may carry more than one relevance role.

## Required metadata

Where available, preserve:

- Library filename;
- Library path/folder;
- stable Library/file identifier;
- source-created/uploaded timestamp;
- modified timestamp;
- MIME/type;
- byte length;
- whether model-generated or user-uploaded;
- exact-byte SHA-256 when raw bytes are safely materialized;
- relationship to duplicates/mirrors;
- relationship to later Git/Drive/Gmail/Dropbox copies;
- professional-dossier section(s) affected;
- P1 coordinate(s) affected;
- proof IDs emitted;
- privacy/protection classification.

## Review procedure

1. Enumerate the Library in stable batches until the Library cursor is exhausted.
2. Record every discovered item in `coverage/chatgpt-library-ledger.csv`.
3. Deduplicate by exact bytes/hash when possible; do not deduplicate by filename alone.
4. Review the actual content where authorized and relevant.
5. Emit proof atoms for patent/provenance-significant concepts.
6. Update `DOSSIER_EVIDENCE_MAP.csv` for professional-history evidence.
7. Update `PROFESSIONAL_DOSSIER.md` when evidence materially strengthens the public narrative.
8. Update `P1/P1_SUPPORT_MATRIX.csv` when evidence supports a P1 disclosure coordinate.
9. Preserve protected material through privacy-safe provenance rather than reproducing sensitive payloads.
10. Cross-link later copies in Git, Drive, Gmail, Dropbox, or other rails rather than silently treating them as independent originals.

## Initial inventory confirmation

The Library rail has been directly inspected and is populated with historical Adroitech and professional records. The first inventory page alone returned at least 100 items and a continuation cursor, confirming that this is a substantial evidence source rather than a small attachment set.

Targeted Library search immediately surfaced, among other items:

- `Charles_Anthony_Todd_Jr_Professional_Dossier_v1_Noted.pdf`
- `verification_letter-letters-of-recommendation.pdf`
- `Academic Transcript.pdf`
- `benefit_summary.pdf`
- `Adroitech LLC: Mission Continuity Brief`

These are examples only. They do **not** define the scope. The sweep remains exhaustive.

## Ordering rule

The source-rail order for the next exhaustive pass is:

1. **ChatGPT Library**
2. canonical Git history / repository-native evidence
3. Google Drive originals
4. Gmail / business Gmail originals and attachments
5. Gemini / Six chat originals/exports
6. Dropbox originals
7. other preserved local/external source systems

Cross-rail reconciliation may cause a later rail to establish an earlier historical date or a stronger original. Source order is an operational sweep order, not a provenance-ranking rule.

## Completion condition

The ChatGPT Library phase is complete only when:

- the Library cursor has been exhausted;
- every recoverable Library item has a ledger entry;
- every item has a disposition;
- duplicates/mirrors are classified;
- privacy-safe handling is applied where needed;
- all relevant dossier/P1/proof linkages are recorded;
- unresolved items remain explicitly marked rather than silently skipped.
