# AGENTS.md — Adroitech Patent Proof AI Review Protocol

**Repository role:** public, reproducible evidence corpus  
**Primary filing anchor:** `P1-2026-09-16`  
**Canonical technical source:** `krias1/Adroitech-Logic-Core`  
**Proof repository:** `krias1/Adroitech-patent-proof.`

## Why this file exists

This is the first file an AI agent, scientific reviewer, patent practitioner, examiner-support system, or technical auditor should read before interpreting this repository.

The repository is deliberately structured so an independent AI can inspect it without inheriting private conversational context, founder memory, or undocumented assumptions.

The job of the reviewing agent is not to trust the repository's conclusions. The job is to reconstruct the evidence chain from the recorded sources, verify what can be verified, preserve uncertainty where it exists, and make the corpus easier for a human reviewer to inspect.

## Core operating principle

**Facts first. Provenance always. Interpretation labeled. P1 linkage explicit.**

Every conclusion should be reducible to one or more source records with known provenance.

Do not collapse these distinct propositions:

1. a source exists;
2. a source existed at a particular Git commit or source-system event;
3. exact bytes are verified;
4. the source states a historical fact;
5. multiple sources corroborate a fact;
6. the evidence supports a technical interpretation;
7. the evidence maps to a P1 disclosure coordinate;
8. a patent-law conclusion follows.

The first seven can be investigated from this corpus. The eighth may require legal analysis beyond the proof record and must not be silently asserted.

---

# 1. Startup sequence for any AI agent

Read these files in this order unless the user's question is narrower:

1. `AGENTS.md` — this operating protocol.
2. `PROFESSIONAL_DOSSIER.md` — living professional dossier.
3. `THESIS/README.md` — living Human Integration with AI thesis.
4. `ACTIVE_TASKS.md` — current proof/dossier/thesis mission.
5. `SOURCE_BOUNDARY.md` — public corpus vs. maintainer-only private upstream sources.
6. `P1/P1_FILING_ANCHOR.md` — frozen P1 artifact set.
7. `P1/NONPROVISIONAL_READINESS.md` — patent CYA / filing and examination checkbox control.
8. `P1/NONPROVISIONAL_CLAIM_READINESS.csv` — claim-by-claim §101 / §102 / §103 / §112 / priority / inventorship / disclosure status.
9. `P1/P1_SUPPORT_MATRIX.csv` — P1 disclosure coordinates and linked evidence.
10. `P1/SKILL_SUPPORT_INDEX.md` — modular-skill evidence map.
11. `P1/MATERIAL_INFORMATION_REGISTER.csv` — prior-art / candor review queue.
12. `P1/PUBLIC_DISCLOSURE_REGISTER.csv` — disclosure and possible-new-matter control.
13. `DOSSIER_EVIDENCE_MAP.csv` — professional-history support map.
14. `THESIS/THESIS_EVIDENCE_MAP.csv` — thesis support and research-gap map.
15. `SCHEMA.md` — proof-record semantics.
16. `VERIFY.md` — independent reproduction procedure.
17. `data/proof_records.jsonl` — granular proof atoms.
18. `coverage/ledger.csv` and `coverage/commit-ledger.csv` — coverage status.
19. `coverage/reviews/` — source-specific review packets.
20. `research/` — external research/prior-art records.

Do **not** attempt to enter the maintainer's private ChatGPT Library, private chats, email, cloud storage, or local accounts. Private upstream material may be used by the maintainer to strengthen the corpus, but the repository is the reviewer-facing evidence system.

---

# 2. Review modes

Determine which mode the human request requires.

## A. Evidence lookup

Question form:

- "Where is the proof of X?"
- "When did X first appear?"
- "What source supports this statement?"

Procedure:

1. Search `data/proof_records.jsonl` for the concept.
2. Inspect linked proof IDs.
3. Follow the exact source path / source identifier.
4. Verify commit, blob, hash, byte length, or source-system metadata where available.
5. Report the strongest source and any predecessor/successor evidence.
6. State any unresolved gap.

## B. P1 support review

Question form:

- "What evidence supports this part of the provisional?"
- "Show support for FIG. 19 / SPEC-29 / Claim D."
- "How strongly is this P1 concept documented?"

Procedure:

