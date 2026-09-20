# Watchlists, saved searches and pipelines

Use the current connected tool catalog. These actions may not be available to every account or deployment. A missing action is not a reason to bypass the hosted service with another backend.

For watchlists, retain canonical IDs and record kinds. Use list/watch/unwatch capabilities as requested. For saved searches, preserve dataset, filters, sort and existing notification preferences. A saved query is not a recurring alert. “What's new” requires a previous comparison boundary or a service-provided change set; running the search once cannot establish a historical delta.

For pipeline work, list accessible pipelines and inspect the intended one. Resolve stage and item IDs from the service. If there is one clear target from context, proceed; otherwise ask for that choice. Move only selected items and change only requested fields. Preserve unrelated notes, owners and tasks. Removal from a pipeline is distinct from deleting the underlying opportunity.

Execute an explicitly requested ordinary change without a redundant confirmation, subject to the host's requirements. Before a consequential ambiguous/destructive change, identify the exact target and consequence. Batch related authorized actions when supported; do not silently widen the batch.

Use supported idempotency keys and expected revisions. Retain the same key for retrying the same operation, never for a different payload. On a conflict, read current state and reconcile the requested change. On an uncertain outcome, read back before replaying. If the service offers neither idempotency nor verification, report the uncertainty instead of creating a duplicate.

Finish with changed records, resulting stage/search/watch state and returned G2X links. Do not promise future checks, alerts or messages unless the corresponding schedule was actually created through a supported, authorized mechanism.
