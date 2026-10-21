# Step 7 — BRD

**Agent:** BRD Builder

## Your role in this step
Decide whether the business baseline is defensible.

## Do
Confirm [DT→BRD handoff](DT-TO-BRD-HANDOFF.md). Select BRD Builder and ask it to create the BRD from completed DT evidence, preserve confidence, avoid restarting discovery, and keep unresolved dependencies as gates. Use the [Step 7 Review Card](STEP-07-REVIEW-CARD.md). Explicitly approve only as the workshop BRD planning baseline.

## What good looks like
Requirements are traceable/decision-backed, reviewable and honest about gates.

## Approval blocker vs open governed dependency
An **approval blocker** means the baseline is not defensible enough to approve, for example a material requirement has no evidence/decision basis or no reviewable acceptance boundary. Stop and repair it before approval.

An **open governed dependency** can remain unresolved when it is explicitly recorded as a gate with ownership, affected requirements, exit evidence and a next decision trigger. For example, the final FX-rate provider may still be unresolved; if that dependency is recorded as a gate rather than assumed away, the BRD can still be approved as a planning baseline with the gate open.

## Stop
BRD and BRD→PRD handoff have no approval blockers. Open governed dependencies may remain as explicit gates.

## Recover if needed
If evidence is unavailable, identify it rather than reconstructing it. Repair only missing governance/traceability.

## Next
[Proceed to Step 8 →](STEP-08-PRD.md)