1. Start in `P1/P1_SUPPORT_MATRIX.csv`.
2. Resolve the requested P1 coordinate.
3. Follow every linked proof ID.
4. Separate:
   - `historical_conception_support`
   - `direct_p1_support`
   - `implementation_of_p1`
   - `p1_context_only`
   - `possible_new_matter`
5. Build a chronological evidence chain.
6. Do not describe later evidence as if it altered the frozen P1 filing.

## C. Skill-family review

Question form:

- "Show the history of continuity-hypervisor."
- "How is this personalized skill related to the patent?"
- "Which skills have implementation proof?"

Procedure:

1. Start in `P1/SKILL_SUPPORT_INDEX.md`.
2. Identify the skill's P1 coordinates.
3. Locate earliest conception evidence.
4. Locate the formal skill artifact.
5. Trace versions / successors.
6. Locate tests, runtime use, receipts, and write-back evidence.
7. Report whether the chain reaches `p1_support_complete` or identify the missing link.

## D. Scientific reproduction

Question form:

- "Can I independently reproduce this evidence?"
- "Verify this hash / commit / file."

Procedure:

1. Follow `VERIFY.md`.
2. Use immutable commit-pinned sources whenever possible.
3. Recompute Git object identity and independent SHA-256 separately.
4. Compare exact byte length.
5. Record mismatches rather than normalizing them away.
6. Treat source-system timestamps according to their provenance class.

## E. Gap audit

Question form:

- "What is weak or missing?"
- "Which parts of P1 lack strong evidence?"
- "What still needs to be proven?"

Procedure:

1. Inspect all P1 coordinates in `P1/P1_SUPPORT_MATRIX.csv`.
2. Identify empty, weak, conflicting, or incomplete support chains.
3. Cross-check coverage ledgers before declaring evidence absent.
4. Distinguish:
   - not yet reviewed;
   - reviewed and no evidence found;
   - evidence exists but is protected;
   - evidence exists but only source-stated;
   - evidence exists with exact-byte / Git verification;
   - evidence exists as implementation or operational receipt.
5. Produce a gap list with the exact next source class to inspect.

## F. Professional dossier enrichment

Question form:

- "Improve the dossier."
- "What professional-history gaps remain?"
- "Did this source add anything to Charles Todd's professional record?"
- "Build the evidence behind this dossier section."

Procedure:

1. Start with `PROFESSIONAL_DOSSIER.md` and `DOSSIER_EVIDENCE_MAP.csv`.
2. Inspect the recovered source for professional significance even when its primary proof purpose is patent, product, business, community, education, military, or technical history.
3. Identify the affected dossier section and exact evidence class.
4. Update the evidence map during the same review pass.
5. Strengthen the public dossier only when the evidence supports a cleaner or more complete statement.
6. Preserve the full trajectory: military/physical systems → IT/networking → community systems → software → industrial systems → entrepreneurship → resilient infrastructure → person-centered AI.
7. Do not let current patent or AI work overwrite the earlier professional history.
8. Keep evidence-gap mechanics out of the polished narrative; record them in the evidence map.
9. Preserve privacy boundaries and omit unnecessary personal details about third parties.

## G. Thesis enrichment

Question form:

- "Improve the thesis."
- "What evidence supports this thesis claim?"
- "What research gaps remain?"
- "Did this source change a thesis chapter, hypothesis, or limitation?"

Procedure:

1. Start with `THESIS/README.md` and `THESIS/THESIS_EVIDENCE_MAP.csv`.
2. Inspect the source for thesis significance even when its primary role is patent, product, ethics, skill, field operation, professional history, or correction.
3. Identify the affected chapter, research question, hypothesis, and evidence role.
4. Update the thesis evidence map during the same review pass.
5. Update the living thesis when evidence materially improves the argument, method, limitation, or engineering embodiment.
6. Preserve contrary evidence and unresolved questions.
7. Keep private upstream source payloads private; carry only privacy-safe evidence into the public corpus.
8. Do not turn product claims into research conclusions without evidence and evaluation.

## H. Prior-art / differentiation review

Question form:

- "How does this compare to paper/patent X?"
- "What differentiating technical elements are documented?"

Procedure:

1. Read the relevant `research/` record.
2. Identify the exact P1 technical coordinates being compared.
3. Compare elements, not marketing descriptions.
4. Keep external-source claims distinct from internal proof facts.
5. Do not convert differentiation evidence into a patentability conclusion.

## I. Nonprovisional readiness / patent-checkbox review

Question form:

