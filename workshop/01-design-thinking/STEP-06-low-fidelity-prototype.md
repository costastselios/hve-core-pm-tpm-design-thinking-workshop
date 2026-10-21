# Step 6 — Low-Fidelity Prototype

**Agent:** DT Coach

## Your role in this step
**Your job:** behave like the product owner/researcher reviewing a low-fidelity workflow. Exercise the workflows, capture what you observe, compare those observations with the supplied participant evidence, and decide what the evidence means.

**HVE's job:** help structure the Method 6 learning and preserve the distinction between evidence, interpretation, assumption, and redesign hypothesis.

**Do not worry about:** production-quality visual design, implementation architecture, or proving that the solution is validated.

## Do

### 1. Prepare the test
1. [Open the detailed test script](../04-prototype/test-script.md).
2. [Open the self-test note template](../../workshop-output/prototype-self-test.md).
3. Open `../04-prototype/iteration-01/index.html` **in a web browser**.

> **Opening a prototype:** in VS Code, right-click `index.html` → **Reveal in Finder/Explorer** → double-click the file. A local HTML preview is also fine. If the page fails on first load, refresh once.

### 2. Exercise Iteration 1 end to end
Do not jump directly to recovery. The earlier workflows provide the context needed for the recovery failure to be meaningful.

Complete:
- statement-based portfolio establishment;
- portfolio orientation/history;
- holding inspection;
- valuation/FX provenance;
- manual transaction entry;
- reviewed activity import;
- duplicate/uncertain import review;
- mismatch discovery;
- recovery.

Keep notes as you go.

### 3. Capture the failure before reading the answer
At the recovery screen, pause **before selecting a correction**.

Write down what you think each option means:
- **Update holding**
- **Fix history**

Then choose one and inspect the outcome.

Ask yourself:

> **Can I explain what changed, what did not change, and what is still uncertain?**

Do not move forward until you have recorded your own interpretation.

### 4. Compare against supplied participant evidence
Only now [open the supplied Iteration 1 test evidence](../04-prototype/iteration-01/test-results.md).

Give DT Coach the decisive supplied finding:

```text
The participant could complete the recovery flow mechanically but could not explain whether the action changed today's holding, historical activity, or both.
Treat this as a concept-comprehension failure, not simply a wording or visual-design defect.
Preserve the distinction between the supplied participant evidence and my own self-test observations.
```

### 5. Exercise Iteration 2
Open `../04-prototype/iteration-02/index.html` in a browser.

Do not inspect only one branch. Complete both:

**Known cause**
- I know the missing activity
- review consequence preview
- confirm

**Unknown cause**
- I only know today's correct holding
- review consequence preview
- confirm

For each branch explain:
- what changes;
- what does not change;
- what remains uncertain.

Then [read the Iteration 2 recovery model](../04-prototype/iteration-02/recovery-model.md).

### 6. State the validation boundary
Iteration 2 is **a redesign hypothesis**. The supplied evidence does not show that representative users have retested and validated it.

Tell DT Coach:

```text
Iteration 2 is an evidence-informed redesign hypothesis, not a validated solution.
Capture what changed in the concept, the evidence that motivated the change, and the representative-user validation that still remains open.
```

### 7. Prepare the next-agent handoff
Once Method 6 is complete, [open the DT → BRD handoff](../05-common/DT-TO-BRD-HANDOFF.md).

Make sure the handoff preserves:
- Method 1–5 evidence and confidence;
- Iteration 1 supplied test evidence;
- your self-test as separate workshop observation;
- the conceptual failure;
- Iteration 2 redesign hypothesis;
- the outstanding representative-user validation gap.

## What good looks like
You can articulate the workflow, the concrete Iteration 1 comprehension failure, how Iteration 2 changes the mental model, and why the redesign remains unvalidated.

The prototype feels coherent enough that the recovery confusion cannot simply be dismissed as “the screens were too incomplete to understand.”

## Stop
Stop Design Thinking when:
- Iteration 1 has been exercised end to end;
- your own observations are recorded separately from supplied participant evidence;
- the conceptual recovery failure is explicit;
- both Iteration 2 recovery branches have been exercised;
- the redesign hypothesis and validation gap are explicit;
- the DT → BRD handoff is ready.

**HVE Design Thinking Methods 7–9 remain outside this workshop.**

## Recover if needed
If a prototype does not open or controls do not respond:
1. Confirm you opened `index.html` in a browser rather than viewing source text.
2. Refresh once.
3. Restart from the prototype's **Restart** control.
4. If the issue persists, record a **tooling failure** in your self-test notes and do not claim that you exercised the affected workflow.

If DT Coach tries to treat your self-test as user research, paste:

```text
Keep my workshop self-test observations separate from the supplied participant-test evidence.
My interaction with the prototype is not representative-user research.
```

## Next
[Proceed to Step 7 — BRD →](../05-common/STEP-07-BRD.md)
