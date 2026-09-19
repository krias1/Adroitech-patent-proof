# Proof Record Schema

Version: 1.0
Status: active

Each row/JSON object represents one granular proof atom. A single source file may produce many proof atoms.

## Required identity fields

- `proof_id`: stable identifier, e.g. `APEP-00000001`.
- `record_version`: integer revision number for the proof record.
- `record_status`: `active`, `superseded`, `disputed`, or `incomplete`.
- `source_repository`: canonical source repository.
- `source_path`: exact path within the source repository.
- `source_commit_sha`: commit at which the hashed source bytes were retrieved.
- `git_blob_sha1`: Git blob object ID for the exact source bytes when available.
- `sha256`: independent SHA-256 digest of the exact retrieved source bytes.
- `byte_length`: exact byte length of the hashed source content.

## Chronology fields

- `origin_commit_sha`: earliest Git commit currently verified to introduce the relevant source.
- `origin_author_timestamp_utc`: author timestamp if available.
- `origin_committer_timestamp_utc`: committer timestamp if available.
- `origin_commit_message`: exact commit message.
- `latest_touch_commit_sha`: latest known commit touching the source at extraction time.
- `latest_touch_timestamp_utc`: timestamp of that touch.
- `source_stated_date`: earlier or additional date explicitly stated inside the source.
- `source_stated_time`: time explicitly stated inside the source.
- `source_stated_place`: place explicitly stated inside the source.
- `chronology_class`: one or more of `git_verified`, `source_stated`, `derived`, `inference`.

## Concept fields

- `concept_title`: concise label for the atom.
- `concept_statement`: precise description of the concept evidenced.
- `source_support`: short description of where/how the source supports the atom; avoid oversized quotation.
- `category`: controlled category such as ethics, teaching_method, skill, runtime, architecture, sovereignty, evidence, privacy, correction, customer_control, human_integration, product, provenance, implementation.
- `ethical_significance`: what ethical behavior or boundary the concept contributes.
- `teaching_significance`: what method of instruction/correction/learning it contributes.
- `implementation_significance`: what system or product behavior it implies.
- `ip_relevance`: factual explanation of why the concept may matter to technical/product conception history. This field must not assert patentability, legal ownership, novelty, non-obviousness, or inventorship without separate support.

## Relationship fields

- `predecessor_proof_ids`: earlier records this develops from.
- `successor_proof_ids`: later records that refine or operationalize it.
- `related_proof_ids`: non-directional relationships.
- `supersedes_proof_ids`: records explicitly superseded.
- `superseded_by_proof_ids`: records that explicitly supersede this one.

## Evidence quality fields

- `evidence_type`: source_doc, policy, skill, runtime_rule, implementation, commit, transcript, receipt, test, archive, report, or other.
- `evidence_strength`: descriptive level based on provenance: `direct_exact_bytes`, `direct_git_history`, `source_stated`, `corroborated`, `derived`, `inference_only`.
- `uncertainty`: what remains unverified or ambiguous.
- `conflicts`: contradictory evidence or later revisions.
- `extraction_notes`: analyst notes that are explicitly not source facts.

## Reproducibility fields

- `source_url`: immutable or commit-pinned source URL when available.
- `commit_url`: immutable commit URL.
- `verification_commands`: commands sufficient to reproduce the hash from a checkout.
- `extracted_at_utc`: extraction timestamp.
- `extractor`: process/tool identity where useful.

## Coverage requirements

A source is not considered covered merely because one record exists. Coverage is tracked separately with:

- source path;
- commit/path examined;
- bytes/hash captured;
- concept extraction status;
- chronology extraction status;
- relationship analysis status;
- exclusion reason if irrelevant;
- last proof ID emitted;
- reviewer notes.

## Integrity rules

1. Never rewrite an old proof ID to hide a mistake. Increment `record_version` and preserve the correction trail.
2. Never substitute a Git SHA-1 object ID for an independent SHA-256.
3. Never describe a source-stated historical date as Git-verified.
4. Never invent a missing date, place, motive, author, or surrounding event.
5. Never infer patentability from existence of a dated record.
6. Prefer commit-pinned URLs over moving branch URLs.
7. Keep source facts, derived relationships, and interpretation in separate fields.
