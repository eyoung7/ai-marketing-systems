# Workflow Readiness Assessment

A framework for deciding whether an AI marketing workflow should be **deployed**, treated as a **gap** to close, or left as a **demo** — instead of defaulting to "it worked once, ship it" or "it's not perfect, kill it."

Most AI workflow failures aren't model failures. They're readiness failures: a workflow that works in a demo gets pushed into daily use before anyone checked whether it's reliable, governed, or owned. This framework is the check that's supposed to happen first.

## The three outcomes

**DEPLOY**
Useful enough, reliable enough, governed enough, and operationally clear enough for repeat use. Someone owns it, failure modes are known, and quality is being evaluated on an ongoing basis — not just at launch.

**GAP**
A promising concept blocked by something specific and nameable: missing context, missing integrations, missing data, unresolved reliability issues, unclear permissions, no workflow owner, or no evaluation method yet. The point of calling it a GAP instead of a DEMO is that it names what has to be true before this can move to DEPLOY.

**DEMO**
Useful primarily as a prototype or illustration of what's possible — a proof of concept, a conference talk example, a "here's the art of the possible" — but not yet suitable for operational, unsupervised use. Not a failure. A demo that never becomes a workflow can still be a good demo.

## Evaluation criteria

Run each candidate workflow through all eleven questions. The goal isn't a single score — it's forcing a specific answer to each question instead of one general impression of "does this feel ready."

| Criterion | Question to answer |
| --- | --- |
| Business value | Does this save meaningful time, improve quality, or enable something that wasn't possible before — for a real, recurring need? |
| Frequency / repeatability | Is this something the team will actually do again, or a one-time task dressed up as a workflow? |
| Quality requirements | How wrong can the output be before it causes real damage — and how would anyone know if it drifted? |
| Data sensitivity | What does this workflow touch — public information, internal-only material, or something regulated or customer-sensitive? |
| Required context | Does the workflow have reliable access to the context it needs, or does quality depend on someone remembering to paste the right thing in? |
| Human judgment required | Where does a person need to be in the loop — and is that actually built into the workflow, or just assumed? |
| Failure impact | If this workflow produces a bad output and no one catches it, what actually happens downstream? |
| Integrations / dependencies | What systems, data sources, or tools does this rely on, and how fragile is that dependency? |
| Ownership | Who is responsible for this workflow working correctly, being updated, and being retired if it stops earning its place? |
| Evaluation method | How will anyone know, on an ongoing basis, whether this workflow is still doing a good job? |
| Adoption friction | Realistically, will people use this as designed, or will they route around it? |

## Decision structure

This is a lightweight, judgment-informed decision — not a scoring formula, and it doesn't pretend to be one. A workflow with a hard "no" on ownership or failure impact doesn't get deployed regardless of how well everything else scores; those two are gating criteria, not inputs to an average.

```
For each criterion: answer honestly, in writing, before discussing readiness.

If ownership is undefined            → GAP (name who needs to own it)
If failure impact is high and
  human review isn't built in         → GAP (design the review step first)
If data sensitivity is high and
  the workflow's access isn't scoped  → GAP (fix access before anything else)

Otherwise:
  Strong across most criteria,
  clear owner, evaluation method exists → DEPLOY
  Real value blocked by 1–2 specific,
  nameable gaps                        → GAP
  Interesting, but frequency, value,
  or reliability aren't there yet       → DEMO
```

## Why this matters

The cost of getting this wrong runs in both directions. Deploying a DEMO as if it's production-ready produces the failure mode everyone worries about with AI. Treating every workflow as a DEMO forever — endless pilots, no real adoption — is the quieter failure mode that wastes just as much effort and never delivers value.

Related: [AI Deployment Checklist](../governance/ai-deployment-checklist.md) for the specific pre-launch checks once a workflow is headed toward DEPLOY.
