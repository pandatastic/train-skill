# One structured closure receipt

At each closeout (PASS, VETO or BLOCKED), the Coordinator assembles one compact receipt in the existing closure record, without a separate user request. Prefer existing helper receipts, task timestamps and consolidated defect entries. This is automatic Coordinator bookkeeping, not a claim that this skill installs logging hooks. Do not scan entire histories, build a telemetry service or delay delivery merely to fill missing fields.

Use the following shape, omitting irrelevant detail but retaining unknowns for unavailable measurements. Numeric zero requires observed coverage; missing events do not prove zero. Evidence references are private to the owning project. Never include credentials, raw private transcripts or operational data in a public/shared receipt.

```json
{
  "schema": "train-closure/1",
  "method_revision": "2026-11-25a",
  "train": "owning-project train identifier",
  "as_of": "actual UTC closeout timestamp",
  "outcome": "PASS | VETO | BLOCKED",
  "candidate_and_configuration": "existing checkpoint reference",
  "handoffs": [
    {"step": "named upstream result → next step", "result_ready_at": "unknown", "next_step_dispatched_at": "unknown"}
  ],
  "destination_live_at": "unknown",
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

## Three timestamps for delivery and handoffs

Record timestamps in UTC from existing task, dispatch or deployment evidence when the event occurs. Keep the current handoff in the checkpoint and preserve prior handoffs in linked history. Include these fields in the existing closure receipt, with candidate/run identity and evidence links as needed.

- `result_ready_at` is when the upstream result or verdict became available for the named handoff. Use the completion or artifact timestamp when available.
- `next_step_dispatched_at` is when the Coordinator actually dispatched or started that named next step. Pair it with the same handoff, even when that step is a repair.
- `destination_live_at` is the first verified serving time for the exact release at the authorized destination. A merge, queued deployment or green source check alone does not establish serving. Use `not_applicable` for work with no serving destination.

Use `unknown` when an applicable time cannot be established. Record pending steps as pending in current state and use `unknown` at closeout if they did not occur or their time is unavailable. Use `not_applicable` for a handoff with no next step. Derive handoff latency only from paired timestamps. Use the final accepted candidate's readiness timestamp to compare with serving time, and use dispatch-to-serving only for the matching promotion step. Keep the existing execution-to-result and execution-to-acceptance measurements. The fields are observational and never block delivery.

Measure both durations in `timing_seconds` from authorized execution start; define usable result against the agreed outcome, not the first passing command. Independent acceptance time stays unknown if never achieved. Distinguish elapsed wall time from effort and overlapping car time. For cost, retain currency, attribution method and source; token counts alone are not dollar savings. Never derive car consumption from concurrent account-wide usage.

A repair round is a consolidated defect handoff and its verification, not each edit or command. Group repairs by supported root cause, including defects introduced during repairs. Classify repeated checks as required, avoidable, or unknown based on changed inputs, independent review and mandatory gates. Do not count justified independent verification as waste. Record late prerequisites discovered after implementation began, with affected scope. Distinguish necessary consent from product decisions and avoidable message relay.

Escaped defects are defects discovered after an acceptance claim, known as of the receipt timestamp. Future discoveries append a linked dated follow-up; preserve the original receipt rather than rewriting history. An incorrectly claimed acceptance can be identified before delivery and is tracked separately. No known defects is not proof of no defects.

Use these receipts to identify demonstrated waste and compare similar work across cars, including implementation, coordination, review, repair and user intervention. A single train is a baseline, not a model ranking. Keep model routing stable in this revision; propose later changes only from comparable evidence. Do not edit skills or memories automatically at closure.
