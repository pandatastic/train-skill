# One structured closure receipt

At each closeout (PASS, VETO or BLOCKED), the Coordinator assembles one compact receipt in the existing closure record, without a separate user request. Prefer existing helper receipts, task timestamps and consolidated defect entries. This is automatic Coordinator bookkeeping, not a claim that this skill installs logging hooks. Do not scan entire histories, build a telemetry service or delay delivery merely to fill missing fields.

Use the following shape, omitting irrelevant detail but retaining unknowns for unavailable measurements. Numeric zero requires observed coverage; missing events do not prove zero. Evidence references are private to the owning project. Never include credentials, raw private transcripts or operational data in a public/shared receipt.

```json
{
  "schema": "train-closure/1",
  "method_revision": "2026-10-28a",
  "train": "owning-project train identifier",
  "as_of": "actual UTC closeout timestamp",
  "outcome": "PASS | VETO | BLOCKED",
  "candidate_and_configuration": "existing checkpoint reference",
  "timing_seconds": {
    "execution_to_usable_result": "unknown",
    "execution_to_independent_acceptance": "unknown"
  },
  "human_interventions": {
    "necessary_consent": "unknown",
    "avoidable_relay": "unknown",
    "other_decisions": "unknown"
  },
  "repairs": {"rounds": "unknown", "by_root_cause": "unknown", "introduced_defects": "unknown"},
  "late_acceptance_prerequisites": "unknown",
  "coordination": {"dispatches": "unknown", "status_reads": "unknown", "repeated_context_loads": "unknown"},
  "checks": {"required_repeats": "unknown", "avoidable_duplicates": "unknown", "unclassified_repeats": "unknown"},
  "known_escaped_defects": "unknown",
  "incorrect_acceptance_claims": "unknown",
  "tooling_effort_seconds": "unknown",
  "attributable_usage_and_cost": "unknown",
  "measurement_sources_and_limits": [],
  "follow_up_receipts": []
}
```

Measure both times from authorized execution start; define usable result against the agreed outcome, not the first passing command. Independent acceptance time stays unknown if never achieved. Distinguish elapsed wall time from effort and overlapping car time. For cost, retain currency, attribution method and source; token counts alone are not dollar savings. Never derive car consumption from concurrent account-wide usage.

A repair round is a consolidated defect handoff and its verification, not each edit or command. Group repairs by supported root cause, including defects introduced during repairs. Classify repeated checks as required, avoidable, or unknown based on changed inputs, independent review and mandatory gates. Do not count justified independent verification as waste. Record late prerequisites discovered after implementation began, with affected scope. Distinguish necessary consent from product decisions and avoidable message relay.

Escaped defects are defects discovered after an acceptance claim, known as of the receipt timestamp. Future discoveries append a linked dated follow-up; preserve the original receipt rather than rewriting history. An incorrectly claimed acceptance can be identified before delivery and is tracked separately. No known defects is not proof of no defects.

Use these receipts to identify demonstrated waste and compare similar work across cars, including implementation, coordination, review, repair and user intervention. A single train is a baseline, not a model ranking. Keep model routing stable in this revision; propose later changes only from comparable evidence. Do not edit skills or memories automatically at closure.
