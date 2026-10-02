# Nonprovisional Readiness — Patent CYA / Checkbox Matrix

## Examiner-first control note

This checklist is subordinate to `EXAMINER_QUESTION_MATRIX.csv`. The proof repository's patent mission is to answer examiner/reviewer questions from the historical P1 record, not to monitor new post-P1 technical development. Later-discovered pre-P1 evidence and later procedural verification are allowed; later technical invention does not retroactively strengthen P1.

**Repository:** `krias1/Adroitech-patent-proof`  
**Primary filing anchor:** `P1-2026-09-16`  
**Purpose:** reduce the future U.S. nonprovisional filing and examination record to a traceable set of explicit technical, evidentiary, procedural, and legal-review checkboxes.

> **Shop-floor rule:** Get the packet right before it hits the desk.

This is an engineering control surface, not a declaration that a patent must issue. The repository can make the factual record unusually complete, auditable, and low-friction; the USPTO still decides patentability, and filing/prosecution requirements still have to be satisfied in the application itself.

## Working deadline control

The frozen P1 anchor records a provisional filing date of **2026-09-16**. Under current USPTO guidance, a corresponding nonprovisional application ordinarily must be filed within 12 months to claim the benefit of the provisional filing date.

**Working target:** `2027-09-16`

The formal USPTO filing receipt must still be reconciled to the public P1 anchor. If the official filing date differs, the official USPTO record controls. Restoration after the ordinary 12-month period is a limited petition path and is **not** the operating plan.

## Status vocabulary

- `PASS_EVIDENCE` — repository contains a strong evidence path for the factual issue.
- `IN_PROGRESS` — evidence exists but the chain is not yet complete.
- `OPEN` — required work has not yet been completed.
- `FILING_ACTION` — must be completed in Patent Center / application papers; the proof repository cannot satisfy it by itself.
- `LEGAL_REVIEW` — claim-specific patent-law analysis is required.
- `N_A_PENDING_CONFIRMATION` — probably inapplicable, but must be affirmatively checked.
- `BLOCKED` — cannot responsibly advance until the stated dependency is resolved.

---

# A. Filing-package checkboxes

| Checkbox | Current status | Repository control / next action |
|---|---|---|
| Formal P1 filing receipt reconciled | **OPEN** | Complete `P1/P1_FILING_ANCHOR.md` follow-through; preserve official filing date and certified copy when available. |
| Nonprovisional filed within benefit window | **FILING_ACTION** | Working target `2027-09-16`; do not wait for restoration period. |
| Specific reference to P1 in ADS | **FILING_ACTION** | Nonprovisional ADS must claim benefit of provisional Application No. 64/155,744, filed 2026-09-16, subject to final anchor reconciliation. |
| Correct inventor(s) | **LEGAL_REVIEW** | Maintain human-conception evidence; review inventorship against the actual final claims. Only natural persons may be inventors. |
| AI-assisted inventorship review | **IN_PROGRESS** | Preserve human-origin, correction, architecture, implementation, and decision evidence. AI systems are tools, not inventors. Final inventorship turns on human conception of claimed subject matter. |
| Application Data Sheet | **FILING_ACTION** | Prepare final ADS with inventor/applicant/correspondence/benefit information. |
| Specification | **IN_PROGRESS** | P1 is frozen; nonprovisional specification must be drafted from supported disclosure plus clearly identified later material. |
| At least one claim | **IN_PROGRESS / LEGAL_REVIEW** | Operative candidate set is Claims 1–20 (3 independent). All 20 now have recorded frozen-P1 written-description/priority dispositions consistent with the operative wording; remaining gates include enablement, eligibility, prior art, definiteness, inventorship, disclosure, and filing QA. |
| Abstract | **FILING_ACTION** | Prepare separate abstract, generally one paragraph and no more than 150 words under current USPTO guidance. |
| Drawings when necessary | **IN_PROGRESS** | P1 drawings exist; final claim set must be checked so every necessary claimed feature is adequately shown. |
| Oath / declaration | **FILING_ACTION** | Execute required inventor declaration for the nonprovisional. |
| Filing, search, examination fees | **IN_PROGRESS / FILING_ACTION** | `P1/2026-10-02_NONPROVISIONAL_INITIAL_FEE_CONTROL.md` records the current baseline for 20 claims / 3 independent: $2,000 regular / $730 qualifying electronic small entity / $400 micro, before circumstance-specific fees. Entity status and final page/format QA remain unresolved. |
| DOCX filing / format controls | **FILING_ACTION** | Use current Patent Center formatting rules; description, claims, and abstract should be filed in DOCX to avoid the current non-DOCX surcharge unless a deliberate exception is chosen. |
| Sequence listing / large table / computer listing if applicable | **N_A_PENDING_CONFIRMATION** | Explicitly determine whether any specialized submission requirement applies. Do not silently assume N/A. |

