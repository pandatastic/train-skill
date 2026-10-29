# Train Skill

A reusable Codex skill for delivering substantial work through a small set of
coordinated tasks: **build → independent review → repair → verify → deliver**.

Agree the scope and destination once. Let the Coordinator handle ordinary
implementation choices, handoffs and repairs within that agreement. Keep
acceptance tied to evidence and stop at the authorized destination.

## Download

- [Latest installable ZIP](https://github.com/pandatastic/train-skill/releases/latest/download/train-skill.zip)
- [Versioned releases](https://github.com/pandatastic/train-skill/releases)

The ZIP includes this README, the MIT license and the complete skill with all
supporting references. It contains no executable installer.

## Install from the ZIP

1. Download and extract the ZIP.
2. Open the extracted folder, then `skills/`.
3. Copy the entire `train-skill` folder into your personal `~/.agents/skills/`
   folder. Create that parent folder if needed.
4. Confirm that `~/.agents/skills/train-skill/SKILL.md` exists, with
   `references/` beside it. Keep the complete folder together.

On Windows, use the `.agents/skills/` folder inside your user home directory.
Codex detects newly installed skills automatically; restart it if the skill
does not appear. Back up or review an existing installation before replacing it.

## Install from Git

Clone this repository into a location of your choice:

```sh
git clone https://github.com/pandatastic/train-skill.git
```

Copy `train-skill/skills/train-skill/` into your personal `~/.agents/skills/`
folder as described above. For a skill shared only within one project, copy
that folder to the project's `.agents/skills/train-skill/` and commit it there.

Alternatively, ask Codex to use its built-in installer:

```text
Use $skill-installer to install the skill from
https://github.com/pandatastic/train-skill/tree/main/skills/train-skill
```

An installation is a snapshot. To update it, review a newer release and replace
the installed folder; pulling the source repository alone does not update a
separately copied installation. Avoid installing the same skill in multiple
discovery locations unless that is intentional.

## Use it

In Codex CLI or the IDE extension, mention `$train-skill`. On surfaces with a
skill picker, select Train Skill using the available picker. Codex can also
select the skill when the request matches its description.

Start with a plan:

```text
Use $train-skill to propose the smallest train for adding a CSV export to
this project. Inspect the existing implementation, define acceptance evidence,
and keep the destination local. Do not create or start tasks yet.
```

After reviewing the plan, authorize execution with specific boundaries:

```text
Create and start the proposed train with the models and limits in its manifest.
Complete the local implementation and independent acceptance. Do not push,
deploy, or change shared systems. Stop at the agreed local destination.
```

When you request sessions, tasks or threads, each car is a separate user-visible
task. Subagents require explicit authorization and do not replace requested cars.

Shared method revision: **2026-10-28a**, released in **v1.2.0**.

## What the skill provides

- A compact delivery contract: outcome, authority, destination, exclusions,
  acceptance evidence and an overall recovery boundary.
- A Coordinator, Builder and independent Closer, with extra cars only when
  there is a concrete need.
- Consolidated review and repair, reuse of still-valid evidence, and proportionate
  checks against the actual candidate.
- Guidance for reusing project verification helpers, isolated database environments
  and review access across repairs and handoffs.
- Concise checkpoints and bounded recovery from stalls or failed approaches.
- Early acceptance feasibility, fixed-candidate evidence and serialized promotion.
- A final PASS, VETO or BLOCKED result with decisive evidence and one compact
  closure receipt; unavailable measurements remain unknown.

## Configure it for your environment

Choose exact models, supported reasoning levels and cost or effort limits in
the manifest. No particular model or provider is required by this package.
The core instructions can inform other agents, but the task-creation workflow
is written for Codex.

Separate task creation, status inspection, browser/API verification and scheduled
monitoring depend on capabilities available in the recipient's environment.
The skill does not install tools, grant permissions, supply credentials or
configure recurring automations. Agree a monitoring cadence when needed;
recurring monitoring requires authorization and a supported scheduler.

Keep project-specific rules, accounts, endpoints and release permissions in the
recipient's own private overlays, project instructions or delivery contract.
Record overlay revisions separately. Preserve current model routing; this release
does not change models, install telemetry instrumentation or migrate active trains. Installing the skill does not authorize execution, deployment or changes to external systems.

## Package contents

```text
README.md
LICENSE
skills/
  train-skill/
    SKILL.md
    references/
      contract-template.md
      car-model-routing.md
      coverage-and-recovery.md
      verification-reuse.md
      acceptance-and-promotion.md
      checkpoint-examples.md
      closure-telemetry.md
```

Official guidance: [Build skills](https://learn.chatgpt.com/docs/build-skills).
For broader installable distribution, OpenAI also supports packaging skills
as plugins; this repository provides the direct skill-folder format.

## License

MIT. You may use, adapt and redistribute the skill under the included license.
