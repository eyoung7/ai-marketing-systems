# Workflow Spec Template

A reusable template for specifying a workflow *before* building it — the point is to force clarity on scope, ownership, and failure handling while it's still cheap to change, rather than discovering the gaps after it's in daily use.

Run a filled-out spec through [Workflow Readiness Assessment](../workflows/workflow-readiness-assessment.md) before treating it as ready to deploy.

---

## Workflow Name

*A short, specific name — not "the AI thing for X."*

## Problem

*What job is this actually solving, for whom, and why does it matter enough to build?*

## User

*Who runs this workflow, or who it serves — be specific about the role, not "the team."*

## Trigger

*What starts this workflow — a scheduled run, a specific event, someone kicking it off manually?*

## Inputs

*What the workflow needs to run: data, documents, context, prior outputs.*

## Context Required

*What background knowledge (brand, product, audience, prior decisions) the workflow depends on to produce good output — and where that context actually lives.*

## AI Responsibilities

*What the model is doing in this workflow, stated specifically — "drafts X from Y," not "helps with X."*

## Human Responsibilities

*What a person is doing, and why it has to be a person — review, approval, judgment calls the workflow doesn't make.*

## Steps

*The actual sequence, numbered. If this can't be written as a clear sequence yet, the workflow isn't specified enough to build.*

## Output

*What this workflow produces, in what format, delivered where.*

## Guardrails

*What the workflow should never do — scope limits, topics it shouldn't touch, data it shouldn't access.*

## Failure Modes

*What specifically can go wrong, and what happens when it does — not "AI can make mistakes," but the actual ways this workflow can fail.*

## Evaluation

*How you'll know, on an ongoing basis, whether this workflow is doing a good job.*

## Deployment Status

*DEPLOY / GAP / DEMO — see [Workflow Readiness Assessment](../workflows/workflow-readiness-assessment.md). If GAP, name what has to be true to move to DEPLOY.*

## Owner

*The specific person accountable for this workflow working correctly and being maintained.*

## Dependencies

*Other systems, tools, data sources, or workflows this relies on.*

## Open Questions

*What's still unresolved — don't leave this section blank just to look finished.*
