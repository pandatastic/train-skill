# Roles, models and reasoning

Choose models available in the recipient's environment. This skill deliberately
sets no provider-specific model IDs, prices, speed settings or reasoning labels.

## Choose the smallest useful team

| Role | Responsibility | Selection guidance |
|---|---|---|
| Coordinator | Scope, dispatch, dependencies, candidate identity and gates | Strong planning and integration judgment; can also own strategy |
| Builder | Implement a settled design and repair confirmed defects | Efficient coding model for settled work; stronger reasoning when diagnosis or design remains open |
| Independent Closer | Review original requirements and prove acceptance | Capable reviewer with effort proportionate to permissions, migrations, concurrency and other material risks |
| Promoter, when needed | Deliver the accepted candidate to the authorized destination | Reuse an existing execution car unless a real ownership or separation boundary requires another |

A car is one user-visible Codex task. A subagent is a delegated worker inside a
task. Honor the user's requested structure; never substitute one for the other.
Create cars only after authorization to create them, and execute only after
authorization to start. If separate tasks are unavailable, report that limitation
before proceeding with a different structure. Do not present a self-review as
independent acceptance.

## Record and verify the configuration

The manifest records each task's exact model, supported reasoning effort,
environment, owner and expected result. Also record permitted alternatives,
escalation triggers and the overall effort boundary. Verify actual settings
at creation rather than assuming the requested configuration took effect.
Preserve active assignments unless a change is authorized.

Route by uncertainty and consequence, not code volume. A settled design states
the intended behavior, relevant implementation, consequential decisions, scope
and acceptance evidence. Important unresolved decisions can justify a stronger
model from the beginning; a cheaper model need not fail first.

Do not silently substitute an unavailable model or increase expenditure beyond
the agreed limits. Reasoning labels are not equivalent across models. Verify
current availability and pricing when they matter to a decision. A model change
does not expand scope or destination or reset accumulated effort and failures.

## Preserve independent acceptance

The Builder supplies the candidate identity, changes, checks, limitations and
risks. The independent Closer establishes PASS, VETO or BLOCKED against the
agreed criteria. Return confirmed defects to the Builder as one consolidated
repair handoff; recheck affected behavior after repair.

Handoffs include only the relevant requirements, exact candidate, changed files,
decisive evidence and unresolved issues. Follow
[coverage and recovery](coverage-and-recovery.md). Do not copy full transcripts
or repeat discovery without a concrete reason.

After two unsuccessful attempts at the same cause, reassess the diagnosis and
approach. Increasing reasoning effort alone is not a new strategy. Continue
justified repair within the agreed overall boundary; preserve explicit user
ceilings and uncertain external-operation state.

Assess routing from observed acceptance, defects, repair rounds and total
delivery time or attributable cost when available. Do not infer one task's cost
from account-wide usage while other work is running, or claim one model is more
efficient without comparable evidence.
