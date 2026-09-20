# Requirements, qualification and compliance

Keep three outcomes separate: extracting what the solicitation requires, assessing the company's fit, and tracking how the response satisfies each requirement. Do not label one as another.

Read an existing completed requirements package or analysis when the connected tools support it. An unavailable result is not permission to create a new paid run. The source documents and versions must match the request; do not reuse results for the wrong amendment or company profile.

When new analysis is needed, use your own model with the accessible source documents and company evidence. Choose documents deliberately: include the relevant instructions and amendments as well as the statement of work. Check the target company or profile and the intended workspace. Build the requested requirements, qualification or compliance output, keep the citations, and follow [Save work in G2X](work-products.md). A draft memo saved in the library is not the same as updating the structured requirements or qualification in a pursuit.

If the user chooses G2X-hosted analysis, use `g2x_shred_opportunity` for requirements or `g2x_qualify_opportunity` for company fit, and only when the current tools expose them. Check their current schemas, the account's access and any confirmed spending limits. Use [G2X pricing](https://g2x.com/pricing) for plan information and do not invent per-call prices. A request for a compliance matrix alone does not require a hosted run when the available evidence supports doing the work in this agent.

For a hosted run, keep the workspace and run IDs, the selected document IDs and the returned status. Poll `g2x_get_analysis_run` at the indicated interval with a bounded wait. Resume the same run after a timeout. Read `g2x_compliance_matrix` with the identifier its current schema requires; do not guess whether that is a workspace, extraction or qualification run ID. Never invent a completed run or review receipt to make an agent-authored result fit that schema.

A useful requirements output includes the requirement, its type (mandatory or desirable where supported), the evidence citation and any unresolved interpretation. A compliance output also distinguishes company evidence, response coverage, owner and review status where supported. Never mark a requirement "compliant" because it was extracted or because a model produced a plausible answer.

Return the completed artifact and its material gaps, or the pending run and the next retrieval step. The bid decision stays with the user. Updating a pipeline stage or CRM after analysis is a separate requested account action.
