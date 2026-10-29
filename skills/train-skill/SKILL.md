---
name: train-skill
description: Plan and execute substantial project delivery, build trains, staged releases, and evidence-based acceptance within an explicit scope and destination. Not for trivial edits or simple questions.
metadata:
  short-description: Autonomous delivery within a compact agreed scope
---

# Train Skill

Shared method revision: 2026-10-28a (package 1.2.0). The operating loop is **build -> independent review -> repair confirmed defects -> verify affected checks -> deliver**. The Coordinator runs the loop; the user does not operate the train.

## Agree once

Identify the active project, applicable instructions, starting candidate, intended outcome, destination, permitted systems/actions, exclusions, acceptance checks, and recovery boundary. Preserve explicit requirements and their user source; resolve consequential ambiguity, not routine technical details. Keep one compact contract using only useful fields from [the template](references/contract-template.md).

Distinguish QUESTION/PROPOSAL/MANIFEST from EXECUTE. A question or proposed train creates nothing. “Build a train” is manifest-only until the user authorizes starting it. Requested sessions/tasks/threads are separate user-visible tasks, never substitute subagents. Delegation requires explicit authorization.

Execution authority covers the necessary implementation, setup, integration, migrations, delivery tooling, ordinary repairs, and stage transitions within the agreed actions and destination. A LOCAL destination stays local; DEVELOPMENT does not authorize PRODUCTION. Existing exclusions and explicit approval conditions remain binding. Readiness alone never expands authority. Do not import another organization's facts, accounts, data or artifacts without explicit authorization.

## Establish acceptance feasibility first

Before substantial implementation, establish how each critical outcome will be demonstrated at the authorized destination. Where applicable and authorized, prove one representative browser/authentication/data path early; identify the destination database major version and canonical readiness checker; confirm required media, data and personas exist. Record proof or the precise prerequisite gap in the existing contract. A local rehearsal does not prove destination readiness. Surface blockers promptly and continue independent work; block only dependent work. Do not create resources or cross authority boundaries merely to complete kickoff.

At kickoff record the installed shared-method revision, applicable private overlay revision, and actual task model/effort against the approved defaults. Flag drift or unavailable readback in the checkpoint; never claim requested settings were verified. Resolve consequential drift before dependent work, without silently reconfiguring active tasks. Keep organization-specific routing, reporting, permissions, release rules and helper paths in recipient-owned overlays/project instructions. This revision does not change model routing; comparable closure evidence is required before proposing routing changes.

## Deliver autonomously

Once execution is authorized, select routine technical methods, use authorized access, dispatch existing cars, run required checks, fix in-scope defects, and advance when gates pass. Do not ask for repeat GO or permission for ordinary implementation choices. Coordinate dependencies directly rather than using the user as a relay.

Automation is part of acceptance: routine approved delivery must not depend on the user typing commands, moving credentials between tools, coordinating cars, or repeatedly confirming runs. Prefer existing native authentication, supported secure credential storage and established release tooling. Before a human handoff, verify the actual access/consent barrier and complete feasible preparation. Never assume provider policy requires manual action without evidence. Never expose secrets or bypass an actual security/approval control. New account permissions or other genuinely new authority still require authorization.

Small scripts, fixtures and integration helpers belong to implementation and receive proportionate review; do not turn each into a separate train, approval stage, or repair budget. A substantial new credential service, receipt framework, infrastructure subsystem or security model is a design expansion, not an automatic release prerequisite.

Ask the user only for an essential business/product decision, genuinely new scope/authority/expenditure, a verified personal authentication/consent action, or a consequential unresolved risk or exhausted agreed effort boundary. Present the concrete decision and smallest practical alternative. Continue independent ready work while the affected step waits.

## Use the fewest cars

Normally use a Coordinator, Builder and independent Closer. Strategy can stay with the Coordinator. The Builder owns implementation plus necessary authorized setup and delivery tooling. The Closer owns independent acceptance. Add a Promoter only for a real deployment ownership/separation need; otherwise assign promotion to an existing execution car while retaining independent acceptance.

Per project, designate one execution Coordinator for routine dispatch and repairs. The Closer owns acceptance; a separate Strategist owns unresolved design/scope decisions. External supervisors receive decisions and exceptions, plus explicitly authorized deployment/completion reports, without parallel coordination or duplicate reviews.

Follow [model routing](references/car-model-routing.md). Record and verify exact task IDs, model/effort, environment and ownership at creation; preserve active configurations unless authorized to change them. Reuse suitable existing cars and worktrees. A model escalation does not imply another car.

## Review what matters

Resolve the verification route before implementation depends on it: candidate, environment/profile, restricted role, required personas and browser/provider capability. For database-backed work or repeated checks, use the project's existing persistent helpers; read [verification reuse](references/verification-reuse.md). Reuse compatible task resources through repairs and sequential review. Pure unit or rendering work does not require a database by default.

