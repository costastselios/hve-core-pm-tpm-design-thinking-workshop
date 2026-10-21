# Step 7 — BRD

**Agent:** BRD Builder

## Your role in this step
Decide whether the business baseline is defensible.

## Do
Confirm [DT→BRD handoff](DT-TO-BRD-HANDOFF.md). Select BRD Builder and ask it to create the BRD from completed DT evidence, preserve confidence, avoid restarting discovery, and keep unresolved dependencies as gates. Use the [Step 7 Review Card](STEP-07-REVIEW-CARD.md). Explicitly approve only as the workshop BRD planning baseline. Then create the BRD→PRD handoff using the [handoff skeleton](BRD-TO-PRD-HANDOFF-SKELETON.md), and save the BRD and the handoff as files.

## What good looks like
Requirements are traceable/decision-backed, reviewable and honest about gates.

## Approval blocker vs open governed dependency
An **approval blocker** means the baseline is not defensible enough to approve, for example a material requirement has no evidence/decision basis or no reviewable acceptance boundary. Stop and repair it before approval.

An **open governed dependency** can remain unresolved when it is recorded as a gate with every [Gate Record](../../docs/GATE-RECORD.md) field completed. For example, the FX provider and coverage decision may still be unresolved. If that dependency is recorded as a gate rather than assumed away, the BRD can still be approved as a planning baseline with the gate open. The [worked example](../../docs/WORKED-EXAMPLES.md#compact-traceability-example) shows a completed gate record.

## Stop
The BRD is explicitly approved as the planning baseline. The BRD and BRD→PRD handoff are saved as files and have no approval blockers. Open governed dependencies may remain as explicit gates.

## Recover if needed
If evidence is unavailable, identify it rather than reconstructing it. Repair only missing governance/traceability.

## Next
[Proceed to Step 8 →](STEP-08-PRD.md)
