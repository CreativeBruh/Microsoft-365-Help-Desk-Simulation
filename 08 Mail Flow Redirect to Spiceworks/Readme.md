08 – Mail Flow Redirect to Spiceworks

This step documents the full end‑to‑end mail‑flow integration between a Microsoft 365 shared mailbox and the Spiceworks Cloud Help Desk. By configuring a transport rule that redirects support emails to Spiceworks while preserving the original sender, this lab simulates a real‑world help desk pipeline used in enterprise environments.

The screenshots in this folder capture each stage of the workflow:
1️⃣ Shared Mailbox Settings

This screenshot shows the configuration page for the Support shared mailbox. It confirms:

    The shared mailbox was successfully created

    The correct primary email address is assigned

    Members have been granted access

    The mailbox is ready to receive incoming support requests

This establishes the source mailbox for the help desk pipeline.
2️⃣ Transport Rule Configuration

This screenshot displays the Exchange transport rule responsible for redirecting all incoming messages sent to the Support mailbox. It verifies:

    The rule is scoped to messages sent to the shared mailbox

    The action is set to Redirect the message to… the Spiceworks help desk address

    Original sender preservation is enabled

    The rule is placed at Priority 0 to ensure it executes first

This rule forms the core of the mail‑flow integration.
3️⃣ Message Trace Verification

This screenshot shows a successful message trace confirming that:

    The test email reached the Support mailbox

    The transport rule executed as expected

    The message was redirected to Spiceworks

    Delivery to the help desk system was completed

Message trace provides the audit trail proving the rule is functioning correctly.
4️⃣ Spiceworks Ticket Creation

This screenshot captures the final result: a new ticket automatically created in Spiceworks from the redirected email. It confirms:

    Spiceworks received the message

    The original sender information was preserved

    The help desk pipeline is fully operational

    The Microsoft 365 → Spiceworks integration works end‑to‑end

This completes the help desk simulation and validates the entire mail‑flow workflow.
