# Worked Examples
**Weak BR:** “Support users well.”

**Stronger BR:** “BR-001: Preserve source context for each recorded holding. Acceptance: every holding has attributable source context or an explicit unsupported state.”

**Feature:** Inspectable holding provenance.

**Task:** Build provenance API endpoint. Tasks are outside this workshop.

## Compact traceability example

IDs below are illustrative. Use the numbering from your own BRD and PRD.

**Evidence:** Participant 01 (low confidence, single participant) reported that manually maintained FX reduces trust. Participant 02 wants automatic FX. These are supplied case-study signals, not prevalence claims.

**Open decision (canonical concept):** FX provider coverage and licensing.

**BR-002:** Portfolio valuations must retain attributable FX context rather than presenting converted values without provenance.

**FR-004** (traces to BR-002): For a converted holding valuation, expose the reporting currency and recorded FX provenance/status used for that valuation.

**Epic:** Trustworthy portfolio valuation.

**Feature:** Inspectable FX provenance (traces to FR-004 → BR-002; conditional on GATE-001).

**Inherited gate record:**

- **Gate ID:** GATE-001
- **Title:** FX provider and coverage
- **Owner:** Product Owner (name the accountable person in your artifact)
- **Status:** Open
- **Affected requirements/features:** BR-002, FR-004, Inspectable FX provenance
- **Exit evidence:** Provider coverage and licensing decision for the supported currencies
- **Next decision trigger:** Before Feature commitment for engineering planning
- **Remaining uncertainty:** Whether all supported currencies can be valued with attributable FX at the required frequency

The gate is carried forward. Backlog decomposition doesn't close it by assumption.
