# Architecture — conceptual design

A description of how the work is *organised*, with no implementation detail and no procedures
that depend on access terms.

## The editorial pipeline in one paragraph

Candidates come from broad source discovery. A candidate is only assessed once the sources
supporting it are preserved at full fidelity with provenance. Verification, drafting and review
then proceed as separate judgments, each able to stop the candidate. Publication is a human
action performed in the user's own space first, and in the main encyclopedia only under a
separate, explicit approval. Everything that happened is recorded so the next pass starts from
knowledge rather than from scratch.

```
   broad source discovery
            │
            ▼
   candidate shortlist ──── rejected? ──▶ recorded with reasons (negative result kept)
            │
            ▼
   evidence preservation      (full fidelity + provenance + integrity check)
            │                  └─ not preserved  ──▶ not admissible; no claim may rest on it
            ▼
   verification
     ├── is there enough independent coverage for the inclusion standard?
     ├── is each personal detail supported exactly, with no inference?
     └── scope: what belongs in the article, and what does not?
            │
            ▼
   draft (neutral, proportionate, source-grounded)
            │
            ▼
   human review  ──────── objection ──▶ revise or reject (recorded)
            │
            ▼
   draft space publication (user space)  ── human action, verified by read-back
            │
            ▼
   main-space publication  ── separate explicit approval required
            │
            ▼
   monitoring of the live article (tracked, with reviewer-visible state)
```

## The five design commitments

### 1. Evidence before assessment

A source is not admissible until it exists in the working environment complete, with its
public reference, acquisition metadata, integrity hash and a check that the capture is the
real article and not a headline, lead or paywall stub. If full preservation fails, the source is
marked as not preserved and **no claim may rest on it** — the workflow does not proceed on a
partial capture.

This is a licensing and verification decision at the same time: preservation exists so a later
person can check the claim, not so content can be reused.

### 2. Separate judgments

Three decisions that are easy to merge, and dangerous when merged:

- **Does enough independent coverage exist?** (inclusion standard)
- **Should this personal detail appear at all?** (dignity and privacy)
- **What is in scope for this article?** (proportion)

Each can stop the candidate independently. A subject who clearly meets the inclusion standard
can still lose a detail on privacy grounds; a well-sourced article can still be too long.

### 3. Corrections go in the subject search, not the standard

Because under-documentation is structural, the effort of searching is deliberately disproportionate:
broad, persistent, across national and regional press, public broadcasting, specialist and
community media, with explicit instruction not to treat absence from any one outlet family as
absence of significance. **The gate itself is not relaxed.**

### 4. Human authority is explicit and reversible

Agent proposals are proposals. Research-correct suggestions have been rejected by the editor on
editorial grounds, and that is the intended behaviour: the workflow requires proposals to
separate "the research supports X" from "X should therefore be done". Publication is never the
end of an agent chain.

### 5. Multi-agent operations serve review, not volume

Where agents are used together, the design principle is one capable agent by default, with
additional roles formed only when a task genuinely crosses specialties — research, verification,
drafting and independent review are separate roles, and a review role must not be the same agent
that produced the draft. Roles are assigned minimally scoped access to the private working
material; a reviewing agent receives the preserved evidence, not the source credentials.

## Boundary between the private workflow and the public output

| Stays private | Becomes public |
|---|---|
| Candidates, drafts, source captures, review threads | The published article, if and when approved |
| Agent roles, channel and routing specifics | The editorial principles (this repository) |
| Reviewer identity and decision history | The fact that a human decided |

## Failure modes this design is built against

- **A claim resting on an unpreserved source** → inadmissible by rule.
- **Inference drifting into assertion** (roles, dates, residence, affiliation) → exact support
  required for living-person claims.
- **Prose drifting toward advocacy** → neutrality is a requirement, checked at review.
- **Volume outpacing review** → candidates are not produced faster than they can be judged.
- **Silent loss of earlier decisions** → rejected candidates and their reasons are recorded.