---

# B. Claim-level patentability checkboxes

Every **final** independent and dependent claim must receive a row in `P1/NONPROVISIONAL_CLAIM_READINESS.csv`. The operative candidate control currently contains Claims 1–20, with three independent claims. No claim is READY merely because it has a row.

| Legal / examination issue | Current repo posture | Required proof work |
|---|---|---|
| **35 U.S.C. §101 — statutory category** | **OPEN** | Identify whether each claim is framed as process, machine, manufacture, or composition/improvement as applicable. |
| **§101 — utility** | **IN_PROGRESS** | Link specific, substantial, credible utility to concrete implementations, field use, tests, or operational receipts. |
| **§101 — subject-matter eligibility** | **LEGAL_REVIEW** | For software/AI claims, map the claim as a whole under current USPTO eligibility analysis; identify concrete technical integration rather than relying on novelty alone. |
| **§102 — novelty** | **IN_PROGRESS** | Maintain prior-art register and element-by-element novelty chart. A broad similarity is not enough; check each limitation. |
| **§103 — nonobviousness** | **OPEN / LEGAL_REVIEW** | Test likely combinations of references, reason to combine, and what the claimed arrangement changes technically. |
| **§112(a) — written description** | **PASS_EVIDENCE / FINAL-QA PENDING** | All 20 operative claims now have recorded frozen-P1 support dispositions consistent with current wording. Claims 12–13 were narrowed to cure identified support defects. Preserve the claim-specific controls and perform final dependency/antecedent-basis and filing-text comparison before READY. |
| **§112(a) — enablement** | **IN_PROGRESS** | Link algorithms, flows, schemas, implementation detail, tests, and reproducibility evidence sufficient for the claimed scope without undue experimentation. |
| **§112(a) — best mode** | **OPEN** | Before filing, inventor must identify the best mode known for carrying out the claimed invention and ensure the specification discloses it. |
| **§112(b) — definiteness** | **OPEN / LEGAL_REVIEW** | Define boundaries and terms; remove ambiguous functional language that leaves scope unclear. |
| **§112(f) — functional limitations, if invoked** | **OPEN / LEGAL_REVIEW** | For computer-implemented means-plus-function limitations, identify corresponding structure/algorithm in the specification. |
| **Priority support to P1** | **PASS_EVIDENCE / FINAL-QA PENDING** | All 20 operative claims have a recorded frozen-P1 priority-support disposition consistent with the current claim wording. Claims 12–13 use the P1-safe narrowed wording. This does not clear enablement, drawings, statutory patentability, inventorship, disclosure, or final-file QA. |
| **Drawings support** | **IN_PROGRESS** | Map claim elements to figures where drawings are needed for understanding. Frozen FIGS. 4/8 remain material to Claim 9 drawing reconciliation. |
| **Inventorship per claim** | **LEGAL_REVIEW** | Final inventorship must be checked against who conceived the subject matter of the actual claims. |
| **Material-information / candor review** | **IN_PROGRESS** | Maintain `P1/MATERIAL_INFORMATION_REGISTER.csv`; preserve contrary evidence and potentially material references rather than burying them. |
| **Public disclosure / new-matter review** | **IN_PROGRESS** | Maintain `P1/PUBLIC_DISCLOSURE_REGISTER.csv`; flag public material not clearly supported by P1 before relying on P1 priority. |

---

# C. The evidence chain each serious claim should have

The target is not just "a file mentions it."

For each material claim element, build:

```text
claim limitation
    ↓
P1 disclosure coordinate
    ↓
pre-filing conception / source evidence
    ↓
implementation
    ↓
test or field operation
    ↓
correction / failure history
    ↓
current best implementation
    ↓
figure / algorithm / schema support
    ↓
prior-art comparison
    ↓
material-information review
    ↓
receipt / reproducibility path
```

