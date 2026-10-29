# Compact checkpoints and incremental handoffs

These examples use fictional identifiers and relative evidence paths. Real records use complete commit IDs. Keep scope/authority in one contract and chronology in history; do not copy them on every repair.

## Current checkpoint example

```yaml
scope: export filtering; contract: contract.md
candidate:
  commit: 1111111111111111111111111111111111111111
  tree: clean
  profile: local-synthetic-pg17
  database_major: 17
  generation: task-export/g2
  runtime_role: restricted-app
  helper_revision: helper-r4
  method_revision: 2026-10-28a
  overlay_revision: project-r2
owners: {execution: coordinator-task, repair: builder-task, acceptance: closer-task}
configuration: {actual_model_effort: "recorded in contract.md", drift: none}
proof: {early_sign_in: evidence/auth.json, readiness: evidence/db.json}
evidence: {cursor: 42, links: [evidence/review.json]}
access: valid through Closer review; owner builder-task
unresolved: [D2 stale saved filter after reload]
next: Builder repairs D2 and verifies existing-state/reload cases
```

If readiness or authentication is blocked, replace its proof link with the actual gap and dependent criterion. Do not mark the whole train blocked when unrelated implementation can proceed. Keep effort totals and uncertain writes in current state when they affect the next action.

## Repair delta to an informed Builder

> Repair D2 from evidence/review.json against commit 1111111111111111111111111111111111111111. You own the filter repair. Preserve task-export/g2 and reviewer access. Cover the failing stale saved filter, valid existing filters, missing saved state, and reload after success/failure. Return the new exact commit, changed-object/dependency impact, decisive evidence and unresolved gaps. Existing contract and destination remain in force.

The Builder chooses and implements the fix. The Closer may explain the failed criterion and reproduction but does not co-author the solution. On return, the Coordinator sends the Closer the changed candidate, D2 evidence and affected checks; independent acceptance remains the Closer's decision.

## Fresh or recovered task

Supply this current checkpoint and the contract location, plus only sources required for the next action. Verify actual candidate/environment state before acting. Do not send an unexplained delta to a task that never received the agreement, and do not reload the entire chronology to recover current ownership.