For applicable new trains, default to the maintained owning-project helper and record its entrypoint/profile/owner. Active trains retain their tools, resources, access and valid evidence; adopt only at compatible safe handoffs, without restart, reset or redispatch.

Every acceptance handoff records exact commit and working-tree state, environment profile/database version, environment generation, runtime role, helper revision and skill revision, alongside evidence links/cursor. Use [candidate validity and promotion](references/acceptance-and-promotion.md) to decide affected checks when these change. An advancing evidence cursor alone does not invalidate checks. Serialize promotion into the same destination, not independent builds and reviews; release shared deployment/migration ownership after mutations are reconciled, independently of feature/human acceptance.

For every material repair the Builder covers the failing case, relevant existing-state cases and affected lifecycle transitions before handoff. The Closer independently verifies the result and does not co-author the repair. See the [worked handoffs](references/checkpoint-examples.md).

Review approved behavior, affected dependencies and material risks. Complete feasible review and return one consolidated defect list; do not drip-feed independent repair requests. If a blocker prevents review, fix it within authority and finish the remaining review. Reuse evidence still applicable to the candidate; rerun affected checks and mandatory integration/CI gates. Do not repeatedly audit a working baseline without a changed dependency or observed failure.

Evidence must match the claim: tests for deterministic behavior; actual database/runtime-role evidence for migrations, data and permissions; authenticated browser/API evidence for relevant behavior; exact deployed candidate for release; observed provider boundary for end-to-end claims. Mocks, source inspection and admin previews do not prove live persona/provider behavior. Keep unavailable proof explicit; never fabricate PASS or manufacture unauthorized shared records to obtain it.

Do not add unrelated cleanup, speculative hardening or open-ended adversarial research to an ordinary delivery. Preserve serious findings and block affected stages where justified. A local observation failure or unavailable inspection method is not proof that the remote service is broken. Optional improvements stay outside the train; required functionality is not silently dropped.

## Bound diagnosis, not every repair

After two unsuccessful attempts at the same root cause, reassess cause and approach internally. This is not an automatic approval request. Continue a materially justified in-scope approach; do not reset history by renaming a blocker, changing candidates, or replacing a car. Use a finite overall effort/recovery boundary proportionate to the task; retain an agreed time/cost limit, or state a bounded diagnostic limit at kickoff without inventing monetary approval. Do not create a fresh budget for each helper or demand repeated “one more repair” approvals.

Do not blindly retry an uncertain external write or migration. Reconcile actual state first. Before recovery/restore actions, verify exact targets, side-effecting defaults and isolation controls; rehearsal labels do not guarantee isolation. Preserve user-defined ceilings and explicit stop conditions on active trains unless the user changes them. Set repair limits for the actual task rather than imposing a universal round count.

## Keep records and supervision small

Follow [coverage and recovery](references/coverage-and-recovery.md): one current checkpoint, existing evidence links, concise handoffs, and active progress supervision. Send the full contract once; send subsequent deltas to tasks that retain it. Fresh/recovered tasks receive the compact checkpoint and access to the contract. No new report, approval round, amendment, seal, or checklist per dispatch; the single closure receipt below is the only added closeout record. Preserve exact candidate identity and use hashes/seals only where they serve a concrete integrity need or existing requirement.

At review handoff preserve the environment identity, evidence cursor and persona lifetime. Revoke temporary access after its last required review. If only human acceptance remains, retain the owned demo as needed and release unrelated shared deployment reservations so a passive wait does not block other authorized work.

Close at the authorized destination with outcome, exact artifact, decisive checks, actual mutations, remaining limitations and owned-resource cleanup. PASS means agreed acceptance proven; VETO means a reviewed criterion failed; BLOCKED means safe in-scope progress needs an external change or user decision. Do not continue into optional work after completion.

## Adopt and stabilize

New trains use this revision. Active trains retain their recorded method and configuration; a shared file update is not a retroactive requirement. For an authorized active-train update, apply at the next compatible safe handoff and record the revision change. Preserve completed work, valid evidence, original requirements, destination, real safeguards and current ownership. Retire redundant agent-created ceremony; identify the shortest remaining delivery path. Do not restart, re-audit everything, erase failures, override direct user ceilings, interrupt healthy operations, or create new gates to adopt this skill.

Freeze the method for one complete delivery unless the user requests a change or a concrete safety-critical defect requires correction. At every closeout, the Coordinator automatically assembles one compact [structured receipt](references/closure-telemetry.md) from available evidence in the existing closure record. Missing measurements are explicitly unknown; do not require retrospective log reconstruction or invent measurements. Skill instructions do not install automatic instrumentation. Do not pause a whole train or add an approval gate for telemetry. Propose later changes only from demonstrated problems; do not automatically edit skills or memories.
