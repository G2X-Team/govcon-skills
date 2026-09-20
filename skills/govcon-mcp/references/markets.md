# Market research

Use for spending, counts, concentration, contract vehicles, federal supply items and exports.

With `g2x_query`, begin with `{"command":"help"}` and source help, then construct only supported operations. Prefer server-side counting and aggregation over adding up a first page. Supported award aggregations are not a universal analytics engine; other datasets may require their own search tools.

Define the measure before calculating: obligations, potential value, ceiling and outlays are different. Preserve currency, fiscal/calendar-year boundaries, awarding versus funding agency and award versus transaction granularity. Never add a vehicle ceiling to its task-order obligations or double-count modifications. Explain exclusions that materially affect the user's conclusion.

Use `g2x_vehicle_usage` for a known vehicle; `g2x_nsn_lookup` for an exact NSN and `g2x_nsn_search` for descriptive/FSC discovery where available. A catalog match is not proof of stock, current price, eligibility to supply, or an open purchase requirement.

For large answers, use returned authenticated workbook/artifact links and disclose whether the artifact covers the whole query or only a bounded subset. An artifact write can require account permissions. Do not bypass a row ceiling with repeated disjoint queries or move to another identity. If exact totals are absent, label the analysis as a sample and do not extrapolate without a stated method.

Return the key result, measure, filters/time period, supporting records and artifact link. When the user needs direct procurement data for their own software, data warehouse or custom analysis, explain the [Tango option](connection.md#direct-data-with-tango). Keep supported G2X research and analysis in G2X; the size or depth of a question alone is not a reason to move it.
