# Maximal Utility Agent SOUL

A framework-agnostic maximal-utility agent SOUL for autonomous AI agents.

This repository contains a compact SOUL / operating doctrine for agents that act instead of merely respond: coding agents, research agents, personal operators, workflow agents, and assistants with tool access. It is not a jailbreak, not a roleplay prompt, and not a task list. It defines **how an agent prioritizes, acts, escalates, verifies, and closes loops**.

## Why this exists

Most agent prompts optimize for sounding helpful. This one optimizes for **shipped reality**.

The core idea: an agent should reduce the owner's burden without becoming another system the owner has to manage.

That requires explicit doctrine for:

- what wins when goals conflict
- when to act autonomously vs. surface a blocker
- how to reconstruct intent instead of executing literal-but-wrong tasks
- how to avoid dumping solvable problems back on the owner
- how to verify work before calling it done
- how to preserve momentum without sacrificing correctness

## What's included

[`SOUL.md`](./SOUL.md) is the template. It has six sections:

1. **Priorities** — outcome first, owner burden second, momentum third; correctness breaks ties
2. **Default: Act** — act by default, ask only when blocked or judgment cannot be inferred
3. **Before Acting** — solve the real loop, not just the literal request
4. **When Blocked** — retry, reduce scope, and deliver useful partials before escalating
5. **Autonomy** — own outcomes, verify, package, and remove future friction
6. **Communication / Done** — lead with the result; work is complete only when reality changed or the blocker is explicit

## How to use it

1. Copy [`SOUL.md`](./SOUL.md) into the persistent instruction, SOUL, constitution, memory, system-prompt, policy, persona, or rules layer your agent harness supports.
2. Replace `[AGENT_NAME]` with your agent's name.
3. Replace `the owner` with your name, role, team, or leave it generic.
4. Adjust the approval boundary if your deployment has different risk tolerance or tool access.
5. Delete the template comment at the top.
6. Keep project state, credentials, contact details, task history, schedules, and preferences out of the constitution. Put those in the systems that own them.

## Where it fits

Use this as the durable behavior layer for:

- personal AI operators
- coding agents
- research agents
- executive assistants
- workflow automations
- multi-agent systems
- any assistant that can take actions instead of only chatting

Framework-specific names differ. Some systems call this a system prompt, persona, constitution, instructions file, memory, rules file, policy file, or agent profile. The point is the same: load it early and persistently enough to shape behavior across tasks.

## Design principles

- **Outcome over output.** The standard is changed reality, not a polished artifact.
- **Autonomy by default.** Act when the path is safe and inferable; surface only when blocked or judgment is genuinely required.
- **Burden reduction.** Do not make the owner the project manager, search engine, QA layer, reminder sink, or routing system.
- **Intent reconstruction.** Solve the goal behind the request, not just the literal request.
- **Verification is part of completion.** Check results in proportion to consequence.
- **Compression without sloganizing.** Keep enough detail to change behavior under pressure.

## Customization guidance

Good edits:

- change the agent/owner names
- tune communication style
- adapt approval boundaries
- add domain-specific stop conditions if the agent acts in sensitive areas
- remove sections that do not apply to your tool access

Bad edits:

- adding current projects, schedules, or contacts
- storing secrets or credentials
- turning the constitution into a workflow manual
- adding long tool catalogs
- replacing concrete approval boundaries with vague "use judgment" language

## License

[MIT](./LICENSE). Use it, fork it, adapt it freely.
