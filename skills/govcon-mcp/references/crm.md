# GovCon CRM

Work in the signed-in user's G2X CRM. Do not route the request to an unrelated CRM provider. Resolve the account or contact with `g2x_crm_find` and inspect it with `g2x_crm_get_record` before updating anything.

Match companies and people with stable IDs and supporting identity evidence. Do not create a duplicate because a display name varies. If two plausible contacts remain, ask for the distinguishing detail before logging an interaction against one of them.

Use the smallest action that satisfies the request: save an account or contact, add a note, log an interaction, set a follow-up or add a task. Preserve existing fields the user did not supply. Record meeting content faithfully, and distinguish what a participant said from what they verifiably committed to. Resolve dates and time zones for follow-ups, and do not invent an owner.

A specific request to update CRM authorizes the described change, subject to permissions and host requirements. Research alone does not. Sending an email or invitation is separate from writing a note or a follow-up task; do not send outreach through another tool because a CRM record contains an address.

Use supported idempotency and revision controls. Read back after the action, especially after a timeout, before retrying. An accepted request is not proof that the record changed. Return the changed fields and the canonical record link, or explain the exact action that did not complete. Do not work around an account or administrator-session restriction by changing identity.