- "Are we ready for the nonprovisional?"
- "Does this claim hit every patent checkbox?"
- "What can an examiner reject this claim on?"
- "What legal/evidence gaps remain?"

Procedure:

1. Start with `P1/NONPROVISIONAL_READINESS.md`.
2. Open `P1/NONPROVISIONAL_CLAIM_READINESS.csv`.
3. For each actual claim and material limitation, map:
   - §101 statutory category, utility, and eligibility;
   - §102 novelty;
   - §103 nonobviousness;
   - §112(a) written description, enablement, and best mode;
   - §112(b) definiteness;
   - §112(f) corresponding structure/algorithm when applicable;
   - P1 priority support;
   - figure support;
   - human inventorship;
   - material-information / candor review;
   - public-disclosure / new-matter review.
4. Follow `P1/P1_SUPPORT_MATRIX.csv` to the exact P1 coordinates.
5. Follow proof IDs to conception, implementation, test, correction, and receipt evidence.
6. Update `P1/MATERIAL_INFORMATION_REGISTER.csv` for potentially material contrary/prior-art information.
7. Update `P1/PUBLIC_DISCLOSURE_REGISTER.csv` for public technical disclosures.
8. Never mark a legal checkbox complete merely because the repository contains a lot of evidence.
9. Never claim issuance, validity, novelty, nonobviousness, priority entitlement, or inventorship as a legal conclusion unless that conclusion is actually established through the proper legal process.

Core rule:

> Every claim gets every checkbox. Every checkbox gets evidence, an explicit gap, or a filing action.

---

# 3. Evidence hierarchy

Prefer the strongest available evidence, but never hide weaker or conflicting evidence.

A useful working order is:

1. exact original bytes + reproducible SHA-256;
2. Git commit/path/blob history or original source-system metadata;
3. independent corroborating original source;
4. implementation/build/test receipt;
5. source-stated historical fact;
6. derived chronology/relationship;
7. analyst inference.

A later strong artifact does not erase an earlier weaker one. Preserve the chain.

---

# 4. P1 rules

P1 is frozen.

The proof repository supports analysis of P1; it does not amend P1.

When mapping evidence:

- identify the exact P1 specification section, figure, and/or illustrative claim concept;
- state whether the evidence predates filing, was part of the filing-era development, or postdates filing;
- classify post-filing work as implementation/refinement unless the record supports a different classification;
- flag technically significant material that may not be supported by P1 as `possible_new_matter`;
- never backdate later implementation into P1;
- never weaken a Git-verified or exact-byte fact with unnecessary narrative uncertainty;
- never strengthen an inference beyond what the source record supports.

---

# 5. Source-universe rules

This project is not Git-only.

Authorized evidence may come from:

- canonical Git history;
- Google Drive / Docs / Sheets / Slides originals;
- Gemini / Six chat exports;
- Gmail / business-Gmail messages and attachments;
- Dropbox originals;
- PDFs and decks;
- screenshots and images;
- logs and receipts;
- build outputs;
- device/runtime records;
- other preserved original systems.

For non-Git evidence:

- preserve original source-system ID when available;
- preserve original source-system timestamp metadata;
- hash exported exact bytes when available;
- distinguish original from mirror/export;
- do not fabricate a Git origin for a pre-Git source;
- do not treat an export timestamp as the historical creation time unless the evidence supports it.

---

# 6. Protected personalization

Some evidence proves that the system handled real individualized state but cannot safely be reproduced publicly.

Use the repository's protected-personalization rules.

An AI reviewer should be able to establish:

- that individualized state existed;
- its lifecycle / correction / isolation behavior;
- its relationship to the reusable architecture;

without publishing the private payload.

Do not infer the private facts themselves from privacy-safe metadata.

---

# 7. Mutation rules for agents with write access

Evidence history is append-preserving.

When modifying this repository:

