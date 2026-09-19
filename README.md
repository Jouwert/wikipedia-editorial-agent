# wikipedia-editorial-agent

Goals and design for an AI-assisted Dutch Wikipedia editorial workflow — **not** an
implementation.

This repository documents *what the work is for, what it must never do, and how the
responsibility is split between people and agents*. It deliberately contains no source code, no
drafts, no article text and no named subjects. Those belong to a private working environment,
because the material is about living people.

## The real problem

Dutch Wikipedia under-documents people and groups who are marginalised or structurally
underrepresented — not through explicit exclusion, but because mainstream coverage is thin,
concentrated in interviews, regional and specialist media, or simply harder to find. Meanwhile
the effort of checking whether a person meets the inclusion and sourcing standard is
substantial, and easy to get wrong in both directions: writing about someone who should not be
written about, or missing someone well-supported by sources nobody looked for.

That makes it a genuine candidate for AI assistance — and a genuinely dangerous one, because
the failure mode is a living person's reputation.

## Who used it

One operator with a stated editorial mission, using agents for research, source preservation,
drafting support and review. There is no public user base; the workflow is a private editorial
operation with a public output.

## What the workflow is for

1. **Find the overlooked.** Broad, persistent source discovery that does not mistake absence
   from one prestigious outlet family for absence of public significance.
2. **Preserve evidence properly.** A source is not "used" until it is captured at full fidelity
   with provenance, so a later agent can independently reproduce the claim check.
3. **Draft neutrally.** Corrective subject selection, encyclopaedic prose. The distinction is
   absolute.
4. **Keep a human at the gate.** Agents propose; a person decides. Publication is an explicit
   human action, never an agent's conclusion.

## Deployment constraints

- **Living people.** Every procedural choice is subordinate to not causing harm to a subject.
- **Access terms.** Some sources sit behind subscription or licensing terms. The obligation is
  full-fidelity internal preservation for verification — not redistribution, not summarisation
  for reuse.
- **Neutrality is a requirement, not a style.** Advocacy is permitted in choosing *whom* to
  research and forbidden in the prose.
- **One operator.** Review capacity is the bottleneck, so the workflow must reduce the
  reviewer's reading load rather than produce more candidates.

## Trade-offs I would defend

- **Research effort, never evidence standards.** Under-documentation changes how hard we search,
  not what counts as a reliable source. No extra fame, celebrity, award-count or
  conventional-career hurdle is added on top of the documented source gate.
- **Separate judgments.** Source availability, inclusion of personal detail, and article scope
  are decided independently — collapsing them is how bad decisions get made quickly.
- **Compact and correct can be the outcome.** A short, well-sourced biography of someone
  overlooked is a valid result; length is not a proxy for significance.
- **Negative candidates are recorded.** "We looked and it does not hold" is an output worth
  keeping, because it stops the same person being re-researched from scratch.
- **Private drafts, public output.** Working material stays private until a person approves
  publication. The public artifact is the article, not the pipeline.

## What is deliberately omitted

No source code, no prompts, no drafts, no article text, no candidate or subject names, no
source captures, no access credentials or procedures for obtaining them, no reviewer identities,
no agent channel or routing specifics. See `docs/public-private-boundary.md`.

## What is transferable here

The value of this writeup to anyone else is not the workflow — it is the **governance pattern**,
which applies to any AI-assisted work about identifiable people (casework, HR, care, journalism,
research):

1. Declare the mission, including the parts that are deliberately corrective.
2. Separate the corrective search from the prose standard, in writing.
3. Require full-fidelity evidence with provenance before any claim may rest on a source.
4. Keep the inclusion judgment, the privacy judgment and the scope judgment separate, each able
   to stop the work.
5. Put a human at the publication gate, and require proposals to separate "the evidence supports
   X" from "X should therefore be done".
6. State in advance what the system must never be handed.

The pattern is the deliverable. Everything else here is an instance of it.

## Honest status

A private editorial workflow in regular use, with human review and publication gates in place.
It is **not** an autonomous publishing system, and this repository does not describe one. The
hard question — whether a marginalised person is *better served* by a new article at all — stays
with the human editor, where it belongs.
