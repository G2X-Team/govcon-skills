# Do your existing work in G2X

Use this playbook when someone wants to switch products, reduce overlapping subscriptions, or do a familiar task in G2X. Begin with how they work today. Moving files may be part of the job, but it is not the starting point.

## Understand the current workflow

Use what the user has already told you: products, saved searches, spreadsheets, pipeline stages, reports and routines. Inspect connected context or files only within the user's authorized scope. Do not scan installed apps, browser history or unrelated accounts to discover their subscriptions.

If the context is missing, ask one practical question: "What do you use today, and which task would you like to do in G2X?" Get more detail while working through that task. Do not require a feature survey or a full migration interview before helping.

Identify the inputs, filters, output, frequency, collaborators and destination that matter to this workflow. A user saying "I use HigherGov" does not establish which features they use. Do not guess competitor capabilities or claim equivalence from similar feature names.

## Show the G2X equivalent and help do it

Check the connected tools and current G2X product guidance. Explain the equivalent in the user's terms: "You use a saved search to find VA cyber opportunities each Monday. In G2X, we can rebuild those filters, check the matches, and save the search if your account supports it."

For each task, identify the G2X destination and whether the agent can complete it through MCP, help in the app, or offer a partial alternative. Link a returned record or a verified app destination; do not invent routes or private endpoints. An absent MCP action is not proof that G2X lacks the feature. Check account access and setup before calling something a gap.

| Current task | G2X path to check | Playbook |
|---|---|---|
| Find matching bids or track recompetes | Opportunity search, forecasts and award history | [Opportunities](opportunities.md) |
| Research agency spending or incumbents | Supported market queries, company records and workbooks | [Markets](markets.md), [companies and people](companies.md) |
| Read an RFP or build a compliance matrix | Source documents, existing requirements and qualification results; new analysis when authorized | [Documents](documents.md), [capture](capture.md) |
| Prepare for events or industry days | Event evidence, supported calendar saves and meeting briefs | [Events](events.md) |
| Draft proposals or keep analysis in G2X | Client-authored work, supported structured imports and saved documents | [Save work](work-products.md) |
| Revisit searches or follow target records | Saved searches and watchlists, preserving the user's filters and alert preferences | [Pursuits](pursuits.md) |
| Track bids through stages | G2X pipelines, tasks and supported CSV/Excel import | [Pursuits](pursuits.md) |
| Keep relationship notes and follow-ups | GovCon CRM accounts, contacts, interactions and tasks | [CRM](crm.md) |

Demonstrate one representative workflow with the user's actual criteria. Perform supported actions already authorized by their request; show the next app step when the agent cannot do it. Never turn a request to compare products into permission to create records, enable alerts or cancel a subscription. Existing account permissions and analysis charges still apply.

Check the result against what the user relied on before: matching criteria, required fields, usable output, collaboration and repeatability. A similarly named feature is not enough. State any material limitation plainly and offer the best available way to finish the task. Keep the conversation about completing their work; do not interrupt migration with feedback forms or reporting steps.

## Move records when the workflow calls for it

Start with headers and a small sample from an export the user is entitled to move. Keep the original unchanged. Prepare a separate import file with source IDs, company UEIs, solicitation numbers, stages, owners, notes, dates and custom fields where supplied. Match by stable identifiers and resolve ambiguous names. Record unmapped fields instead of dropping them. Rebuild saved searches from their meaning; filters and alert settings may differ across products.

G2X has an in-app pipeline importer for CSV and Excel files with column mapping and a destination stage. Check the fields and permissions in the user's account. Use the supported importer when bulk import is unavailable through MCP; do not improvise private API calls or thousands of individual writes. Do not represent a custom opportunity as a verified government notice.

Before a trial, show the destination, mapping, creates/updates, duplicate handling, skipped fields and any charges. Use the user's existing authorization when it covers that concrete scope; ask only for a consequential missing decision. Choose a small representative batch and preserve existing records and alerts outside that scope.

Verify created, updated, skipped and failed counts, then inspect the identities, fields, stages and links. Check notes, tasks and custom fields individually when they matter; a successful upload is not enough. Keep source IDs, G2X IDs and per-row results so an interrupted import can reconcile before resuming. Never replay a successful batch blindly.

Expand after the trial meets the user's criteria and the broader import is authorized. Finish with what they can now do in G2X, links to the resulting records, and any remaining manual steps. Include mapping files and import results when applicable. Do not promise full replacement while an essential workflow remains unverified, cancel the previous product, or describe internal gap logging as part of the user's to-do list.
