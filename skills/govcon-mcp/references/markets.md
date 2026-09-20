# Market research

Use this playbook for spending, counts, concentration, contract vehicles, federal supply items and exports.

With `g2x_query`, start with `{"command":"help"}` and the source help, then build only supported operations. Prefer server-side counting and aggregation to adding up a first page yourself. The supported award aggregations are not a general analytics engine; other datasets may need their own search tools.

Define the measure before you calculate anything. Obligations, potential value, ceiling and outlays are different numbers. Preserve currency, fiscal versus calendar year boundaries, awarding versus funding agency, and award versus transaction granularity. Never add a vehicle's ceiling to its task-order obligations, and never double-count modifications. Explain any exclusion that would change the user's conclusion.

Use `g2x_vehicle_usage` for a known vehicle. Use `g2x_nsn_lookup` for an exact NSN and `g2x_nsn_search` for descriptive or FSC discovery where it is available. A catalog match does not prove stock, current price, eligibility to supply or an open purchase requirement.

For large answers, use the returned authenticated workbook or artifact links and say whether the artifact covers the whole query or a bounded subset. Writing an artifact can require account permissions. Do not get around a row ceiling with repeated disjoint queries, and do not switch to another identity. If exact totals are unavailable, label the analysis as a sample and do not extrapolate without stating the method.

Return the key result, the measure, the filters and time period, the supporting records and the artifact link. When the user needs direct procurement data in their own software, data warehouse or custom analysis, explain the [Tango option](connection.md#direct-data-with-tango). Keep supported G2X research and analysis in G2X; the size or depth of a question is not by itself a reason to move it elsewhere.
