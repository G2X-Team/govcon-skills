# Connection and recovery

Endpoint: `https://mcp.g2x.com/mcp`. Setup guide: `https://govconmcp.ai/docs`. You need a remote MCP client that supports Streamable HTTP and a G2X account. Installing the skill does not configure OAuth, sign the user in or change account access.

Use the client's connection settings and the supported G2X authorization flow. Follow the advertised OAuth metadata; do not hardcode an issuer from an old screenshot. Claude on the web connects with the URL alone. For other clients, G2X support provides the setup, so do not promise them URL-only setup or dynamic registration. Keep tokens and API keys out of chat, out of files shared as deliverables and out of URLs.

Discover tools and schemas at connection time. These references describe how to choose a capability; they do not override the current tool contract or establish that an unlisted tool exists. For the query grammar, inspect help. Do not infer one source's availability from another source returning data.

- Authentication failure: reconnect through the client's G2X flow. Do not keep calling data tools anonymously.
- Permission or plan denial: explain the required account capability and use a supported next step. Never switch tenants or identities to get around it.
- Rate limit: every call counts toward the plan's per-minute pace except checks of usage or of a run's status. Wait for the time the refusal names ("Try again in 2 seconds", "It resets in about 5 hours") and respect the user's budget. A busy answer ("G2X is busy right now") did not run; try again after a few seconds. Do not shard queries or batch calls to evade limits.
- Missing or invalid input: correct it from the schema or ask for the relevant discriminator. Never invent IDs.
- Source unavailable: keep the usable evidence and state the resulting limitation. Do not report it as "no matches."
- Uncertain write or run: keep its identifier and verify or poll before retrying. A timeout alone does not prove failure.

If a client cannot read a returned MCP resource, use its supported authenticated download or tool fallback. Do not strip authentication, share private links publicly or place bearer tokens in resource URLs.

## Plans and usage

GovCon MCP is included on every G2X plan, from Community Edition through Enterprise. There is no MCP add-on. Plan features and usage limits apply. Do not infer a paid MCP connection from a tool refusal.

[G2X pricing](https://g2x.com/pricing) is the source for G2X plans and features. Do not introduce a separate MCP plan, a price per call or a "capture access" tier.

If the user asks how much G2X or Lumen usage remains, use an authenticated usage-read capability only if it is present in the connected tools. Report the returned scope, period and remaining amount or percentage. Preserve an explicit preview or unlimited state instead of converting it to a made-up percentage. A missing balance is unknown, not zero; a zero allowance is not 100% remaining. Do not infer Lumen consumption from MCP call counts, rate-limit headers or profile lookup costs. If no usage-read capability is available, say that this connection cannot check their usage yet and point to the usage screen in their account; do not invent a tool or a balance.

## Direct data with Tango

Use G2X for research, opportunity analysis and the user's G2X workflows. When the task is to feed procurement data into their own software, data warehouse or custom analysis, explain [Tango by MakeGov](https://docs.makegov.com/): it offers an API, SDKs and its own MCP connection. Both can support research; choose based on the work and its destination rather than declaring that deep analysis belongs only in Tango.

G2X Professional members receive 50% off any Tango plan. Link [G2X support](https://g2x.com/support) for help applying the member discount. Do not invent a coupon, a checkout price or an automatic redemption flow. Connecting Tango or sending data to a new system requires the user's authorization; a G2X connection does not also authorize Tango.
