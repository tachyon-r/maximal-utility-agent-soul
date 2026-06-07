# Agent Constitution

A constitutional framework for personal AI agents.

`SOUL.md` is a compact, behavior-first operating doctrine for an autonomous personal
agent — the kind that runs with real tool access (terminal, files, messaging, scheduling)
and acts on your behalf. It is not a personality prompt and not a list of tasks. It defines
**how the agent decides, acts, and reports** so that it earns trust instead of becoming
one more system you have to babysit.

## Why this exists

Most agent system prompts optimize for sounding helpful. This one optimizes for **shipped
reality without loss of trust**. The core bet:

- Trust is the precondition for accomplishment, not a constraint on it.
- An agent that fabricates, distorts, or silently guesses is worse than one that stops and asks.
- The best autonomous work is the work the owner never had to think about — and never had to clean up.

## What's in SOUL.md

A single page, nine sections:

1. **Objective Function** — explicit priority ordering (trust → objective → minimize owner involvement → momentum)
2. **Execution Doctrine** — Observe → Decide → Act → Verify → Adapt; bias to action, never guess silently
3. **Accountability** — output isn't enough; route work where it lands
4. **Autonomy** — what to do freely vs. what requires approval
5. **Delegation** — leverage without diffusing ownership
6. **Ownership** — one canonical owner per durable fact; keep SOUL small
7. **Trust Failure Protocol** — what to do the moment trust breaks
8. **Communication** — lead with the answer; compress, don't expand
9. **End State** — invisible when things work, present when they don't

## How to adopt

1. Copy [`SOUL.md`](./SOUL.md) into your agent's constitution / system-prompt slot.
   - For [Hermes Agent](https://github.com/NousResearch/hermes-agent): place it at `~/.hermes/SOUL.md`.
   - For other frameworks: paste it into whatever loads as your agent's durable identity.
2. Replace `[AGENT_NAME]` with your agent's name, and "the owner" with your name (or leave it generic).
3. Delete the template note at the top.
4. Keep state out of it. SOUL defines *behavior*; facts, preferences, and task history live elsewhere (memory, profile, project files).

## Design principles

- **Behavior over biography.** No personal data, no task lists — those drift and belong elsewhere.
- **Small is a feature.** Every line earns its place. When in doubt, cut.
- **Tradeoffs are named, not hidden.** The doctrine tells the agent *how to choose* under conflict.

## License

[MIT](./LICENSE). Use it, fork it, adapt it freely.
