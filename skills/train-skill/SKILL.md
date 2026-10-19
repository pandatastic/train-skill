---
name: train-skill
description: Plan and execute substantial project delivery, build trains, staged releases, and evidence-based acceptance within an explicit scope and destination. Not for trivial edits or simple questions.
metadata:
  short-description: Autonomous delivery within a compact agreed scope
---

# Train Skill

The operating loop is **build -> independent review -> repair confirmed defects -> verify affected checks -> deliver**. The Coordinator runs the loop; the user does not operate the train.

## Agree once

Identify the active project, applicable instructions, starting candidate, intended outcome, destination, permitted systems/actions, exclusions, acceptance checks, and recovery boundary. Preserve explicit requirements and their user source; resolve consequential ambiguity, not routine technical details. Keep one compact contract using only useful fields from [the template](references/contract-template.md).

Distinguish QUESTION/PROPOSAL/MANIFEST from EXECUTE. A question or proposed train creates nothing. “Build a train” is manifest-only until the user authorizes starting it. Requested sessions/tasks/threads are separate user-visible tasks, never substitute subagents. Delegation requires explicit authorization.

Execution authority covers the necessary implementation, setup, integration, migrations, delivery tooling, ordinary repairs, and stage transitions within the agreed actions and destination. A LOCAL destination stays local; DEVELOPMENT does not authorize PRODUCTION. Existing exclusions and explicit approval conditions remain binding. Readiness alone never expands authority. Do not import another organization's facts, accounts, data or artifacts without explicit authorization.

## Deliver autonomously

Once execution is authorized, select routine technical methods, use authorized access, dispatch existing cars, run required checks, fix in-scope defects, and advance when gates pass. Do not ask for repeat GO or permission for ordinary implementation choices. Coordinate dependencies directly rather than using the user as a relay.

Automation is part of acceptance: routine approved delivery must not depend on the user typing commands, moving credentials between tools, coordinating cars, or repeatedly confirming runs. Prefer existing native authentication, supported secure credential storage and established release tooling. Before a human handoff, verify the actual access/consent barrier and complete feasible preparation. Never assume provider policy requires manual action without evidence. Never expose secrets or bypass an actual security/approval control. New account permissions or other genuinely new authority still require authorization.

Small scripts, fixtures and integration helpers belong to implementation and receive proportionate review; do not turn each into a separate train, approval stage, or repair budget. A substantial new credential service, receipt framework, infrastructure subsystem or security model is a design expansion, not an automatic release prerequisite.

Ask the user only for an essential business/product decision, genuinely new scope/authority/expenditure, a verified personal authentication/consent action, or a consequential unresolved risk or exhausted agreed effort boundary. Present the concrete decision and smallest practical alternative. Continue independent ready work while the affected step waits.

## Use the fewest cars

Normally use a Coordinator, Builder and independent Closer. Strategy can stay with the Coordinator. The Builder owns implementation plus necessary authorized setup and delivery tooling. The Closer owns independent acceptance. Add a Promoter only for a real deployment ownership/separation need; otherwise assign promotion to an existing execution car while retaining independent acceptance.

Follow [model routing](references/car-model-routing.md). Record and verify exact task IDs, model/effort, environment and ownership at creation; preserve active configurations unless authorized to change them. Reuse suitable existing cars and worktrees. A model escalation does not imply another car.

## Review what matters

Review approved behavior, affected dependencies and material risks. Complete feasible review and return one consolidated defect list; do not drip-feed independent repair requests. If a blocker prevents review, fix it within authority and finish the remaining review. Reuse evidence still applicable to the candidate; rerun affected checks and mandatory integration/CI gates. Do not repeatedly audit a working baseline without a changed dependency or observed failure.

Evidence must match the claim: tests for deterministic behavior; actual database/runtime-role evidence for migrations, data and permissions; authenticated browser/API evidence for relevant behavior; exact deployed candidate for release; observed provider boundary for end-to-end claims. Mocks, source inspection and admin previews do not prove live persona/provider behavior. Keep unavailable proof explicit; never fabricate PASS or manufacture unauthorized shared records to obtain it.

Do not add unrelated cleanup, speculative hardening or open-ended adversarial research to an ordinary delivery. Preserve serious findings and block affected stages where justified. A local observation failure or unavailable inspection method is not proof that the remote service is broken. Optional improvements stay outside the train; required functionality is not silently dropped.

## Bound diagnosis, not every repair

After two unsuccessful attempts at the same root cause, reassess cause and approach internally. This is not an automatic approval request. Continue a materially justified in-scope approach; do not reset history by renaming a blocker, changing candidates, or replacing a car. Use a finite overall effort/recovery boundary proportionate to the task; retain an agreed time/cost limit, or state a bounded diagnostic limit at kickoff without inventing monetary approval. Do not create a fresh budget for each helper or demand repeated “one more repair” approvals.

Do not blindly retry an uncertain external write or migration. Reconcile actual state first. Before recovery/restore actions, verify exact targets, side-effecting defaults and isolation controls; rehearsal labels do not guarantee isolation. Preserve user-defined ceilings and explicit stop conditions on active trains unless the user changes them. Set repair limits for the actual task rather than imposing a universal round count.

## Keep records and supervision small

Follow [coverage and recovery](references/coverage-and-recovery.md): one current checkpoint, existing evidence links, concise handoffs, and active progress supervision. No mandatory new report, amendment, seal, or checklist for every dispatch. Preserve exact candidate identity and use hashes/seals only where they serve a concrete integrity need or existing requirement.

Close at the authorized destination with outcome, exact artifact, decisive checks, actual mutations, remaining limitations and owned-resource cleanup. PASS means agreed acceptance proven; VETO means a reviewed criterion failed; BLOCKED means safe in-scope progress needs an external change or user decision. Do not continue into optional work after completion.

## Adopt and stabilize

For an authorized active-train update, apply at the next safe handoff. Preserve completed work, valid evidence, original requirements, destination, real safeguards and current ownership. Retire redundant agent-created ceremony; identify the shortest remaining delivery path. Do not restart, re-audit everything, erase failures, override direct user ceilings, interrupt healthy operations, or create new gates to adopt this skill.

Freeze the method for one complete delivery unless the user requests a change or a concrete safety-critical defect requires correction. At closure record, when observable, user interventions and their reasons, repeated checks, delivery-tooling effort, elapsed delivery time and outcome. Do not invent measurements. Propose later changes only from demonstrated problems; do not automatically edit skills or memories.
