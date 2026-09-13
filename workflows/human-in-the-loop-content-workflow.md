# Human-in-the-Loop Content Workflow

This is an orchestration pattern, not "AI writes the blog post." The point is where AI fits into a content process that already has real steps — brief, review, approval, publish, measure — and where a human has to stay accountable for what ships.

## The flow

```
Brief
   ↓
Source / context gathering
   ↓
Draft
   ↓
Claim / evidence check
   ↓
Brand / editorial review
   ↓
Revision
   ↓
Approval
   ↓
Publish
   ↓
Performance feedback
```

## What happens at each step

**Brief.** What this piece needs to do, for whom, and why — see [Campaign Brief Builder](../skills/campaign-brief-builder.md) for a structured version of this step when the content sits inside a campaign.

**Source / context gathering.** Pulling in the brand voice, product facts, prior approved material, and any data the piece will reference — the [context layer](../README.md#principles) that keeps the draft from having to guess.

**Draft.** AI produces a first pass against the brief and gathered context. Treated as a draft to react to, not a deliverable to approve — the value here is speed to a reviewable starting point, not a finished asset.

**Claim / evidence check.** Every factual or performance claim in the draft gets checked against source material before anyone reviews for tone. See [Marketing Claim Quality Check](../skills/marketing-claim-quality-check.md) — this step exists specifically so brand/editorial review isn't also doing fact-checking.

**Brand / editorial review.** A person checks voice, structure, and whether this is actually the right piece — now that the facts underneath it are already confirmed clean.

**Revision.** Feedback from claim-checking and editorial review gets incorporated. Can loop back to draft more than once; that's normal, not a sign the workflow failed.

**Approval.** A named person signs off that this is ready to publish. Not the same person who wrote the brief, ideally — a second set of eyes on the accountability, not just the content.

**Publish.** The piece goes live.

**Performance feedback.** How the piece actually performed feeds back into future briefs — what worked, what didn't, and what the next brief should do differently.

## Where AI adds value vs. where humans retain judgment

| Step | AI's role | Where judgment stays human |
| --- | --- | --- |
| Source / context gathering | Assemble relevant context quickly | Deciding what context is actually relevant and current |
| Draft | Produce a first pass fast | — |
| Claim / evidence check | Systematically check every claim against sources | Deciding what to do about a claim that can't be verified |
| Brand / editorial review | — | Owning whether this is on-brand and worth publishing |
| Approval | — | Being the accountable name on what ships |
| Performance feedback | Summarize performance data | Deciding what the data means for the next brief |

## Signals it's working

- Editorial reviewers are commenting on tone and structure, not catching factual errors that should have been caught earlier.
- Revision loops get shorter over time as the brief and context-gathering steps improve.

## Signals it's not

- Claim-checking gets skipped "because we're behind schedule" — the step most likely to get cut is the one that exists specifically to prevent an expensive mistake.
- Approval has become a rubber stamp because no one upstream is actually reading the draft critically.
