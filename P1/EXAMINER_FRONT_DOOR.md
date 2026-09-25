# Examiner Front Door — P1 Zero-Reconstruction Packet

**Anchor:** P1-2026-09-16  
**Strategy:** "Undeniable" = eliminate avoidable unanswered questions and evidence archaeology before examination; it is not a guarantee of issuance.

## Start here

1. `EXAMINER_QUESTION_MATRIX.csv` — every material examination/formality question, authority, answer route, gap, and next action.
2. `P1_FILING_ANCHOR.md` — exact frozen P1 artifact identity.
3. `P1_SUPPORT_MATRIX.csv` — P1 disclosure coordinates and evidence linkage.
4. `NONPROVISIONAL_CLAIM_READINESS.csv` — claim-level statutory checklist.
5. `MATERIAL_INFORMATION_REGISTER.csv` — prior-art / candor candidates.
6. `PUBLIC_DISCLOSURE_REGISTER.csv` — disclosure timing control.
7. `../data/proof_records.jsonl` — granular proof atoms.
8. `../coverage/ledger.csv` and `../coverage/commit-ledger.csv` — reviewed-source coverage.

## Operating question

For every actual claim, the repository should answer:

**What is claimed? -> where is it in P1? -> when did the supporting concept exist? -> who conceived it? -> how is it enabled? -> what is the closest prior art? -> why does no single reference disclose it? -> why would/wouldn't the combination be obvious? -> is the language definite? -> what algorithm/structure supports functional language? -> what material information/disclosures must be handled?**

## Current P0 gaps

1. Final claims and stable limitation IDs are not in the front door.
2. P1 support is incomplete at limitation level.
3. Formal USPTO Filing Receipt is not reconciled.
4. §101 eligibility is not charted against actual claims.
5. §102 single-reference novelty charts are incomplete.
6. §103 obviousness combination / reason-to-combine pressure tests are incomplete.
7. §112(a) written-description and full-scope enablement charts are incomplete.
8. §112(b) claim glossary / term-boundary / antecedent-basis review is open.
9. §112(f) algorithm/structure mapping is open.
10. Inventorship is not mapped to the actual final claims.
11. Pre-P1 public-disclosure / public-use / sale/offer audit is open.
12. Material-information / IDS candidate register is underpopulated.
13. Best-mode confirmation is open.
14. Restriction/election risk is not analyzed across final claim families.
15. Filing formalities remain: ADS benefit claim, final claims, abstract, drawings/formal review, oath/declaration, fees, and Patent Center format.

## Extraction priority

Do not scrape the source universe merely to increase corpus size.

Work each P0 matrix row until it has either:

- a reproducible answer route;
- an explicit evidence gap;
- or a clearly identified filing/legal action.

## Historical cutoff

For P1 technical/conception proof, source events must predate the actual P1 filing moment.

A later-created proof record may point to older evidence. A later-created Adroitech feature may not be backdated into P1.

## Secondary outputs

Every historical source pass may also improve:

- `../PROFESSIONAL_DOSSIER.md`
- `../DOSSIER_EVIDENCE_MAP.csv`
- `../THESIS/README.md`
- `../THESIS/THESIS_EVIDENCE_MAP.csv`

Those are secondary extractions from the same source review. They do not replace the patent examiner matrix.
