# Complete documents and amendment changes

Identify the opportunity, the attachment and the relevant version. A document named "final" is not necessarily the controlling version; check the notice, amendment and attachment context.

Use a complete stored document or artifact capability when one is available. Honor the requested format: Markdown for readable text, JSON for document structure, both when asked. Preserve every supplied table, page, section and citation anchor. For large files, use the returned authenticated resource or download instead of trimming content to fit a message. Never assemble an alleged complete JSON artifact from selected passages.

`g2x_opportunity_attachment_text` may expose only one page. Read its current schema. A page read is useful for a citation, but it does not satisfy a request for the entire document. Even all pages can be incomplete if a page was truncated without continuation inside it. Follow continuation for the same artifact and version, and never join different versions without saying so. If the client exposes no complete artifact capability, explain that limit and offer a supported document link or targeted reading. Do not start extraction to compensate. Check whether a document-listing tool creates a workspace or starts processing before treating it as a plain read.

For uploads, use the client's supported file transfer and the connected G2X library capability. A local path or a file ID from another product does not mean G2X has the bytes. For a client without file transfer, use an available G2X upload flow and resume with the returned document reference. Verify the stored document, destination and version before proceeding. Do not send a large file as base64 in an ordinary tool argument, and do not recover connection credentials to upload it.

If text is unavailable, use explicit parsing or OCR when it is supported and authorized. Parsing a source does not authorize qualification, requirements analysis or enrichment. Keep a returned operation ID and resume it rather than starting another job. Use your model to analyze the retrieved content, then follow [Save work in G2X](work-products.md) for the resulting document or structured work.

For amendment comparisons, establish both versions and the affected documents. Compare deadline, submission instructions, scope, quantities, evaluation criteria and changed requirements. Return old -> new meaning with file, page and section citations. Mark conclusions that are limited to the documents actually available; do not assert "no changes" from partial text. Do not offer an opinion that a requirement is legally waived.

If extracted requirements already exist, return them with citations. Extracted rows are not evidence that the user's company complies. Use the [capture playbook](capture.md) only when the user needs additional analysis.
