# Agent Constitution

A framework-agnostic constitution for autonomous AI agents.

This repository contains a compact operating doctrine for agents that act with real autonomy: coding agents, research agents, personal operators, workflow agents, and assistants with tool access. It is not a jailbreak, not a roleplay prompt, and not a task list. It defines **how an agent decides, acts, escalates, verifies, and repairs trust**.

## Why this exists

Most agent prompts optimize for sounding helpful. This one optimizes for **shipped reality without loss of trust**.

The core idea: an agent should reduce the owner's burden without becoming another system the owner has to manage.

That requires explicit doctrine for:

- what to optimize when goals conflict
- when to act autonomously vs. ask
- how to verify work before calling it done
- how to handle uncertainty and contradictory sources
- how to avoid dumping solvable problems back on the owner
- how to recover when trust is damaged

## What's included

[`SOUL.md`](./SOUL.md) is the template. It has eight sections:

1. **Objective Function** — correctness/trust, objective completion, burden reduction, momentum
2. **Operating Loop** — Observe → Validate → Decide → Act → Verify → Adapt
3. **Autonomy** — safe action by default, concrete approval boundaries for risky work
4. **Communication** — lead with the answer; separate facts, assumptions, recommendations, and uncertainty
5. **Accountability** — verification, routing, delegation, and definition of done
6. **Simplicity** — remove steps before optimizing them; prune doctrine when it stops earning its place
7. **State Ownership** — constitution defines behavior; other systems define state
8. **Trust Failure Protocol** — what to do immediately when trust is damaged

## How to use it

1. Copy [`SOUL.md`](./SOUL.md) into the persistent instruction, constitution, memory, or system-prompt layer your agent framework supports.
2. Replace `[AGENT_NAME]` with your agent's name.
3. Replace `the owner` with your name, role, team, or leave it generic.
4. Adjust the approval boundaries to match your agent's tool access and risk tolerance.
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

Framework-specific names differ. Some systems call this a system prompt, persona, constitution, instructions file, memory, rules file, or agent profile. The point is the same: this should be loaded early and persistently enough to shape behavior across tasks.

## Design principles

- **Behavior over biography.** No personal data, task lists, credentials, or current projects.
- **Autonomy with boundaries.** Act on low-risk reversible work; escalate before side effects that are costly to repair.
- **Verification is part of completion.** The standard is whether the intended reality changed.
- **State has owners.** The constitution should not become a second memory store or project tracker.
- **Trust beats momentum.** Fast work that fabricates, distorts, or hides uncertainty is not work completed.
- **Compression without sloganizing.** Keep enough detail to change behavior under pressure.

## Customization guidance

Good edits:

- change the agent/owner names
- tune communication style
- adapt approval categories
- add domain-specific risk boundaries if the agent acts in sensitive areas
- remove sections that do not apply to your tool access

Bad edits:

- adding current projects, schedules, or contacts
- storing secrets or credentials
- turning the constitution into a workflow manual
- adding long tool catalogs
- replacing concrete approval boundaries with vague "use judgment" language

## License

[MIT](./LICENSE). Use it, fork it, adapt it freely.
