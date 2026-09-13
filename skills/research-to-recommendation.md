# Skill: Research to Recommendation

## Purpose

Turn a set of sources or research material into actionable marketing recommendations without losing evidence quality along the way. The failure mode this guards against is research that reads well but doesn't tell anyone what to actually do — or worse, a confident recommendation nobody can trace back to a source.

## When to use

Any time the job is "figure out what we should do about X" from a set of inputs — market research, competitive teardown, customer interview notes, analytics exports, a stack of articles. Not a fit for pure creative brainstorming, where the point is volume of ideas rather than evidence-backed conclusions.

## Inputs

- The source material (reports, transcripts, data exports, articles, prior research)
- The specific question the research needs to answer
- Any constraints already known (budget, timeline, channels off the table)

## Process

1. **Extract facts.** Pull out what the sources actually state, each with its source attached. A fact with no attached source doesn't belong in this list.
2. **Separate facts from interpretations.** "Churn increased 12% in Q2" is a fact. "Customers are leaving because onboarding is confusing" is an interpretation — plausible, but not the same category of claim, and it should read differently.
3. **Identify patterns.** Where do multiple independent sources point the same direction? A pattern across three sources is stronger evidence than a strong claim in one.
4. **Identify gaps and uncertainty.** State plainly what the research doesn't cover, and what would need to be true for a recommendation to hold. Don't quietly skip the question the sources didn't answer.
5. **Generate recommendations.** Each recommendation should be a specific action, not a restatement of a finding. "Clicks are down" is a finding; "revise the meta description on these three pages" is a recommendation.
6. **Tie each recommendation to evidence.** Every recommendation should trace back to specific facts or patterns from step 1–3 — not just to "the research."
7. **Identify what requires human judgment.** Flag recommendations that hinge on a business call the research alone can't make (risk tolerance, brand positioning, resourcing) rather than presenting them as though the evidence settles it.

## Rules / guardrails

- Never state a recommendation with more confidence than the underlying evidence supports.
- Never treat an interpretation as a fact, even when it's very likely true.
- If sources conflict, say so — don't quietly pick the one that supports a cleaner narrative.
- Don't fill an evidence gap with a plausible-sounding assumption; name it as an assumption.

## Output format

```
QUESTION
[the specific decision this research needs to inform]

FACTS
- [fact] — Source: [source]
- ...

PATTERNS
- [pattern observed across multiple sources, with which sources support it]

GAPS / UNCERTAINTY
- [what the research doesn't cover, and what would change the answer]

RECOMMENDATIONS
1. [specific action]
   Evidence: [facts/patterns this traces back to]
   Requires human judgment on: [the business call this doesn't settle, if any]

CONFIDENCE
[High / Medium / Low], with the reason
```

## Human review points

- Every recommendation, before it's treated as a decision rather than an input to one.
- Any point where the research is thin but the recommendation is presented with high confidence — that mismatch is the most common failure mode.
- Any recommendation that touches risk, budget commitment, or brand positioning — those are calls for a person who owns that outcome.

## Example invocation

> "Here are the transcripts from six customer interviews and last quarter's churn data. The question is: why are mid-market customers churning after month three, and what should we do about it? Run research to recommendation."

Expected response: the structured output above — facts and patterns clearly sourced, gaps named honestly, and recommendations that read as decisions to make, not just findings to skim.
