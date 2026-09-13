# AI Deployment Checklist

A pre-launch check for any AI marketing workflow moving from prototype toward real use. Meant to be answered in writing, by the workflow owner, before deployment — not discussed vaguely in a meeting and waved through.

## Before deployment

- [ ] **Is the business problem clearly defined?** Not "we could use AI here" — a specific, named problem this workflow solves.
- [ ] **Is AI actually necessary?** Would a simpler process, template, or rule-based tool solve this just as well?
- [ ] **What data does the workflow access?** Named explicitly — not "whatever's needed."
- [ ] **Is sensitive or confidential information involved?** Customer data, unreleased plans, internal-only material, anything regulated.
- [ ] **What can the model get wrong?** Specific failure modes, not a general "AI can hallucinate" disclaimer.
- [ ] **What is the consequence of failure?** If the worst realistic output shipped without anyone catching it, what actually happens?
- [ ] **Is human review required?** And is it actually built into the workflow, not just assumed to happen informally.
- [ ] **Who owns the output?** A named person accountable for what this workflow produces — not "the team."
- [ ] **How is quality evaluated?** Defined before launch, not improvised after something goes wrong.
- [ ] **How is feedback incorporated?** A real path for "this output was wrong" to change how the workflow runs next time.
- [ ] **What happens when the model cannot complete the task?** A defined fallback, not a silent failure or a confidently wrong guess.
- [ ] **Is the workflow documented well enough for another person to run it?** If it only works when its creator is available to explain it, it isn't ready.

## How to use this

Answer every item honestly before deployment — a checklist with unanswered or hand-waved items isn't complete just because it exists. Any item answered with "not sure" or "we'll figure it out" is a signal the workflow belongs in [Workflow Readiness Assessment](../workflows/workflow-readiness-assessment.md) as a GAP, not a DEPLOY.

Related: [Human Review Framework](./human-review-framework.md) for deciding what level of review a given workflow needs, and [Quality Control Checklist](./quality-control-checklist.md) for what to check in the output itself.
