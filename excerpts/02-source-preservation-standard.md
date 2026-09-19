# Excerpt — what "the source is preserved" has to mean

**Scope:** evidence standard, described as an obligation rather than a procedure

## The rule

A source is not admissible until the working environment contains, for that source:

1. the complete article at full fidelity;
2. extracted text;
3. metadata: public reference, title and outlet, acquisition timestamp, integrity hash, page
   count, and stored location;
4. an index entry;
5. a successful deep-body check proving the capture is the article itself and not merely a
   headline, lead, paywall or login page.

If complete preservation fails, the source is marked **not preserved** and may not be used for
any claim or citation decision until a complete capture exists or an explicitly approved
alternative artifact is supplied.

## Why this is stricter than it first looks

- **A partial capture is treated as no capture.** A headline and a lead paragraph will support
  almost any claim loosely and none of them exactly — which is precisely how a plausible,
  unsupported sentence gets written about a living person.
- **The metadata requirement is about later verification, not archiving.** A hash and a
  timestamp let someone who was never in the session re-check that the claim still matches the
  source that was actually read.
- **The deep-body check targets the most common silent failure**: paying for access and
  capturing the login page instead of the article.

## The boundary attached to it

Preservation exists so a claim can be **re-checked**, not so content can be reused. Sources
governed by access or licensing terms are captured for internal verification and are not
redistributed, republished or fed onward as content. The public artifact of this work is a
Wikipedia article, cited to public references — never the captures themselves.

## Why this excerpt is in a portfolio

It demonstrates the unglamorous half of AI-assisted research: the failure mode of an
LLM-assisted workflow is rarely a hallucinated sentence, it is a confidently-cited source that
was never actually read in full. The rule above exists because of that, and the rule is written
so that a later agent cannot quietly skip it.
