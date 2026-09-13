# Human Review Framework

Not every AI output needs the same level of scrutiny. Applying heavy review to low-stakes output wastes time and trains people to skip the checklist; applying light review to high-stakes output is how mistakes ship. This framework sets the review level based on risk, not on how busy the reviewer happens to be that day.

## The three levels

### Low-risk: human spot-check

**What it covers:** output that's easy to reverse, low-visibility, and wrong in a way someone would likely catch downstream anyway.

**Review:** a person periodically samples output for quality, rather than reviewing every instance before it's used.

**Marketing example:** AI-drafted internal meeting notes summarized from a recorded call, used for the team's own reference.

### Medium-risk: human approval before external use

**What it covers:** output that's visible externally or influences a decision, but where a factual or tonal error is embarrassing rather than damaging, and there's time to catch it before it matters.

**Review:** a named person reviews and explicitly approves each output before it's used — not a sample, every instance.

**Marketing example:** a drafted social post, a blog draft, an internal research summary that will inform a planning decision.

### High-risk: AI assists, human owns the judgment

**What it covers:** output tied to claims about performance or competitors, customer-facing commitments, anything with legal or compliance exposure, or anything where being wrong damages trust.

**Review:** AI can draft, research, and structure — but a specific accountable person makes the actual call, and that person's judgment is the deciding factor, not the AI's confidence.

**Marketing example:** a customer-facing case study with performance claims, a comparison against a named competitor, anything referencing pricing or contractual terms.

## Choosing a level

Ask two questions about the output:

1. **If this is wrong and no one catches it, what happens?** Minor annoyance → low-risk. Embarrassing but fixable → medium-risk. Real damage to trust, legal exposure, or a customer relationship → high-risk.
2. **How reversible is it once it's out?** An internal doc can be corrected quietly. A published claim or a sent customer email often can't be fully walked back.

When in doubt, review at the higher level. The cost of over-reviewing a low-stakes piece is a few minutes; the cost of under-reviewing a high-stakes one is much larger and usually not yours alone to absorb.

Related: [AI Deployment Checklist](./ai-deployment-checklist.md) for setting review requirements before a workflow launches, and [Quality Control Checklist](./quality-control-checklist.md) for what the reviewer is actually checking at each level.
