# Research to Action Workflow

An end-to-end pattern for turning research into a decision that actually gets acted on and measured — not just a synthesized document that sits in a shared drive.

## The flow

```
Sources / context
      ↓
Evidence extraction
      ↓
Synthesis
      ↓
Recommendation generation
      ↓
Human review
      ↓
Action plan
      ↓
Measurement
```

## What happens at each step

**Sources / context.** Whatever the research draws from — interviews, analytics, competitive material, prior research, support tickets. Quality of the whole workflow is bounded by quality of this step; no amount of synthesis fixes thin sources.

**Evidence extraction.** Pull out discrete facts, each attached to its source. This is where AI adds real value — it can go through volume of material a person would reasonably skim, without getting tired or bored partway through.

**Synthesis.** Find the patterns across the extracted evidence: where multiple sources agree, where they conflict, and what's genuinely uncertain. AI is useful here for surfacing patterns across a large set; it's not the step where the final call gets made.

**Recommendation generation.** Turn synthesized patterns into specific, actionable recommendations — each one traceable back to the evidence that supports it. See [Research to Recommendation](../skills/research-to-recommendation.md) for the detailed skill this step runs.

**Human review.** The recommendations get checked against three questions: does the confidence level match the evidence, does the recommendation actually follow from the synthesis, and is there a claim in here that would be a problem if it turned out to be wrong? This is not a formality step — it's where accountability for the decision actually sits.

**Action plan.** The accepted recommendation becomes a specific plan: who does what, by when, with what resources. A recommendation that never turns into an owned action plan didn't accomplish anything, regardless of how good the research was.

**Measurement.** Define upfront how the team will know whether the action worked — and revisit it. This closes the loop back to future research: what did we learn, and what should the next round of research check.

## Where AI adds value vs. where humans retain judgment

| Step | AI's role | Where judgment stays human |
| --- | --- | --- |
| Evidence extraction | Process volume, attach sources | Deciding which sources are trustworthy enough to include at all |
| Synthesis | Surface patterns and conflicts across sources | Deciding which pattern actually matters for this decision |
| Recommendation generation | Draft specific, evidence-traced recommendations | Accepting the recommendation as the actual plan |
| Human review | — | All of it — this step exists specifically to keep a person accountable |
| Action plan | Draft a plan structure from the accepted recommendation | Assigning ownership, resourcing, and timeline realistically |
| Measurement | Track and report against the defined metric | Deciding what the result means and what to do next |

## Signals it's working

- Research produces decisions with an owner and a date attached, not just a synthesized writeup.
- The measurement step actually gets revisited — not just defined and forgotten.

## Signals it's not

- Recommendations get accepted without anyone checking the evidence trail behind them.
- The same research gets re-run because no one wrote down what was already learned, or what the next question should be.