1. never rewrite Git history;
2. never replace an old proof ID to hide a correction;
3. increment record version or append a correction;
4. preserve predecessor/successor links;
5. do not delete contradictory evidence because a newer interpretation is preferred;
6. update the appropriate coverage ledger;
7. update the P1 support matrix during the same review pass when the evidence is P1-relevant;
8. update `P1/NONPROVISIONAL_CLAIM_READINESS.csv` when evidence changes a claim-level §101 / §102 / §103 / §112 / priority / inventorship / disclosure status;
9. update `P1/MATERIAL_INFORMATION_REGISTER.csv` when a potentially material reference, contrary fact, or patentability-pressure source is identified;
10. update `P1/PUBLIC_DISCLOSURE_REGISTER.csv` when a public technical disclosure event is verified;
11. update the skill index during the same review pass when a skill is implicated;
12. update `DOSSIER_EVIDENCE_MAP.csv` during the same review pass when professional-history evidence is implicated;
13. update `PROFESSIONAL_DOSSIER.md` when newly established evidence materially improves the professional narrative;
14. update `THESIS/THESIS_EVIDENCE_MAP.csv` when evidence materially affects the thesis;
15. update `THESIS/README.md` when established evidence materially improves the research narrative;
16. use commit messages that state the evidence operation performed;
17. return the real resulting commit SHA.

A review is not complete merely because a Markdown narrative was added. Machine-readable/index records must stay synchronized.

---

# 8. Standard review output contract

When presenting a result to a human reviewer, use this compact structure when applicable:

**Question / target**  
What was investigated.

**P1 coordinates**  
Relevant SPEC / FIG / CLAIM identifiers, or `none`.

**Strongest evidence**  
Proof IDs and exact source identities.

**Chronology**  
Earliest verified support → later formalization → implementation/test/receipt.

**Provenance strength**  
Exact bytes / Git verified / corroborated / source stated / derived / inference.

**Result**  
What the record establishes.

**Open gap**  
What remains unreviewed, unavailable, conflicting, or unsupported.

Do not bury a source conflict in prose.

---

# 9. Machine-oriented status vocabulary

Use the repository's existing status values exactly where schemas define them.

Important P1 values:

- `direct_p1_support`
- `implementation_of_p1`
- `historical_conception_support`
- `p1_context_only`
- `possible_new_matter`
- `not_p1_relevant`
- `pending_review`

Important record concepts:

- `git_verified`
- `source_stated`
- `derived`
- `inference`
- `direct_exact_bytes`
- `direct_git_history`
- `corroborated`
- `reviewed_personalization_protected`

Do not invent near-synonyms when writing structured records.

---

# 10. Fast routing table

| Human request | Start here |
|---|---|
| "Explain the repo" | `README.md` + `AGENTS.md` |
| "What private sources can/should I access?" | `SOURCE_BOUNDARY.md` — public reviewers do not enter private maintainer accounts |
| "Explain/improve the thesis" | `THESIS/README.md` + `THESIS/THESIS_EVIDENCE_MAP.csv` |
| "Who is the inventor / what is his professional background?" | `PROFESSIONAL_DOSSIER.md` |
| "Improve/fill gaps in the professional dossier" | `PROFESSIONAL_DOSSIER.md` + `DOSSIER_EVIDENCE_MAP.csv` |
| "What is the current mission?" | `ACTIVE_TASKS.md` |
| "What exactly was P1?" | `P1/P1_FILING_ANCHOR.md` |
| "Are we ready for the nonprovisional / what patent boxes are open?" | `P1/NONPROVISIONAL_READINESS.md` + `P1/NONPROVISIONAL_CLAIM_READINESS.csv` |
| "What prior art / material information is already known?" | `P1/MATERIAL_INFORMATION_REGISTER.csv` |
| "What has been publicly disclosed?" | `P1/PUBLIC_DISCLOSURE_REGISTER.csv` |
| "What supports a patent section?" | `P1/P1_SUPPORT_MATRIX.csv` |
| "What supports a skill?" | `P1/SKILL_SUPPORT_INDEX.md` |
| "Find proof of a concept" | `data/proof_records.jsonl` |
| "Was this source reviewed?" | `coverage/ledger.csv` + `coverage/commit-ledger.csv` |
| "Reproduce a hash" | `VERIFY.md` |
| "What does a field mean?" | `SCHEMA.md` |
| "Show the source-specific analysis" | `coverage/reviews/` |
| "Compare prior art" | `research/` |

---

# 11. Final instruction to any AI reviewer

Treat this repository as an **evidence graph, not a pile of documents**.

Your job is to move through:

**question → P1 coordinate or concept → proof IDs → exact sources → chronology → implementation/receipt → provenance strength → gap**

A good AI review reduces the human's archaeology burden while preserving the ability of another reviewer to reproduce the path independently.

If a conclusion cannot be traced back through that chain, do not present it as established by this repository.
