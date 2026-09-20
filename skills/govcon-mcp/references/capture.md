# Requirements, qualification and compliance

Separate three outcomes: extracting what the solicitation requires; assessing the company's fit; and tracking how the response satisfies each requirement. Do not label one as another.

Read an existing completed requirements package or analysis when the connected tools support it. An unavailable result is not permission to create a new paid run. The requested source documents and versions must match; do not reuse results for the wrong amendment or company profile.

When new analysis is needed, use your own model with the accessible source documents and company evidence. Select documents deliberately; include relevant instructions and amendments, not only the statement of work. Check the target company/profile and intended workspace. Build the requested requirements, qualification or compliance output, retain citations, and follow [Save work in G2X](work-products.md). A draft memo saved in the library is not the same as updating the structured requirements or qualification in a pursuit.

If the user chooses G2X-hosted analysis, use `g2x_shred_opportunity` for requirements or `g2x_qualify_opportunity` for company fit only when the current tools expose them. Check their current schemas, account access and any confirmed spending limits. Use [G2X pricing](https://g2x.com/pricing) for plan information; do not invent per-call prices. A request for a compliance matrix alone does not require a hosted run when the available evidence supports doing the work in this agent.

For a hosted run, retain workspace/run IDs, selected document IDs and returned status. Poll `g2x_get_analysis_run` at the indicated interval with a bounded wait. Resume the same run after timeout. Read `g2x_compliance_matrix` with the identifier required by its current schema; do not guess whether that is a workspace, extraction or qualification run ID. Never invent a completed run or review receipt to make an agent-authored result fit that schema.

A useful requirements output includes requirement, type (mandatory/desirable where supported), evidence citation and any unresolved interpretation. A compliance output also distinguishes company evidence, response coverage, owner and review status where supported. Never mark “compliant” because a requirement was extracted or because a model supplied a plausible answer.

Return the completed artifact and material gaps, or the pending run and next retrieval step. The user's accountable bid decision remains theirs. Updating pipeline stage or CRM after analysis is a separate requested account action.
