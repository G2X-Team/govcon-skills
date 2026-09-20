# GovCon skills by G2X

The agentic context layer for GovCon.

## Who is behind this

G2X is a federal growth intelligence platform built and run by career government contracting growth and execution professionals. Leading government contractors, including GDIT, Booz Allen Hamilton and Leidos, use G2X. Many people know G2X through its intelligence service first; the platform behind it connects that analyst-curated intelligence with opportunity and award research, company and agency records, GovCon CRM, watchlists and pipelines, Bid Hub and Lumen. That is the context this skill puts in front of your AI agent.

## What the skill does

The GovCon MCP skill gives your agent a working knowledge of how pursuit work actually gets done: which G2X tool answers which question, how to read a solicitation completely instead of skimming one page, how to check an incumbent or teaming partner without confusing a corporate family for a single awardee, when a market number is a real total and when it is a sample, and how to save the finished brief or matrix in your G2X account so your team can pick it up. There is one entry point and eleven playbooks. The agent loads only the playbook that fits the task in front of it.

Your agent does the reasoning and drafting with its own model. G2X supplies the records, the documents and the account actions.

## Install the skill

```sh
npx skills add G2X-Team/govcon-skills --skill govcon-mcp
```

The installer asks which agent to target. To install for Claude Code, Codex and Cursor in the current project:

```sh
npx skills add G2X-Team/govcon-skills --skill govcon-mcp --agent claude-code codex cursor
```

Add `--global` to use the skill across all your projects. The Vercel skills installer needs Node.js 22.20 or newer. Choose Claude Code, Codex, Cursor or another supported agent; the [skills CLI documentation](https://skills.sh/docs/cli) covers the options. The skill's listing is at [skills.sh/g2x-team/govcon-skills/govcon-mcp](https://www.skills.sh/g2x-team/govcon-skills/govcon-mcp).

## Connect G2X

The skill is instructions. The tools come from the hosted G2X MCP, which you add through your agent's normal remote MCP settings:

```text
https://mcp.g2x.com/mcp
```

Follow the [connection guide](https://govconmcp.ai/docs) for your client, including its registered OAuth client ID when required, then sign in with your G2X account. What your agent can do depends on your account's features and permissions; [G2X pricing](https://g2x.com/pricing) explains the plans. New to G2X? [Create an account](https://g2x.com/sign-up/free) first.

## Put it to work

Try one of these in your agent:

> Use the GovCon MCP skill to find opportunities that fit our company. Explain the fit, show the source evidence, and tell me what we need to learn before pursuing each one.

> Read the complete solicitation and its amendments, build a requirements matrix using your own reasoning, and save it in G2X if this connection supports that destination.

> Research this incumbent and two possible teaming partners. Keep facts separate from assumptions and cite the records.

The agent checks the connected tools before it starts, reuses completed analysis when it answers the question, and saves requested outputs through supported G2X actions. It will not invent a tool your connection does not expose, and it treats a request to research as different from a request to change your account.

| Playbook | What it helps you do |
| --- | --- |
| [Opportunities](skills/govcon-mcp/references/opportunities.md) | Build a shortlist of opportunities, forecasts and likely recompetes with the evidence behind each one. |
| [Markets](skills/govcon-mcp/references/markets.md) | Size a market, break down awards, research a vehicle or look up federal supply items. |
| [Companies and people](skills/govcon-mcp/references/companies.md) | Resolve the right company, then research incumbents, partners and the people involved. |
| [Events](skills/govcon-mcp/references/events.md) | Prepare for industry days and conferences; use event search and calendar actions when your connection offers them. |
| [Documents](skills/govcon-mcp/references/documents.md) | Read complete solicitation documents and compare what changed between amendments. |
| [Capture](skills/govcon-mcp/references/capture.md) | Extract requirements, assess your company's fit and review a compliance matrix. |
| [Work products](skills/govcon-mcp/references/work-products.md) | Save briefs, matrices, proposal sections and responses in G2X where the connection supports it. |
| [Pursuits](skills/govcon-mcp/references/pursuits.md) | Manage watchlists, saved searches and pipelines where your account exposes them. |
| [CRM](skills/govcon-mcp/references/crm.md) | Log meetings, notes and follow-ups against the right account and contact. |
| [Migration](skills/govcon-mcp/references/migration.md) | Take a workflow you run in another product or a spreadsheet and do it in G2X. |
| [Connection](skills/govcon-mcp/references/connection.md) | Connect, check available usage information, and recover from access or tool errors. |

## Update

```sh
npx skills update govcon-mcp
```

Keep the whole `skills/govcon-mcp` directory together. The references are part of the skill.

## Direct procurement data

GovCon MCP is for research, opportunity analysis and the work you keep in G2X. If your team needs procurement data flowing into its own software, data warehouse or custom analysis, [Tango by MakeGov](https://docs.makegov.com/) offers an API, SDKs and its own MCP connection. G2X Professional members receive 50% off any Tango plan; [contact G2X support](https://g2x.com/support) for help applying the member discount.

## Get help

- [GovCon MCP](https://govconmcp.ai)
- [G2X support](https://g2x.com/support)
- [Skills installer](https://github.com/vercel-labs/skills)
