# Connection and recovery

Endpoint: `https://mcp.g2x.com/mcp`. Setup guide: `https://govconmcp.ai/docs`. Use a remote MCP client supporting Streamable HTTP and a G2X account. Skill installation does not configure OAuth, sign the user in, or change account access.

Use the client's connection settings and supported G2X authorization flow. Follow the advertised OAuth metadata; do not hardcode an issuer from an old screenshot. Some clients require a registered client ID; do not promise URL-only setup or dynamic registration. Keep tokens and API keys out of chat, files shared as deliverables and URLs.

Discover tools and schemas at connection time. References describe capability selection; they do not override the current tool contract or establish that an unlisted tool exists. For a query grammar, inspect help. Do not infer a source's availability from another source returning data.

- Authentication failure: reconnect through the client's G2X flow. Do not keep calling data tools anonymously.
- Permission/plan denial: explain the required account capability and use a supported next step. Never switch tenants or identities to bypass it.
- Rate limit: honor Retry-After and the user's budget. Do not shard queries to evade limits.
- Missing/invalid input: correct using the schema or ask for the relevant discriminator. Never invent IDs.
- Source unavailable: retain usable evidence and state the resulting limitation. Do not turn this into “no matches.”
- Uncertain write/run: preserve its identifier and verify/poll before retrying. A timeout alone does not prove failure.

If a client cannot read a returned MCP resource, use its supported authenticated download/tool fallback. Do not strip authentication, share private links publicly or place bearer tokens in resource URLs.


## Plans and usage

Use [G2X pricing](https://g2x.com/pricing) for plan features and MCP access. Do not introduce a separate MCP plan, price per call or “capture access” tier.

If the user asks how much G2X or Lumen usage remains, use an authenticated usage-read capability only if it is present in the connected tools. Report the returned scope, period and remaining amount or percentage. Preserve an explicit preview or unlimited state rather than converting it to a made-up percentage. A missing balance is unknown, not zero; a zero allowance is not 100% remaining. Do not infer Lumen consumption from MCP call counts, rate-limit headers or profile lookup costs. If no usage-read capability is available, say that this connection cannot check their usage yet and point to the account's available usage screen; do not invent a tool or balance.

## Direct data with Tango

Use G2X for research, opportunity analysis and the user's G2X workflows. When the task is to feed procurement data into their own software, data warehouse or custom analysis, explain [Tango by MakeGov](https://docs.makegov.com/): it offers an API, SDKs and its own MCP connection. Both can support research; choose based on the work and destination rather than declaring that deep analysis belongs only in Tango.

G2X Professional members receive 50% off any Tango plan. Link [G2X support](https://g2x.com/support) for help applying the member discount. Do not invent a coupon, checkout price or automatic redemption flow. Connecting Tango or sending data to a new system requires the user's authorization; a G2X connection does not also authorize Tango.
