# Proof Scraper Mission — Examiner-First Historical Extraction

**Effective:** 2026-09-25  
**Anchor:** P1-2026-09-16

## Purpose

This is the operating instruction for any AI, script, or human doing source extraction for the Adroitech patent-proof repository.

The scraper is not a news feed and not a forward product monitor.

Its patent job is to make examination easy to navigate:

**examiner question -> exact answer -> exact evidence -> exact repository route -> explicit gap**

## Undeniable Strategy

"Undeniable" means zero-surprise, zero-reconstruction preparation.

It does **not** mean that a patent is guaranteed to issue.

The strategy is to identify in advance every material question the USPTO may test, then place the best available answer and provenance route directly in the repository.

## Hard patent boundary

Technical/conception evidence used to support P1 must arise before the actual P1 filing moment on 2026-09-16.

Later discovery is allowed. Later invention is not backdated.

Allowed later records:

- USPTO procedural records for P1;
- hash/byte/timestamp verification of old evidence;
- later-created indexes or proof records pointing to old evidence;
- prior art discovered later when the reference itself has a legally relevant earlier date.

Disallowed as P1 proof:

- new post-P1 Adroitech features;
- new post-P1 implementation used to pretend P1 had more disclosure;
- new post-P1 explanations treated as contemporaneous conception;
- passive monitoring of current Adroitech work merely because it exists.

## Extraction loop

1. Open `P1/EXAMINER_QUESTION_MATRIX.csv`.
2. Select the highest-priority OPEN or PARTIAL question.
3. Convert the question into concrete evidence targets.
4. Search the authorized pre-P1 source universe.
5. Preserve exact source identity, timestamps, hashes, blob/commit IDs, and source-system IDs.
6. Emit granular proof atoms.
7. Link those atoms to P1 coordinates.
8. Update the examiner matrix answer route/status.
9. Update prior-art/material-information controls when relevant.
10. Update coverage.
11. From the same source only, do the secondary dossier pass.
12. From the same source only, do the secondary thesis pass.
13. Move to the next unanswered examiner question.

## Priority order

1. Patent examiner question closure.
2. Professional dossier extraction.
3. Thesis extraction.
4. Everything else is out of scope unless the operator explicitly changes the mission.

## Question closure rule

A patent question is not closed because "there is probably evidence somewhere."

A row can move to READY_ROUTE only when the repository gives the reviewer a reproducible route to the answer.

Preferred route:

**question ID -> claim/limitation -> P1 coordinate -> proof ID -> exact source -> date/provenance -> supporting/contrary evidence -> status**

## Do not hide bad facts

Prior art, contradictory evidence, missing support, and uncertainty stay visible.

The strategy is stronger when the reviewer can see that the record was pressure-tested rather than curated to look clean.

## Scraper output contract

For each reviewed source, return:

- source identity;
- whether it predates P1;
- examiner question IDs affected;
- P1 coordinates affected;
- proof IDs created/updated;
- dossier significance;
- thesis significance;
- open gap remaining;
- coverage disposition.

If the source does not answer a patent question, do not force it into the patent lane.
