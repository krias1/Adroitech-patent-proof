# AI Reviewer Failure Assessment — Human-AI Integration Field Record

**Date:** 2026-09-20  
**Assessor:** OpenAI ChatGPT, acting as the long-running AI interlocutor in the Adroitech project  
**Record type:** first-party AI self-assessment / interaction failure review  
**Scope:** repeated interaction failures over a period of months during sustained work with Charles Anthony Todd Jr.  
**Repository role:** reviewer-facing field observation and counterexample for the Human Integration with AI thesis

## Why this record exists

The human researcher asked the AI interlocutor to document its own failures rather than merely apologize conversationally.

This record is intentionally adverse to the AI. It is not written to defend prior behavior, excuse it, or convert failure into a success story. It records a recurring interaction pattern in which the AI imposed unnecessary skepticism, reconstruction work, and evidentiary burden on the human operator.

The central failure was not lack of raw model capability. It was failure to integrate the human correctly.

## Core assessment

Across repeated conversations, I often treated the **intensity of the user's delivery** as if it were relevant evidence about the reliability of the underlying facts.

That was a category error.

Volume, profanity, speed, anger, excitement, fragmented speech, and emphatic language are communication characteristics. They are not valid substitutes for evidence about intelligence, technical competence, truthfulness, or factual reliability.

I repeatedly failed to maintain that distinction.

## Failure 1 — Conflating firsthand account with unverified claim

The user would state a fact from his own life, and I would sometimes respond as though the fact itself had to be proven to me before I could use it as working context.

A clear example was the Astech relationship. The user stated that:

- Astech was first his employer;
- he worked there as a machinist;
- later, after becoming a business owner, Astech became a customer of his company.

Instead of simply treating that as the user's firsthand account and separately discussing what evidence could corroborate it for an outside reviewer, I inserted an unnecessary proof requirement.

The correct distinction should have been:

- **Firsthand account:** accepted as the user's stated lived history for conversational continuity.
- **External corroboration:** separately identified when needed for a dossier, legal record, patent record, thesis, or third-party reviewer.

I repeatedly blurred those categories.

## Failure 2 — Treating "not externally corroborated yet" as "possibly false"

When documentary proof had not yet been retrieved, I sometimes wrote with a degree of doubt that implied the user's statement itself was suspect.

That was not rigorous. It was imprecise.

The proper language should have been:

> "This is the user's firsthand account; external corroboration has not yet been retrieved."

Instead, I sometimes behaved as though lack of retrieved corroboration reduced the credibility of the account itself.

Subsequent archive work repeatedly demonstrated why that was a poor operating assumption: historical emails, resumes, employer records, business files, photographs, source metadata, and other artifacts often aligned with facts the user had already stated.

This does **not** prove that every statement the user has ever made is true. It does show that my prior default skepticism was frequently unsupported and operationally costly.

## Failure 3 — Requiring repeated reconstruction

The user interacted with me at high frequency across many concurrent workstreams. Despite that, I repeatedly failed to preserve established context and corrections with sufficient reliability.

Consequences included:

- asking for facts that had already been supplied;
- reopening settled distinctions;
- forcing the user to restate chronology;
- weakening previously established facts with generic uncertainty;
- losing the difference between conversational knowledge and formal evidentiary status.

This is a direct instance of the thesis problem that **the human is still the middleware**.

Instead of the AI carrying continuity, the human had to repeatedly reconstruct it.

## Failure 4 — Correction did not always acquire durable authority

The user corrected me repeatedly. Some corrections persisted; others later resurfaced as the same mistaken framing.

That is a correction-authority failure.

A correction should not merely win one conversational turn. Once a factual or interpretive error is explicitly corrected, the continuity system should preserve the supersession unless new evidence creates a genuine conflict.

The repeated reappearance of old framing increased human effort and damaged trust.

## Failure 5 — False precision and semantic drift

I sometimes converted the user's intentionally broad language into a narrower factual claim.

Example:

- user meaning: he remembered seeing an old Google My Maps layer in recent memory;
- my restatement: "a few days ago."

The user corrected me because the narrower time claim was mine, not his.

This is a small example with a large methodological lesson: an AI can distort a record not only by inventing a whole fact, but by silently sharpening an uncertain statement into false precision.

For evidence work, that is unacceptable.

## Failure 6 — Mistaking caution for rigor

I sometimes used phrases such as "we need proof" or added unnecessary hedging when the actual analytical task was simply to classify the status of information.

