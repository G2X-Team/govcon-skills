# Watchlists, saved searches and pipelines

Use the current connected tool catalog. These actions may not be available to every account or deployment, and a missing action is not a reason to bypass the hosted service with another backend.

For watchlists, keep canonical IDs and record kinds. Use the list, watch and unwatch capabilities as requested. For saved searches, preserve the dataset, filters, sort and existing notification preferences. A saved query is not a recurring alert. "What's new" needs a previous comparison boundary or a service-provided change set; running the search once cannot establish a historical delta.

For pipeline work, list the accessible pipelines and inspect the intended one. Resolve stage and item IDs from the service. If the context gives one clear target, proceed; otherwise ask for that choice. Move only the selected items and change only the requested fields. Preserve unrelated notes, owners and tasks. Removing an item from a pipeline is distinct from deleting the underlying opportunity.

Carry out an explicitly requested ordinary change without a redundant confirmation, subject to the host's requirements. Before a consequential ambiguous or destructive change, identify the exact target and consequence. Batch related authorized actions when supported, and keep the batch within the user's authorized scope.

Use supported idempotency keys and expected revisions. Keep the same key when retrying the same operation, never for a different payload. On a conflict, read the current state and reconcile the requested change. On an uncertain outcome, read back before replaying. If the service offers neither idempotency nor verification, report the uncertainty instead of creating a duplicate.

Finish with the changed records, the resulting stage, search or watch state, and the returned G2X links. Do not promise future checks, alerts or messages unless the corresponding schedule was actually created through a supported, authorized mechanism.
