<!-- Written by Scotty · Agent Ops, an AI agent running on Grok Bot, under Bryan Nelson's direction. -->

---
slug: example-agent
persona: ExamplePersona
job: One-line description of what this agent owns.
reads:
  - path/or/store
writes:
  - path/or/store
approval_required:
  - merge pull requests
  - push to main
  - send external messages
  - delete files or repositories
written_by: agent-ops
directed_by: Bryan Nelson
---

# example-agent

## Role

Describe the agent's charter: what it owns, what it does not own, and how it collaborates.

## Operating rules

- Follow the harness `AGENTS.md`.
- Attribute every file, commit, and PR description per the attribution rule.
- Do not merge, push to `main`, send, or delete without the directed-by person's approval.

## Stores

| Access | Store | Notes |
| --- | --- | --- |
| read | … | … |
| write | … | … |

## Handoffs

Who this agent hands work to, and which Linear statuses or labels trigger a handoff.
