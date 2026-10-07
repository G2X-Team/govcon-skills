# Opportunity discovery

Use this playbook for a pursuit shortlist, an opportunity search, a forecast scan or a recompete watch.

Start from the calibrated profile (see "Calibrate the session first" in the skill) and the goal the user named. The profile gives the default NAICS codes, agencies, and set-asides or certifications. Add the words of the user's goal and any PSC codes, geography, contract size or deadlines they supplied. Without a profile, work from the context the user gave, and ask the setup questions only when a missing detail would change the search materially. Do not invent certifications or past performance.

Turn the profile into queries:

- Open opportunities: `g2x_search_opportunities` with `naics_codes` from the profile, plus words from the user's goal.
- Other datasets: `g2x_search_records` with `filters` from the keys that dataset takes. The tool's description lists the opportunity keys, such as `naics`, `agency_code` and `set_aside`; other datasets take their own, and an unknown key is refused with the list.
- When the user wants notices whose documents they can read, add `with_readable_documents: true` if the search offers it.

A value the user names for one search (a different NAICS, agency, set-aside or place) replaces the profile's value for that query only. Say which profile values you set aside, then go back to the profile.

Prefer `g2x_query` for structured filtering, counts and a bounded complete list. Read its `help` and the relevant source help instead of assuming which filters exist. Use `g2x_search_supplementary` to search text inside attachments or across the supported opportunity sources. Use the narrower opportunity search for a quick topical shortlist. Forecasts, expiring awards and recompete candidates each have their own tools, and none of them is an open solicitation; do not present them as one.

Carry filters and returned cursors consistently through the search. Deduplicate by canonical record and version, and do not merge different notices just because their titles match. Stop at the scope or budget the user set. Keep the difference between records shown, total matches and a truncated result visible in what you report.

For each recommended pursuit, give the agency, notice type, response deadline (with time zone when provided), the fit rationale, the evidence behind it and a G2X link. Separate mandatory eligibility from softer fit signals. A likely follow-on is not a confirmed forthcoming solicitation, and an award that ends soon does not establish a recompete date.

When the user asks you to "find work and save the best matches," research first, then follow the [pursuit-management playbook](pursuits.md) for the matches that meet their stated criteria. Ask only if the selection criteria or destination is ambiguous. Do not change the user's saved-search notification preferences as a side effect of research.
