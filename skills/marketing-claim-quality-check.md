# Skill: Marketing Claim Quality Check

## Purpose

Review marketing copy for unsupported claims, inconsistent metrics, bad math, weak evidence, ambiguity, or wording that overstates what the source material actually supports. This is a quality gate, not a style or voice edit.

## When to use

Run this on anything making a factual, performance, or competitive claim before it goes external: landing pages, case studies, sales one-pagers, social copy, press materials, pitch decks. Skip it for copy that's purely descriptive or brand-voice-only, with no claim to verify.

## Inputs

- The draft copy to review
- The source material each claim should trace back to (data, a case study, a customer quote, a spec sheet, a report)
- If no source material is provided: say so explicitly rather than assuming the claims are supported

## Process

1. **Extract every claim.** Pull out each factual, quantitative, or comparative statement as its own item — don't evaluate the copy as a whole.
2. **Distinguish fact from recommendation.** A source metric is a fact; "this means you should X" is an interpretation layered on top of it. Both can be reasonable, but they fail differently — flag interpretive leaps separately from factual errors.
3. **Distinguish associated value from generated value.** "Customers using this saw a 20% lift" is not the same claim as "this generated a 20% lift" — the first allows for other contributing factors, the second asserts causation. Flag claims that assert causation the source doesn't establish.
4. **Cross-check every number.** If the same metric appears more than once — in this document or against material provided for comparison — confirm it's identical every time. A number that drifted between two mentions is a finding, not a rounding error to wave through.
5. **Flag unsupported superlatives.** "Fastest," "best," "industry-leading," "most trusted" — these need a named, checkable source. If the source material doesn't support the superlative, flag it, even if it's a claim marketing has used before.
6. **Check the math.** Percentages, totals, and derived stats should actually compute from the numbers given. Don't assume a stat is correct because it's stated confidently.
7. **Identify claims requiring evidence that isn't provided.** Not every gap means the claim is false — it means it's currently unverifiable, and that distinction matters in the output.

## Rules / guardrails

- Never silently "fix" a claim by inventing supporting evidence, softening language on your own judgment call, or assuming a plausible source exists. Report the gap; don't paper over it.
- Don't approve legal, regulatory, or compliance risk. Flag it for a human reviewer with that authority — don't clear it yourself.
- Don't rewrite voice or tone. A claim can be phrased in the brand's voice and still be flagged if it's unsupported; fixing the claim's accuracy and fixing its style are separate jobs.
- If no source material was provided at all, say so up front — the review is structural only (internal consistency, math, absolute language) and cannot confirm factual accuracy.

## Output format

```
FLAGGED CLAIMS
1. "[exact quote]"
   Issue: [unsupported / inconsistent number / bad math / absolute language /
           unsupported comparison / causation not established / missing disclaimer]
   Why: [one line — what's missing or what conflicts]
   Suggested fix: [a version that's still strong copy, but defensible]

CLEAN
- Claims that were checked and are adequately supported by the provided source
  material, so a reviewer doesn't have to re-verify everything from scratch.

CONFIDENCE
[High / Medium / Low] — [what would raise or lower it, e.g. "no source material
was provided, so this only caught structural and internal-consistency issues,
not factual accuracy"]
```

## Human review points

- Any flagged claim tied to legal, regulatory, or compliance exposure — a person with that authority decides, not this skill.
- Any "CLEAN" claim where the source material itself is old, from a small sample, or otherwise fragile — the skill checks traceability, not whether the underlying data is still good.
- The overall confidence rating, before this review is treated as a sign-off.

## Example invocation

> "Here's the draft one-pager for [product]. Here's the case study and the analytics export the stats are pulled from. Run the claim quality check before this goes to design."

Expected response: a structured review in the format above — not a rewritten one-pager, and not a claim marked clean because it "sounds right."