If one of those links does not exist, record the gap. Do not manufacture a clean chain.

---

# D. Computer / AI-specific CYA controls

Because the invention family is software / AI / distributed-runtime heavy, the proof project must make these issues explicit.

## 1. Human inventorship

Current USPTO guidance applies the ordinary inventorship standard even when AI tools were used. Only natural persons can be inventors.

Repository action:

- preserve human-authored architectural decisions;
- preserve earliest human problem formulations and specific technical solutions;
- preserve corrections where the human rejected, modified, or redirected AI output;
- preserve implementation decisions and tests;
- do not list an AI system as an inventor;
- do not claim that merely operating an AI tool establishes inventorship.

## 2. Algorithms and functional language

For claim limitations that may trigger §112(f), a generic statement such as "software configured to do X" may be insufficient. The specification should expose the algorithm / finite sequence / flow that performs the claimed computer function where required.

Repository action:

- link each functional limitation to a flowchart, finite step sequence, state transition, schema, or other understandable algorithmic disclosure;
- preserve implementation variants;
- identify which structure performs which function.

## 3. Eligibility is separate from novelty

A system can be new and still face §101 eligibility analysis. A §101 argument cannot be replaced by "nobody has done this before."

Repository action:

- identify the concrete technical system;
- identify the computer / network / storage / runtime behavior changed by the claimed arrangement;
- identify data structures, control flows, state transitions, bounded authority, provenance handling, continuity behavior, or other technical mechanisms actually recited;
- keep social value and philosophical goals as context, not substitutes for technical claim limitations.

---

# E. Prior-art and candor controls

The patent-proof repository is adversarial by design. That is an advantage.

A reference that cuts against a broad claim is not an enemy artifact. It is a design input.

For every potentially material reference:

1. preserve the exact source;
2. record publication / priority date when verified;
3. identify which claim elements it appears to teach;
4. identify which elements it does not teach;
5. preserve contrary or inconsistent information;
6. route it for IDS / duty-of-disclosure review when appropriate;
7. never delete it because it makes the claim narrower.

The centralized material-information register includes pre-P1 references requiring limitation-level treatment; those records must stay adverse rather than promotional.

---

# F. Public disclosure / new-matter controls

The public proof repository, outreach, papers, talks, demos, posts, and public code can create patent-timing consequences.

For every meaningful public disclosure, record:

- exact artifact;
- first verified public date if known;
- what technical content was actually disclosed;
- P1 coordinates that support it;
- whether any content appears to be later-added / possible new matter;
- whether the disclosure predates the corresponding nonprovisional filing;
- whether foreign-rights review is needed.

**Do not backfill a P1 priority date onto later technical material merely because it belongs to the same overall project.**

---

# G. Nonprovisional "zero-reconstruction" packet

Before filing review, the repository should let a patent professional move through the record without archaeology.

Minimum front-door packet:

1. `P1/P1_FILING_ANCHOR.md`
2. `P1/NONPROVISIONAL_READINESS.md`
3. `P1/NONPROVISIONAL_CLAIM_READINESS.csv`
4. `P1/P1_SUPPORT_MATRIX.csv`
5. `P1/SKILL_SUPPORT_INDEX.md`
6. `P1/MATERIAL_INFORMATION_REGISTER.csv`
7. `P1/PUBLIC_DISCLOSURE_REGISTER.csv`
8. strongest proof IDs for each final claim element
9. prior-art element charts
10. final-spec support chart
11. final-figure support chart
12. formal filing receipt / priority record
13. final filing receipt after submission

The goal is that counsel or a reviewer should not have to ask:

- Where did this limitation come from?
- Was it in P1?
- When was it first documented?
- Is there an implementation?
- Is there a test?
- What prior art did you already find?
- What contradicts the broadest version?
- Was this already publicly disclosed?
- Which figure / algorithm supports it?
- Which human conceived it?
- What remains unresolved?

Those answers should already have a route.

---

# H. Current gap assessment — reconciled 2026-10-02

