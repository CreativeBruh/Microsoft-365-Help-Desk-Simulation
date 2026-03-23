# Microsoft-365-Help-Desk-Simulation
A complete Microsoft 365 help desk simulation demonstrating shared mailbox management, mail flow configuration, transport rules, and integration with a cloud-based ticketing system. This lab replicates real-world IT support workflows from email intake to automated ticket creation.


📌 Overview

This project simulates a real enterprise help desk environment using Microsoft 365 and Spiceworks Cloud Help Desk.
It demonstrates how support emails sent to a shared mailbox can be automatically routed, processed, and converted into help desk tickets — mirroring the workflows used by actual IT support teams.
🧱 What This Lab Covers

    Microsoft 365 shared mailbox administration

    Mail flow and transport rule configuration

    Redirect‑based routing (preserves original sender)

    Message trace verification

    Integration with Spiceworks Cloud Help Desk

    Automatic ticket creation

    Realistic help desk workflow behavior

This lab showcases both technical and operational skills expected in entry‑level IT roles.
📂 Project Structure
Code

08 – Mail Flow Redirect to Spiceworks
│
├── 01 – Shared Mailbox Settings
│     (Support mailbox configuration)
│
├── 02 – Transport Rule Configuration
│     (Redirect rule setup and validation)
│
├── 03 – Message Trace Verification
│     (Proof of delivery and rule execution)
│
└── 04 – Spiceworks Ticket Creation
      (Final ticket generated from redirected email)

Each folder contains screenshots and documentation for that stage of the workflow.
🛠️ Technical Workflow
1️⃣ Shared Mailbox Setup

Created a Microsoft 365 shared mailbox named Support to receive help desk requests.
Verified forwarding was disabled to ensure proper sender preservation.
2️⃣ Mail Flow Redirect Rule

Configured a transport rule to:

    Detect messages sent to the Support mailbox

    Redirect them to the Spiceworks help desk address

    Preserve the original sender

    Run with highest priority (Priority 0)

Redirecting (not forwarding) is essential because forwarding rewrites the sender, which breaks ticket creation.
3️⃣ Message Trace Verification

Used Microsoft 365 Message Trace to confirm:

    Delivery to the Support mailbox

    Execution of the redirect rule

    Routing to Spiceworks

This step mirrors real-world troubleshooting and auditing.
4️⃣ Automatic Ticket Creation

Verified that Spiceworks successfully created a help desk ticket from the redirected email.
Example: Ticket ID 3 – “My dog is not working”

This confirms the entire pipeline is functioning end‑to‑end.
🔍 Troubleshooting Highlights

During the lab, several real-world issues were encountered and resolved:

    Transport rule initially created in Disabled mode

    Message trace showing only “Delivered”

    Rule priority adjustments

    Validation of redirect vs. forward behavior

These steps demonstrate practical troubleshooting and operational awareness.
🎯 Skills Demonstrated

    Microsoft 365 administration

    Shared mailbox management

    Mail flow and transport rules

    Redirect vs. forward behavior

    Message trace analysis

    Ticketing system integration

    Realistic help desk workflow simulation

    Professional documentation practices

📌 Why This Project Matters

This lab demonstrates the exact workflows used by IT support teams in real organizations.
It shows not only technical ability but also:

    Understanding of operational processes

    Ability to troubleshoot mail flow

    Awareness of sender preservation and security considerations

    Experience integrating Microsoft 365 with third‑party systems

