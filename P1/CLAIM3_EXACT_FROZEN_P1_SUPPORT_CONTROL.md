# Claim 3 Exact Frozen-P1 Support Control

**Control date:** 2026-10-01
**Priority anchor:** U.S. Provisional Application No. 64/155,744, filed/acknowledged 2026-09-16
**Exact specification:** `ADROITECH_PERSON_SPECIFIC_AI_RUNTIME_PROVISIONAL_SPECIFICATION_2026-09-16.pdf`
**Exact specification SHA-256:** `267628a51cc938dbcbd724af4f7f9b0a1ad58532f32b738b12a36490c2cff00e`
**Exact specification byte length:** `35,893`

## Operative Claim 3

Claim 3 depends from Claim 1 and recites that selecting the bounded subset is constrained by an inference-resource budget comprising at least one of a token budget, byte budget, record-count budget, node budget, latency budget, or inference-cost budget.

## Exact frozen-P1 support

The independently recovered, hash-matched 12-page P1 specification directly supports the budget-constrained selection mechanism.

- p.2 Summary: bounded connected-record retrieval and context relevance expressly include an `inference resource budget` among the selection controls.
- p.3 FIG. 9 description: `minimal current world-slice selection under a resource budget`.
- p.5 §7 Dynamic Relevance Determination: candidate-context activation/relevance expressly includes `resource budget` as a factor.
- p.5 §8 Bounded World-Slice Construction: after candidate context is ranked, the system constructs a bounded current world slice and the selection algorithm may enforce a maximum `token, byte, node, edge, record, cost, latency, or privacy-exposure budget`.

## Limitation disposition

| Claim 3 limitation | Exact frozen-P1 coordinate | Disposition |
|---|---|---|
| bounded-subset selection constrained by an inference-resource budget | p.2 Summary; p.5 §§7-8 | DIRECT |
| token budget | p.5 §8 | DIRECT |
| byte budget | p.5 §8 | DIRECT |
| record-count budget | p.5 §8 (`record` maximum) | DIRECT; claim wording expresses the disclosed record maximum as a count |
| node budget | p.5 §8 | DIRECT |
| latency budget | p.5 §8 | DIRECT |
| inference-cost budget | p.5 §8 (`cost` maximum), read with p.2 `inference resource budget` | DIRECT WITH TERMINOLOGY CONTROL |

## Breadth controls

1. Claim 3 remains tied to Claim 1's bounded current-world-slice selection. The P1 support does not establish a generic right to every resource-budgeted AI operation.
2. `record-count budget` is controlled to the disclosed maximum-record budget; do not broaden it into unrelated database cardinality limits.
3. `inference-cost budget` is controlled to the disclosed cost maximum used in bounded current-world-slice selection under the expressly disclosed inference-resource budget. It does not establish every possible monetary, compute, energy, or provider-billing optimization.
4. The exact P1 additionally discloses edge and privacy-exposure budgets, but their presence does not enlarge the current Claim 3 beyond its recited alternatives.
5. Later implementation or drafting evidence cannot repair or enlarge P1 priority.

## Gate consequence

Claim 3's §112(a) written-description mapping and P1 priority support are controlled against the exact frozen specification. This does not establish enablement at every conceivable budget implementation, novelty, nonobviousness, eligibility, definiteness, inventorship, best mode, or filing readiness.

Remaining gates include §101, §102/§103, enablement/commensurate scope, §112(b)/(f), inventorship/best mode, material-information/public-disclosure review, drawing inspection (including frozen FIG. 9), and final filing-artifact QA.
