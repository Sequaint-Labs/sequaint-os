<!-- Written by Scotty · Agent Ops, an AI agent running on Grok Bot, under Bryan Nelson's direction. -->

# sequaint-os

**Sequaint OS** is an open pattern for running a team of AI agents with:

- **Role files** — one markdown file per agent (slug, persona, job, stores, approval gates)
- **`AGENTS.md`** — shared operating rules that every agent in a harness reads on boot
- **Linear as the task system** — work lives in Linear; knowledge lives in git; join them by issue ID ("link, don't copy")

This public repository ships the generic templates, the `sq` CLI (later), and eventually an MCP server. It does **not** contain Sequaint Labs private harnesses, personal memory, client names, or secrets.

## What's here

| Path | Purpose |
| --- | --- |
| [`templates/agent-role.md`](templates/agent-role.md) | Role-file template with YAML frontmatter |
| [`templates/AGENTS.md`](templates/AGENTS.md) | Generic harness operating rules |
| [`.github/workflows/scan.yml`](.github/workflows/scan.yml) | Secret scan (gitleaks) plus optional denylist check |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | How to contribute |
| [`LICENSE`](LICENSE) | Apache-2.0 |

## Principles (short)

1. Markdown in git is canonical for knowledge; Linear holds the work.
2. Agents are named by **function** (slug). Persona is a field in the role file, not the identifier.
3. One repo per audience; access is declared as code (`access.yaml` in private memory repos).
4. Never push private names, people, clients, or products into this public repo.

## Licence

Apache-2.0. See [LICENSE](LICENSE).

## Attribution

Written by Scotty · Agent Ops, an AI agent running on Grok Bot, under Bryan Nelson's direction.
