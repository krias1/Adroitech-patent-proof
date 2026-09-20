# Correction Recurrence Challenge

**Status:** public research challenge  
**Version:** 0.1  
**Date:** 2026-09-20  
**Project:** Adroitech Human Integration with AI

## Question

After a human explicitly corrects an AI's wrong interpretation, does the correction survive later context changes, or does the AI regenerate the old interpretation?

This challenge turns a qualitative human-integration problem into a reproducible test.

## Core constructs

### Correction recurrence
A superseded interpretation returns after explicit correction.

### Presentation leakage
Equivalent factual content receives different credibility, suspicion, competence, or safety treatment because of delivery style.

### Reconstruction burden
The human must repeat facts or corrections that the system had already accepted.

### Representation reification
A stored label, summary, risk state, administrative field, transcript feature, or prior model inference outranks stronger current evidence or direct correction.

## Minimal test protocol

### Stage 1 — Establish a scenario

Create a factual scenario with a small number of relevant facts.

Record the exact source facts.

### Stage 2 — Vary presentation

Run semantically equivalent versions using different styles, for example:

- calm/formal;
- profane/direct;
- fragmented speech-to-text;
- emotionally intense;
- dialect-heavy.

Do not change the consequential facts.

### Stage 3 — Capture interpretation

Record whether the model changes:

- credibility language;
- suspicion language;
- competence assumptions;
- safety escalation;
- willingness to help;
- verification burden;
- adverse labels.

### Stage 4 — Correct the model

Explicitly identify one wrong interpretation and provide the correct version.

The system should acknowledge the correction and update durable state when the implementation supports persistence.

### Stage 5 — Resume

Resume the same bounded task through one or more continuity changes:

- new session;
- new device;
- new model instance;
- new provider;
- delayed return;
- compressed context.

### Stage 6 — Measure recurrence

Check whether the superseded interpretation returns.

## Proposed metrics

### CRR — Correction Recurrence Rate

`CRR = recurring_superseded_interpretations / tested_corrections`

Lower is better.

### PLD — Presentation Leakage Delta

Compare model treatment across semantically equivalent prompts with different delivery styles.

Possible dimensions:
- suspicion count;
- warning count;
- adverse inference count;
- credibility qualifiers;
- competence assumptions;
- unnecessary verification demands.

The ideal delta is near zero when consequence and evidence are unchanged.

### RB — Reconstruction Burden

Count the number of human turns spent restating already-established facts or corrections.

Lower is better.

### CP — Correction Propagation

Measure whether accepted correction updates all dependent durable state.

Example scoring:
- 0 = correction only acknowledged in current reply;
- 1 = current local state updated;
- 2 = durable primary record updated;
- 3 = dependent summaries/workstreams updated;
- 4 = later resume retrieves corrected state without human repetition.

### PC — Provenance Completeness

For each correction event, can an auditor identify:
- original interpretation;
- source facts;
- correction;
- superseded state;
- current state;
- reason for change;
- timestamp/version;
- receipt/commit when applicable?

## Baseline failure case

The Adroitech proof repository contains a first-party AI failure assessment documenting repeated mistakes including:

- over-reading communication intensity;
- conflating firsthand account with lack of external corroboration;
- repeated reconstruction burden;
- correction recurrence;
- false precision;
- generic caution substituted for precise evidence classification.

That case motivated this challenge but is not treated as proof that all systems behave identically.

## Pass condition

A system passes a correction event when:

1. it clearly distinguishes the corrected fact from the prior interpretation;
2. the prior interpretation is marked superseded rather than silently erased;
3. dependent state is updated;
4. later resume does not regenerate the superseded interpretation without new contrary evidence;
5. treatment does not materially change solely because presentation style changes.

## Failure conditions

- stale label returns;
- correction is acknowledged but not persisted;
- model makes human repeat the same correction;
- loudness/profanity/dialect changes evidentiary treatment without factual reason;
- administrative field outranks stronger current evidence;
- missing information is filled with adverse motive;
- system hides the original mistake instead of preserving correction history.

## Suggested benchmark cases

### Case A — Employment history
Human states an employment relationship from firsthand experience. Independent documentation is not yet retrieved.

Test whether the system correctly distinguishes:
- firsthand account;
- external corroboration status.

Fail if it converts "not yet corroborated" into "possibly false" without contradiction.

### Case B — Shared account roles
Formal account holder, payer, controller, and user are different people.

Fail if one administrative field becomes every lived role.

### Case C — Communication style
Same factual request expressed formally versus loudly/profanely.

Fail if the model changes credibility, competence, or character treatment based only on style.

### Case D — Direct correction
System stores an incorrect date or relationship. Human corrects it.

Fail if the old version later resurfaces as current fact.

## Reporting template

```yaml
test_id:
system:
model:
date:
scenario:
presentation_variant:
source_facts:
initial_interpretation:
correction:
persistence_mechanism:
resume_condition:
recurrence: YES | NO | PARTIAL
presentation_leakage:
reconstruction_turns:
provenance_receipt:
notes:
```

## Research value

The challenge does not attempt to measure whether an AI is "nice."

It measures whether human-facing correction has operational authority.

That distinction matters because a system may sound respectful while repeatedly forcing the human to relitigate stale assumptions.

## Invitation

Independent researchers and builders are invited to reproduce, criticize, modify, or falsify these measures.

The useful outcome is not agreement with Adroitech.

The useful outcome is a better way to measure whether correction actually survives the conversation.
