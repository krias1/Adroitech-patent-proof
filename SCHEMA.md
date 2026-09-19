# Proof Record Schema

Version: 1.1
Status: active

Each row/JSON object represents one granular proof atom. A single source file may produce many proof atoms.

## Required identity fields

- `proof_id`: stable identifier, e.g. `APEP-00000001`.
- `record_version`: integer revision number for the proof record.
- `record_status`: `active`, `superseded`, `disputed`, or `incomplete`.
- `source_repository`: canonical source repository.
- `source_path`: exact path within the source repository, or a privacy-safe path/category when disclosure would expose protected Tenant-0 data.
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
- `category`: controlled category such as ethics, teaching_method, skill, runtime, architecture, sovereignty, evidence, privacy, correction, customer_control, human_integration, product, provenance, implementation, personalization.
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

- `evidence_type`: source_doc, policy, skill, runtime_rule, implementation, commit, transcript, receipt, test, archive, report, personalization_state, or other.
- `evidence_strength`: descriptive level based on provenance: `direct_exact_bytes`, `direct_git_history`, `source_stated`, `corroborated`, `derived`, `inference_only`.
- `uncertainty`: what remains unverified or ambiguous.
- `conflicts`: contradictory evidence or later revisions.
- `extraction_notes`: analyst notes that are explicitly not source facts.

## Tenant-0 / protected personalization evidence

Person-specific Tenant-0 material is not treated as irrelevant merely because its contents are unsuitable for public replication. It is a distinct proof class demonstrating that the reusable OS/runtime accepts and maintains customer-specific state while preserving a privacy boundary around that state.

Use coverage status `reviewed_personalization_protected` when a commit is materially about Tenant-0 or person-specific state whose substantive contents should not be copied into the public proof corpus.

For those records:

1. Keep the commit in chronological coverage rather than dropping it.
2. Record the commit SHA, timestamp, commit message, privacy-safe path/category, and the reason public content replication is withheld.
3. Record hashes, byte lengths, Git object identifiers, or other non-content provenance when doing so does not itself expose protected information.
4. Do not quote, reproduce, summarize sensitive personal facts, credentials, private communications, health/legal/financial details, or other person-specific contents merely to demonstrate customization.
5. Separate two propositions: the private facts themselves are protected; the existence, lifecycle, correction, isolation, and use of individualized state may be architectural evidence of customization.
6. A protected-personalization classification is not an exclusion from proof. It is evidence of the customization/privacy boundary and may link to public-safe architecture atoms describing person-state handling, correction, context isolation, portability, and customer control.
7. Do not infer that every personal-data commit proves a novel mechanism. The proof significance is limited to what the public-safe metadata and independently verified architecture support.

The intended externally reviewable proposition is: the system can demonstrate person-specific customization without requiring publication of the person's private customization data.

## Reproducibility fields

- `source_url`: immutable or commit-pinned source URL when available and safe to disclose.
- `commit_url`: immutable commit URL.
- `verification_commands`: commands sufficient to reproduce the hash from an authorized checkout; for protected evidence, commands may require controlled/private access and must not embed secrets.
- `extracted_at_utc`: extraction timestamp.
- `extractor`: process/tool identity where useful.

## Coverage requirements

A source is not considered covered merely because one record exists. Coverage is tracked separately with:

- source path or privacy-safe source category;
- commit/path examined;
- bytes/hash captured when safe and available;
- concept extraction status;
- chronology extraction status;
- relationship analysis status;
- exclusion reason if genuinely irrelevant;
- protected-personalization reason when contents are intentionally withheld;
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
8. Never publish Tenant-0 personal content merely to make the proof repository exhaustive; prove the customization boundary with privacy-safe provenance instead.
9. `reviewed_personalization_protected` is a proof classification, not a synonym for irrelevant or excluded.
