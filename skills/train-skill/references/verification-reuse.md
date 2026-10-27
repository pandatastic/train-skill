# Verification helpers and reusable environments

Use this reference when delivery needs a database or repeated verification.
The daily loop is short: inspect status, acquire or resume, run a named check,
read failure evidence, complete independent review, then release or retain.
Helpers supply scoped evidence; the independent Closer owns acceptance.

## Discover once, reuse across handoffs

Inspect the project's existing helpers, canonical migration path, supported
runtime, role/fixture recipes and available browser/provider capabilities before
writing another bootstrap. Prefer a maintained project entrypoint with compact
results and private logs. Record its actual commands in project instructions;
do not assume that installing this skill installs a verification toolkit.

When a missing helper is necessary and within the agreed implementation scope,
build the smallest reusable helper and validate its relevant behavior in the
existing review loop. Do not make it a separate train or general infrastructure
framework. Keep source versioned in the owning project and reusable state outside
disposable worktrees where appropriate. Reference an installed revision only
after verifying it exists and supports the required commands.

Use the existing task/environment identity across turns, repairs and sequential
Builder/Closer review when the state remains suitable. Concurrent mutations need
separate environments. A new turn or reviewer does not justify a fresh database.
Preserve healthy environments when adopting helpers at a safe handoff.

## Choose the required fidelity

- Pure calculations, validation and rendering: existing runners, without a
  database unless the behavior actually depends on one.
- Ordinary persistence/API work: a reusable local database service, validated
  synthetic baseline and separate task database with a restricted runtime role.
- Cluster-wide role, membership or server changes: a dedicated server/cluster.
  In PostgreSQL, separate databases do not isolate roles.
- Hosted transport, pooling, managed permissions or deployed connectivity:
  an explicitly selected environment in the owning project's provider account.
  Local evidence cannot prove a hosted claim.

Choose the project's supported runtime/version and canonical migration verifier.
Keep organization/project resources separate: credentials, data, state roots,
roles, cloud branches and browser profiles are not reusable across unrelated
projects merely because the helper convention matches.

## Keep database reuse honest

Baseline compatibility follows database inputs: ordered migrations and journal
rules, bootstrap roles, extensions/configuration, synthetic fixture and clock
recipes, and relevant helper/dependency versions. Record the application
candidate separately; an unrelated UI change should not force reconstruction.
Cache only complete, validated baselines. Preserve active generations when
inputs diverge; do not rewrite their history or silently reset a retained demo.

Apply a missing migration tail in place only when compatibility and ownership
are established. Otherwise preserve the old environment and create a compatible
generation. A cached latest schema does not prove clean replay or an upgrade
transition. Migration work retains applicable replay and upgrade checks.

Verify real restricted-role behavior, including the relevant positive and
negative permission boundary. Owner credentials do not prove application
permissions. With PostgreSQL template cloning, reapply database connection
permissions and settings explicitly; they are not inherited from the template.

For disposable hosted branches, select an authorized project/parent explicitly,
set and read back expiration, retain ownership and resource limits, and reconcile
uncertain creation before retrying. Copying live data requires the appropriate
data authority and outbound controls before starting workers. Preserve actual
provider approval requirements for destructive operations. Do not allocate paid
resources merely because a local check is inconvenient.

## Small evidence, precise validity

Prefer named checks returning status, candidate, environment identity, timings,
reuse decisions and evidence paths. Keep full logs private on disk; expose bounded
failure excerpts and cursor-based summaries. Never include credential values in
handoffs. Saved status is a recorded observation, not a fresh runtime verdict.

Reuse successful deterministic evidence only when its complete inputs still
match, including files read indirectly, command/runtime and helper revision.
Retain the original candidate/time provenance. Runtime, role, authentication and
deployed-state checks need evidence fresh enough for their claim. Unknown impact
requires the relevant broader check; mandatory repository CI remains mandatory.

Preparing a persona does not prove normal sign-in. Use the application's actual
authentication boundary for acceptance. Preserve temporary access through the
last required review, then revoke it without deleting audit-linked users. Retained
human demos need an owner and a clear access lifetime; disclose absent automatic
expiry rather than assuming one exists.

Keep environment owner/identity, evidence cursor and missing proof in the existing
checkpoint. Do not add a parallel report system or reload successful logs on every
turn. Measure setup/reuse duration and output volume when observable; do not invent
token savings or attribute aggregate account usage to one task.

## Recover and clean up owned resources

Before mutation or reuse, verify actual server/database identity, task ownership
and compatibility. Use proportionate locks and durable intent where interrupted
setup could otherwise create duplicates. A timeout or incomplete receipt calls
for reconciliation, not a new task ID that hides the failure.

Cleanup is scoped to exact owned resources. Preserve active connections, retained
demos and other tasks. A generic cache/disk cleanup must not infer that databases
are disposable. Keep working environments and valid evidence through review;
release unrelated shared deployment reservations during a final human wait.

Missing browser/provider capability stays explicit and blocks only the dependent
claim. Do not repeat identical environment setup attempts or convert unavailable
proof into PASS. Adoption of this guidance does not expand execution authority,
require a pilot, restart active work or authorize new cars or automations.
