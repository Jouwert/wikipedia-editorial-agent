# Excerpt — where the human stays in the loop (and why agents do not publish)

**Scope:** authority, review separation, multi-agent roles

## The authority rule

Agents research, preserve evidence, verify, propose drafts and review each other's work.
**A person decides what is published.** Publication is a human action, not the terminal step of
an agent chain.

Concretely, within the private workflow: uploading a draft to the editor's own user space
requires his standing instruction; publishing to the main encyclopedia always requires a
separate, explicit approval. Neither is inferred from an agent's confidence.

## Proposals must separate two different sentences

A recurring failure in agent-assisted editorial work is collapsing these:

- "the sources support X"
- "X should therefore be done"

They are different claims with different evidence. The workflow requires proposals to state
them separately, because research-correct suggestions have been **rejected by the editor on
editorial grounds** — and that is the intended behaviour, not a defect.

Rejections are recorded. The record is what stops the same proposal being re-made by a fresh
session that lacks the context for why it was declined.

## Review separation in multi-agent work

Where several agents are used, the design principle is deliberately conservative:

- **One capable agent is the default.** A second role has to justify its coordination cost.
- **Research, verification, drafting and review are separate roles**, and the reviewing agent is
  never the agent that produced the draft.
- **Least access.** A reviewing agent receives the preserved evidence it needs — not the source
  credentials, not the browser session, not the account.
- **The reviewer is asked to object.** An agent asked to approve will approve; the useful
  instruction is to find what is wrong with the draft.

## The honest scale

This is a single-operator editorial workflow, not a fleet. The multi-agent structure exists
where independent review genuinely adds value — in checking a claim against a preserved source,
and in catching the drift from neutral prose toward advocacy. Where it adds nothing, it is not
used.

## Why this excerpt is here

It is the clearest statement in this repository of a position that is easy to state and hard to
hold: **AI can do most of the work, and must not do the last step.** The design is judged by
whether it survives contact with a reviewer who disagrees with it.
