# GovCon CRM

Use the signed-in user's G2X CRM capabilities, not an unrelated CRM provider. Resolve the account/contact with `g2x_crm_find` and inspect it with `g2x_crm_get_record` before updating.

Match companies and people with stable IDs and supporting identity evidence. Do not create a duplicate because of a display-name variation. If two plausible contacts remain, ask for the distinguishing detail before logging an interaction on one of them.

Use the smallest requested action: save account/contact, add note, log interaction, set follow-up or add task. Preserve existing fields not supplied by the user. Record meeting content faithfully; distinguish a participant's statement from a verified commitment. Resolve dates and timezone for follow-ups, and do not invent an owner.

A specific user request to update CRM authorizes that described change, subject to permissions and host requirements. Research alone does not. Sending an email or invitation is separate from writing a note or follow-up task. Do not send outreach through another tool because a CRM record contains an address.

Use supported idempotency/revision controls. Read back after the action, especially after a timeout, before retrying. An accepted request is not proof that the record changed. Return changed fields and the canonical record link, or explain the exact uncompleted action. Do not work around an account or administrator-session restriction by changing identity.
