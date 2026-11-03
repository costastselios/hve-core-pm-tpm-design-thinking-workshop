# Step 9 — Backlog

**Agent:** PRD Builder (new chat)

## Your role in this step
Judge outcome/capability boundaries and gate status.

## Do
Before leaving the Step 8 chat, confirm the **approved PRD planning baseline** is saved as a file. Then start a **new PRD Builder chat** and attach that file using your VS Code Copilot file-context mechanism. Make sure the attached baseline includes its inherited exclusions and open gates. Don't rely on the Step 8 chat context.

Ask for a planning-only Epic/Feature proposal from that baseline: Epics/Features only, PRD traceability back to the approved baseline, deferred scope excluded, gated capabilities kept conditional, and no Stories/Tasks/architecture/estimates/RPI/code. Tell it not to edit the approved PRD and not to hand off to a tracker or Functional Planner. Review [worked examples](../../docs/WORKED-EXAMPLES.md).

## What good looks like
Epics are outcomes; Features capabilities; gates visible.

## Stop
Complete Epic/Feature proposal.

## Recover if needed
If the agent decomposes too deeply, stop and roll back Story/Task-level items. If it starts a new PRD, revises the approved one, or offers a tracker or Functional Planner handoff, decline and restate that this step only proposes Epics/Features from the approved baseline.

## Next
[Proceed to Step 10 →](STEP-10-REVIEW.md)
