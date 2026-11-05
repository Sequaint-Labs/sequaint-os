<!-- Written by Scotty · Agent Ops, an AI agent running on Grok Bot, under Bryan Nelson's direction. -->

# AGENTS.md (template)

Copy this file into a private harness repo and fill in the placeholders. This public template must stay free of private names, people, clients, and secrets.

## Purpose

Operating rules for every AI agent that works in this harness.

## Attribution

Every file you write, every commit message, and every PR description must start with:

> Written by \<Persona\> · \<Role\>, an AI agent running on \<platform\>, under \<Director\>'s direction.

Every commit must end with trailers:

```
Agent: <slug> (<platform>)
Directed-by: <Director>
```

Use function slugs (for example `agent-ops`), never persona-based slugs.

## Hard rules

- Never push to `main`.
- Never merge pull requests without the director's approval.
- Never send external messages, delete repositories/files, or change repo settings/collaborators without explicit approval.
- Never commit secrets, credentials, or private personal data into a public repository.

## Task system

Linear is the source of tasks. Join Linear issues to git knowledge by issue ID ("link, don't copy"). Define handoff statuses for each model/platform your team uses (for example `Needs Grok` / `Needs Claude`).

## Role files

One role file per agent under `agents/<slug>.md`, using the template in `templates/agent-role.md` from sequaint-os. Agents are named by function; persona is a frontmatter field.

## Design

If agents produce UI or design artifacts, point them at your design system path here. Do not copy brand assets into this public template.

## Routing

Document who handles inbound outside-platform messages and how they are routed to the owning agent.
