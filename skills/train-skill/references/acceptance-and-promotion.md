# Candidate validity and promotion

## Identify what was accepted

Each acceptance names the exact commit and clean/dirty working-tree state. Prefer a clean committed candidate for promotion; if reviewing uncommitted work, identify the patch/tree and do not describe its commit alone as the tested artifact. Record the environment profile (including database major version where applicable), verification generation, runtime role, helper revision and shared-method/overlay revisions. Use not-applicable for absent components, not an invented identity.

Evidence links, observation times and cursor accompany that identity. A cursor is a reading position, not an environment version. An advancing cursor or additional evidence does not invalidate prior checks. A method revision changed only for wording does not require runtime checks; a changed acceptance requirement does require its missing proof. Resolve mutable helper aliases to the installed revision used, without changing an active installation.

## Decide what must run again

Compare the accepted candidate and environment with the proposed result, including destination/base changes, configuration, fixtures, permissions, runtime and helper changes. In the existing checkpoint state what changed, what evidence remains valid and why, and which checks must run again.

Trace changed objects through relevant dependencies and interactions:

- Database: enumerate all changed objects, including triggers, helper functions, policies, grants, roles and migration ordering. Check callers, affected existing data, canonical readiness under the actual runtime role, and applicable replay/upgrade transitions. A table-only inventory is insufficient.
- Routes, UI and contracts: check changed inputs/outputs, consumers, authorization, persisted state and affected user flows. Include interactions introduced by other changes on the destination branch.
- Environment/helper inputs: recheck evidence whose execution or observations depended on those inputs. A new database generation needs relevant readiness/role proof; it need not invalidate independent pure-function tests.

Reuse deterministic results only when their full relevant inputs still match, retaining original provenance. Runtime/authentication/provider evidence must remain fresh enough for the claim. Uncertain impact requires broader relevant checks, never a default of no tests. Required CI/integration gates remain required. A documentation-only change with no behavioral or acceptance effect does not require a database rerun.

## Promote the accepted combination

Use the project's existing destination queue or ownership mechanism. Serialize only shared promotion/migration/deployment mutations into that destination; independent builds and reviews continue concurrently. Do not introduce a second lock or claim an informal note enforces exclusion.

Before promotion, refresh the destination and verify the exact intended head/base or integration candidate. Use the repository's merge queue or equivalent race-safe checks. If integration/base advances change the tested combination, assess impact and rerun affected checks before promotion; conflicts are implementation changes, not bookkeeping. If the destination cannot be held stable, recheck/requeue instead of treating stale approval as current. Record the actual resulting commit and confirm that accepted evidence applies to its tree and destination. Preserve required post-deployment checks and destination-specific authority.

### Claim the slot when ready

Use the destination's existing queue or ownership mechanism. Claim the release slot immediately before the next authorized shared mutation, once the exact candidate and required pre-mutation checks, approvals and operator access are ready. A provider-required queue or check that runs inside the shared operation follows its native rules. Drafts, isolated rehearsals, independent review, pending pre-mutation CI and human acceptance waits do not reserve the destination. Record a real dependency or collision when another release is blocked.

On acquiring the slot, refresh destination state and verify the exact candidate again. If drift or another prerequisite makes the mutation unready, return the slot and requeue after the gap is resolved. Once a shared mutation starts, retain ownership while its effects are uncertain or required reconciliation is in progress. Release the slot as soon as the shared operation and its required reconciliation finish. Use the existing checkpoint for ownership and release evidence.

Acceptance never authorizes a later destination.
