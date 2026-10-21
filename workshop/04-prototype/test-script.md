# Low-Fidelity Prototype Test Script

## Purpose
This exercise demonstrates **workflow fidelity**, not visual polish. Iteration 1 should be believable enough to expose a conceptual problem in the recovery experience. Iteration 2 redesigns that problem.

Your own walkthrough is a **self-test**, not representative-user research. Keep your observations separate from the supplied participant-test evidence.

## Before you start
Open `iteration-01/index.html` in a browser. Use the prototype itself; statement/activity-file selection is simulated inside the HTML.

Record notes in `workshop-output/prototype-self-test.md` using four categories:
- observation;
- your interpretation;
- supplied participant evidence;
- open question.

---

# Iteration 1 — Task A: Establish and orient

### A1. Establish the portfolio
1. Start from the empty/setup state.
2. Choose **Use workshop statement**.
3. Inspect the detected holdings and source context.
4. Establish the portfolio.

Observe:
- Is import-first setup understandable?
- Is it clear that holdings retain source/broker context?
- Can you see that manual entry remains a fallback rather than the primary path?

### A2. Orient to the portfolio
1. Review the consolidated portfolio screen.
2. Explain, in your own words, what the history panel is communicating.
3. Identify the source broker and asset type for each holding.
4. Notice the valuation and FX/trust indicators.

Observe:
- Can you understand that the view spans multiple source platforms?
- Is historical direction visible without implying forecasting?
- Is valuation detail progressively available instead of overwhelming the overview?

### A3. Inspect provenance
1. Open **Global Equity ETF**.
2. Inspect the holding overview and recent activity.
3. Choose **View provenance**.
4. Explain where the displayed valuation/FX context comes from.

Observe:
- Does provenance increase trust?
- Is the distinction between source broker, price evidence, FX evidence, and reporting currency understandable?

---

# Iteration 1 — Task B: Maintain and recover

### B1. Add activity manually
1. From Global Equity ETF choose **Add transaction**.
2. Review the transaction fields: activity, date, units, price, currency, fee.
3. Choose **Review transaction**, then **Save transaction**.

Observe:
- Does the transaction model make sense after the investing primer?
- Is review-before-save clear?

### B2. Import activity
1. Return to the portfolio and choose **Import activity**.
2. Use the simulated workshop activity file.
3. Review all three staged cases:
   - ready activity;
   - possible duplicate;
   - activity needing attention.
4. Make a duplicate decision.
5. Apply the reviewed activity.
6. Follow **Go to holding**.

Observe:
- Is it obvious that imported activity is staged before commitment?
- Can you distinguish ready, duplicate, and uncertain records?

### B3. Resolve the mismatch
1. Open **Resolve mismatch**.
2. Read the broker evidence and recorded portfolio state.
3. **Before clicking**, explain what you expect **Update holding** and **Fix history** to do.
4. Choose one option.
5. Read the result.

Critical question:

> Can you explain whether today's holding, historical activity, or both changed — and what remains uncertain?

If you cannot, that is the intended Iteration 1 learning signal.

---

# Compare with supplied participant evidence

Now read `iteration-01/test-results.md`.

Do not rewrite your own self-test as participant evidence. Compare your observations with the supplied finding that recovery could be completed mechanically without understanding its consequence.

---

# Iteration 2 — Test the redesign

Open `iteration-02/index.html` in a browser.

### C1. Understand the conflict
1. Read **New evidence says**.
2. Read **Your portfolio currently says**.
3. Explain why the system flagged the conflict.
4. Distinguish **current impact** from **historical impact**.

### C2. Test the known-cause path
1. Choose **I know the missing activity**.
2. Read the consequence preview.
3. Before confirming, identify:
   - what will change;
   - what will not change;
   - what will remain uncertain.
4. Confirm.

### C3. Test the unknown-cause path
1. Choose **Try other branch**.
2. Choose **I only know today's correct holding**.
3. Read the consequence preview.
4. Again identify what changes, does not change, and remains uncertain.
5. Confirm.

## Final comparison
Answer these questions in your self-test notes:

1. What exactly failed in Iteration 1?
2. What mental model does Iteration 2 introduce?
3. Why is Iteration 2 more trustworthy even though it may leave uncertainty unresolved?
4. What still requires representative-user validation?

The intended learning loop is:

> **prototype → evidence → conceptual failure → redesign hypothesis**
