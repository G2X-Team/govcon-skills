# Opportunity discovery

Use this playbook for a pursuit shortlist, an opportunity search, a forecast scan or a recompete watch.

Start with the user's company and the market they named. Pull the relevant NAICS and PSC codes, set-asides, agencies, geography, contract size and deadlines from the context they supplied or from profile evidence you can access. Do not invent certifications or past performance. Ask for a missing discriminator only when it would change the search materially.

Prefer `g2x_query` for structured filtering, counts and a bounded complete list. Read its `help` and the relevant source help instead of assuming which filters exist. Use `g2x_search_supplementary` to search text inside attachments or across the supported opportunity sources. Use the narrower opportunity search for a quick topical shortlist. Forecasts, expiring awards and recompete candidates each have their own tools, and none of them is an open solicitation; do not present them as one.

Carry filters and returned cursors consistently through the search. Deduplicate by canonical record and version, and do not merge different notices just because their titles match. Stop at the scope or budget the user set. Keep the difference between records shown, total matches and a truncated result visible in what you report.

For each recommended pursuit, give the agency, notice type, response deadline (with time zone when provided), the fit rationale, the evidence behind it and a G2X link. Separate mandatory eligibility from softer fit signals. A likely follow-on is not a confirmed forthcoming solicitation, and an award that ends soon does not establish a recompete date.

When the user asks you to "find work and save the best matches," research first, then follow the [pursuit-management playbook](pursuits.md) for the matches that meet their stated criteria. Ask only if the selection criteria or destination is ambiguous. Do not change the user's saved-search notification preferences as a side effect of research.