- P1 artifact identity is strongly anchored to the exact preserved specification, drawings, signed cover-sheet artifact, and USPTO acknowledgement. The acknowledgement records Application No. `64/155,744`, confirmation `5031`, Patent Center number `81801706`, title, first named inventor, provisional application type, and the $325 filing fee; the **formal USPTO Filing Receipt remains an explicit reconciliation task**.
- The operative candidate claim surface is **Claims 1–20, including 3 independent claims**.
- All 20 operative claims now have a recorded frozen-P1 written-description/priority-support disposition consistent with current claim wording. Claims 12 and 13 were deliberately narrowed after adverse exact-P1 review rather than treating later semantics as P1-supported.
- Claim 12 no longer relies on the unsupported completed-or-rejected-operation taxonomy/suppression breadth; Claim 13 no longer relies on unverified voice/retrieval alternatives.
- This support milestone is **not** a patentability clearance. Enablement, §101, §102, §103, §112(b), §112(f) where relevant, dependency/antecedent basis, drawings, inventorship, best mode, material-information, public-disclosure/new-matter review, and final filing-text QA remain open as applicable.
- Claim 9's general support premise is **not** universal static resume-point invariance. Persistent workstream identity and checkpoint/resume state are distinct. A preserved checkpoint during a paused/non-advancing embodiment may be used only to the extent the exact frozen P1 supports that narrower embodiment.
- Claims 7, 8, and 19 retain heightened exact-filed-page verification flags in the operative claim-readiness control.
- Prior-art work is centralized in `P1/MATERIAL_INFORMATION_REGISTER.csv`; pre-P1 references must receive element-level novelty/obviousness treatment and IDS/materiality review rather than being suppressed.
- Public-disclosure/new-matter review remains open in `P1/PUBLIC_DISCLOSURE_REGISTER.csv`.
- Human inventorship must be resolved against the final claims; AI participation does not replace the natural-person conception analysis.
- Current initial-fee control is preserved in `P1/2026-10-02_NONPROVISIONAL_INITIAL_FEE_CONTROL.md`: for the present 20-total/3-independent claim surface, baseline initial fees are $2,000 regular / $730 qualifying electronic small entity / $400 micro, before circumstance-specific fees. **Entity status remains a blocker before final payment**, and final page/format QA can change the fee calculation.
- Filing papers, DOCX/Patent Center validation, exact-file QA, final hashes/byte lengths, and the zero-reconstruction upload packet remain filing-critical work.

That is the correct current state to expose. **Undeniability means an adversarially checked, reproducible record with every remaining defect visible—not pretending every box is green.**

---

# I. Official control sources

Current procedural/fee controls should be rechecked immediately before filing. Core sources:

- Nonprovisional Utility Patent Application Filing Guide  
  https://www.uspto.gov/patents/basics/apply/utility-patent
- Provisional Application for Patent / 12-month benefit window  
  https://www.uspto.gov/patents/basics/apply/provisional-application
- USPTO Fee Schedule  
  https://www.uspto.gov/learning-and-resources/fees-and-payment/uspto-fee-schedule
- Small / micro entity guidance  
  https://www.uspto.gov/patents/apply/save-on-fees
- MPEP §2103 — patent examination sequence / §§101, 102, 103, 112  
  https://www.uspto.gov/web/offices/pac/mpep/s2103.html
- MPEP §2106 — subject matter eligibility  
  https://www.uspto.gov/web/offices/pac/mpep/s2106.html
- MPEP §2141 — obviousness under §103  
  https://www.uspto.gov/web/offices/pac/mpep/s2141.html
- MPEP §2161 / §2161.01 — §112 requirements for computer-implemented inventions  
  https://www.uspto.gov/web/offices/pac/mpep/s2161.html
- MPEP §2181 — §112(f), including computer-implemented functional limitations  
  https://www.uspto.gov/web/offices/pac/mpep/s2181.html
- MPEP §2001 — duty of disclosure, candor, and good faith  
  https://www.uspto.gov/web/offices/pac/mpep/s2001.html
- USPTO revised inventorship guidance for AI-assisted inventions (Nov. 2025)  
  https://www.uspto.gov/subscription-center/2025/revised-inventorship-guidance-ai-assisted-inventions

## Core rule

> **Every claim gets every checkbox. Every checkbox gets evidence, an explicit gap, or a filing action. Nothing important lives only in somebody's memory.**
