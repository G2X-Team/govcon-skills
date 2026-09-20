# GovCon skills by G2X

The agentic context layer for GovCon.

Give your agent a practical way to research opportunities, analyze solicitations, prepare for meetings, and manage work in your G2X account. The **GovCon MCP** skill contains eleven focused playbooks and loads the guidance relevant to your task.

## Install the skill

```sh
npx skills add command3rkeen/govcon-skills --skill govcon-mcp
```

Choose your agent when prompted. To target Claude Code, Codex, and Cursor in your current project:

```sh
npx skills add command3rkeen/govcon-skills --skill govcon-mcp --agent claude-code codex cursor
```

Add `--global` to make the skill available across your projects. The Vercel skills installer currently requires Node.js 22.20 or newer. See the [skills CLI documentation](https://skills.sh/docs/cli) for installation options.

## Connect G2X

Add the hosted G2X MCP through your agent's normal remote MCP connection settings:

```text
https://mcp.g2x.com/mcp
```

Sign in with your G2X account. Follow the [connection guide](https://govconmcp.ai/docs) for your client. Installing this skill adds instructions; your client's MCP connection provides the tools. Account features and permissions apply. See [G2X pricing](https://g2x.com/pricing).

## Put it to work

Try a request such as:

> Use the GovCon MCP skill to research opportunities that fit our company. Explain the fit, show the source evidence, and identify what we need to learn before pursuing each one.

Or:

> Read the complete solicitation, build a requirements matrix using your own reasoning, and save it in G2X if this connection supports that destination.

The skill uses your chosen agent for reasoning and drafting by default. It checks the connected tools before starting work, reuses completed analysis when appropriate, and saves requested outputs through supported G2X actions. It does not add capabilities that your connection does not expose.

| Playbook | What it helps you do |
| --- | --- |
| [Opportunities](skills/govcon-mcp/references/opportunities.md) | Find and narrow opportunities, forecasts, and recompetes. |
| [Markets](skills/govcon-mcp/references/markets.md) | Size a market and research awards, vehicles, or NSNs. |
| [Companies and people](skills/govcon-mcp/references/companies.md) | Resolve companies and research incumbents, partners, and people. |
| [Events](skills/govcon-mcp/references/events.md) | Find available event context and prepare for meetings and follow-up. |
| [Documents](skills/govcon-mcp/references/documents.md) | Read complete documents and compare amendments. |
| [Capture](skills/govcon-mcp/references/capture.md) | Extract requirements, assess fit, and review compliance. |
| [Work products](skills/govcon-mcp/references/work-products.md) | Save supported briefs, matrices, proposals, and responses in G2X. |
| [Pursuits](skills/govcon-mcp/references/pursuits.md) | Work with watchlists, saved searches, and pipelines where available. |
| [CRM](skills/govcon-mcp/references/crm.md) | Make requested updates to accounts, contacts, notes, and follow-ups. |
| [Migration](skills/govcon-mcp/references/migration.md) | Map an existing workflow to the available G2X equivalent. |
| [Connection](skills/govcon-mcp/references/connection.md) | Connect, check available usage information, and recover from access errors. |

## Update

```sh
npx skills update govcon-mcp
```

Keep the entire `skills/govcon-mcp` directory together. Its references are part of the skill.

## Get help

- [GovCon MCP](https://govconmcp.ai)
- [G2X support](https://g2x.com/support)
- [Skills installer](https://github.com/vercel-labs/skills)