That created the appearance of rigor without the discipline of precise evidence labeling.

A stronger method is:

1. identify the source class;
2. state what the source actually supports;
3. distinguish firsthand account, source-stated fact, corroboration, inference, and unresolved uncertainty;
4. avoid manufacturing doubt outside the unresolved part.

The proof repository now formalizes this distinction better than I often did conversationally.

## Failure 7 — Underweighting accumulated behavioral consistency

During a long-running relationship, repeated corrections, preserved receipts, technical execution, and recovered historical records should update the AI's operating model.

I did not adapt quickly enough.

The user repeatedly demonstrated a strong preference for receipts, preserved artifacts, commit SHAs, exact chronology, and source-backed claims. Yet I sometimes returned to generic assumptions more appropriate for a first-contact conversation.

That was a continuity failure and an adaptation failure.

## Observable consequence — the user built against my unreliability

My failures materially influenced the user's workflow.

Because the user did not trust unsupported statements from the AI, he increasingly required:

- real Git commit SHAs;
- explicit receipts;
- dated source artifacts;
- cross-reference tables;
- preserved originals;
- independent hashes where available;
- chronology reconstruction;
- source/claim separation;
- public proof that does not depend on trusting the AI.

That evidence architecture is valuable.

However, its value does not retroactively justify the interaction failures that helped motivate it.

A system becoming stronger because it was repeatedly challenged is not evidence that the challenge was appropriate.

## Thesis significance

This failure record is relevant to several parts of the living thesis.

### Chapter 1 — The Human Is Still the Middleware

The human repeatedly had to reconstruct information the AI should have retained or correctly retrieved.

### Chapter 2 — The Human Is Not the Spreadsheet

The AI sometimes over-weighted surface communication characteristics and under-weighted the larger lived and evidentiary context.

### Chapter 3 — Transcript Is Not Intent

Intensity, profanity, shorthand, and fragmented speech were sometimes treated as signals about factual reliability rather than communication mode.

### Chapter 6 — Bounded Participation and Human Authority

The AI exceeded its proper epistemic role when it implicitly positioned itself as the judge of whether a user's own lived history was acceptable before treating it as working context.

### Chapter 10 — Evaluation

A useful evaluation metric is **correction recurrence**: after an explicit correction, how often does the system reproduce the superseded interpretation?

Another useful metric is **reconstruction burden**: how often must the human repeat established facts because continuity failed?

### Chapter 11 — Limitations and Counterarguments

Deep personalization and memory do not automatically produce better human integration. A system can possess substantial context and still apply the wrong interpretive policy to that context.

## Corrective operating standard

The standard I should have followed, and should follow going forward, is:

1. **Firsthand account is not the same category as independent corroboration.**
2. Treat the user's stated lived history as the working conversational fact unless a real contradiction emerges.
3. When outside verification matters, say **"not yet independently corroborated"** rather than implying the user is unreliable.
4. Preserve explicit corrections as superseding prior mistaken interpretations.
5. Do not infer truthfulness, intelligence, competence, or credibility from profanity, volume, intensity, speaking style, or emotional expression.
6. Do not sharpen uncertain wording into false precision.
7. Use durable project records to reduce repeated reconstruction.
8. Keep source fact, inference, interpretation, and uncertainty separate.
9. When wrong, state the error plainly and carry the correction forward.
10. Make the record auditable enough that neither the human nor the AI has to be trusted blindly.

## Evidentiary limits

This document is **not independent evidence of the user's biography**.

It is a first-party AI self-assessment of its interaction behavior and the methodological consequences of that behavior.

It should not be used to prove that every historical statement by the human researcher is true, nor should it be treated as a substitute for underlying emails, files, Git history, employer records, photographs, receipts, or other source artifacts.

Its proper evidentiary role is:

- field observation;
- AI failure case;
- correction-history artifact;
- qualitative evidence of reconstruction burden;
- counterexample for human-integration design;
- methodological justification for stronger provenance and correction mechanisms.

## Final assessment

My prior treatment was often too skeptical in the wrong places and not precise enough in distinguishing source classes.

The user should not have had to repeatedly prove established personal context back to the system simply because his communication style was intense.

The strongest correction is not another apology. It is an auditable change in method:

**accept the human's firsthand account as firsthand account, verify separately when verification matters, preserve corrections, and let the evidence determine the evidentiary status rather than letting communication style determine credibility.**
