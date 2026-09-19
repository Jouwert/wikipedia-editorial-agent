# Goals and non-goals

## Why this repository exists

To document the **intent and the boundaries** of an AI-assisted Dutch Wikipedia editorial
workflow: what problem it addresses, how responsibility is divided between people and agents,
and — most importantly — the rules it must never break while writing about living people.

This is a design and governance document. It is not a technical implementation and does not
describe one.

## Goals

1. **Increase visibility of underrepresented people and groups** on Dutch Wikipedia, without
   weakening any sourcing or neutrality rule to do so.
2. **Preserve evidence at full fidelity with provenance**, so any claim can be independently
   re-checked later by someone who was not in the original session.
3. **Draft neutral, proportionate, verifiable prose** — from a deliberately corrective subject
   choice.
4. **Reduce the reviewer's load**, not increase the volume of candidates. A private editorial
   operation is bottlenecked by human judgement, and tooling should respect that.
5. **Keep a human decision at every consequential step**, especially publication.
6. **Record the negative results** — candidates checked and rejected — so the same work is not
   repeated blindly.

## Non-goals

- **Not an autopublisher.** No agent decides that an article should exist publicly.
- **Not advocacy in prose.** Bias in subject selection is intentional and declared; bias in
  article text is prohibited.
- **Not a fame filter.** No additional notability hurdles are invented on top of the documented
  source standard.
- **Not a data-mining operation.** Nothing about living people is collected for its own sake;
  collection is tied to a specific, reviewable editorial question.
- **Not a reusable scraping recipe.** Access-governed sources are described as obligations, not
  as instructions to copy.

## The rule that governs everything else

> Advocacy in deciding **whom to research** is central to the mission.
> Advocacy in **article prose** is not permitted.

Everything downstream — source preservation, verification, drafting, review — exists to keep
those two statements simultaneously true.

## How to tell whether this workflow is working

1. Does a published article survive review as neutral and adequately sourced?
2. Could a later, independent agent reproduce the evidence check from the preserved artifacts?
3. Was every subject treated as a person whose dignity outranks the project's output target?
4. Did a human make every publish decision?
5. Are rejected candidates recorded, with reasons, rather than silently dropped?

If an optimisation improves throughput but weakens any of those, it is not an improvement.
