# Microsoft 365 Help Desk Simulation

A fully documented, end-to-end simulation of a Microsoft 365 help desk
environment designed to replicate common IT Support and Microsoft 365
administration responsibilities.

The project covers user provisioning, licensing, organizational structure,
shared mailboxes, delegated permissions, Exchange Online mail flow, and
integration with a third-party help desk platform.

---

## 📌 Key Skills Demonstrated

- Microsoft 365 Administration
- User & Identity Management
- License Provisioning
- Microsoft Entra ID
- Organizational Structure & Manager Hierarchies
- Shared Mailboxes & Delegated Access
- Exchange Online Transport Rules
- Mail Flow Troubleshooting & Message Trace
- Help Desk Ticketing Integration
- Technical Documentation

---

## 🛠️ Environment & Technologies

- Microsoft 365 Admin Center
- Microsoft Entra ID
- Exchange Online
- Spiceworks Cloud Help Desk
- Outlook
- Exchange Message Trace
- Exchange Mail Flow Rules

---

# 🧩 Project Walkthrough

## 1. Microsoft 365 Tenant Setup

Created and configured a Microsoft 365 tenant to serve as the foundation
for a simulated business environment.

<img width="2553" height="1265" alt="Admin Center Dashboard" src="https://github.com/user-attachments/assets/c8a5de8e-2bb3-4e22-8bd8-0a07624fc720" />


The tenant provides the administrative environment used throughout the
project for managing users, licenses, mailboxes, organizational information,
and Exchange Online configuration.

---

## 2. User Account Creation

Created employee accounts through the Microsoft 365 Admin Center to
simulate onboarding users into an organization.

<img width="1177" height="395" alt="Alex James Created" src="https://github.com/user-attachments/assets/d0a92e5c-d4c9-48d2-9bd6-1cb9a603c7c8" />
<img width="1198" height="517" alt="All Users Created" src="https://github.com/user-attachments/assets/bb066465-fa16-4ce2-a019-ceddb71351cd" />



Configured user information and credentials before validating that the
accounts were available within the tenant.

---

## 3. User Sign-In Validation

After creating and provisioning the user account, I signed in as the newly
created user to verify that the account was accessible and functioning.

<img width="2524" height="1219" alt="Alex James First Login" src="https://github.com/user-attachments/assets/116d2436-20cd-489b-82d4-e6107143bf4f" />


The successful sign-in confirmed that the account credentials were working
and that the user could access the Microsoft 365 environment.

---

## 4. Service Provisioning & Licensing

Assigned Microsoft 365 licenses to users and verified that the appropriate
services were provisioned.

<img width="937" height="528" alt="All Users Active" src="https://github.com/user-attachments/assets/448eb47a-d0cd-411e-82b3-36a7db948c70" />


This demonstrated the relationship between user accounts, licensing,
and access to Microsoft 365 services.

---

## 5. Organizational Structure

Configured departments, job titles, and manager relationships to represent
a realistic organizational hierarchy.

<img width="920" height="1157" alt="User Job Info Example" src="https://github.com/user-attachments/assets/35460177-de38-43c9-89fa-e345e5dbac51" />

These attributes created a structured company directory rather than a
collection of unrelated test accounts.

---

## 6. Microsoft 365 Org Chart

Validated manager relationships through the resulting organizational chart.

<img width="930" height="1005" alt="Manager Assignment Example" src="https://github.com/user-attachments/assets/eae4fa6a-62b7-4bed-92b0-3738eea39ced" />

This confirmed that the directory relationships configured for the
simulated employees were functioning as intended.

---

## 7. Groups & Shared Mailboxes

Created groups and a departmental Support shared mailbox to simulate
team-based communication within the organization.

<img width="994" height="983" alt="Shared Mailbox Example" src="https://github.com/user-attachments/assets/2803a7df-abff-492e-abae-19590d96ee6f" />

Configured authorized users as members of the Support mailbox and assigned
delegated permissions, including Read and Manage and Send As access.

<img width="508" height="930" alt="Shared Mailbox Settings and Delegated Permissions" src="https://github.com/user-attachments/assets/901fffbe-4347-4bbc-8ebf-12ce8dcf50a4" />

This configuration allows authorized users to access and send mail from the
shared Support address without sharing individual account credentials.

---

## 8. Spiceworks Help Desk Integration

Integrated Microsoft 365 mail flow with the Spiceworks Cloud Help Desk
to simulate an operational support workflow.

The goal was to automatically redirect messages sent to the Support shared
mailbox into Spiceworks, where they could be converted into help desk tickets.

### Exchange Transport Rule Configuration

Configured an Exchange Online mail flow rule to redirect messages sent to
the Support shared mailbox to the Spiceworks Cloud Help Desk ticketing address.

<img width="574" height="727" alt="Transport Rule Configuration" src="https://github.com/user-attachments/assets/6df5e903-119f-4033-ada5-0bc702571d23" />

The rule was enabled in Enforce mode and configured to redirect messages
addressed to the Support mailbox to the Spiceworks ticketing address.

### Message Trace Validation

Used Exchange Online Message Trace to verify that the test support message
successfully traveled through the configured mail flow.

<img width="1634" height="95" alt="Message Trace Verification" src="https://github.com/user-attachments/assets/c75d4eac-1055-4519-bef2-5c8e4de9a14f" />

This provided a way to validate message delivery and troubleshoot the mail
flow between Microsoft 365 and Spiceworks.

### Automatic Ticket Creation

Confirmed that the redirected support message automatically generated a
ticket inside the Spiceworks Cloud Help Desk.

<img width="2535" height="1266" alt="Spiceworks Ticket Creation" src="https://github.com/user-attachments/assets/91263953-9edd-4d68-ad83-a3a95e6a5163" />

This validated the complete integration between the Microsoft 365 Support
mailbox and the Spiceworks ticketing system.

### End-to-End Workflow

**User sends support request to the Support mailbox**  
↓  
**Exchange Online processes the message**  
↓  
**Transport rule redirects the message to Spiceworks**  
↓  
**Spiceworks receives the message**  
↓  
**Help desk ticket is automatically created**

---

# 🔧 Troubleshooting & Validation

Configuration alone was not considered completion. Each major component
was validated after implementation.

Validation included:

- Confirming successful user sign-ins
- Verifying Microsoft 365 service provisioning
- Checking organizational relationships
- Testing shared mailbox access
- Sending test support messages
- Reviewing Exchange Message Trace
- Confirming automatic Spiceworks ticket creation

This validation process helped identify configuration problems and verify
that the environment functioned as intended.

---

# 🎯 What I Learned

This project provided hands-on experience with Microsoft 365 administration
beyond basic user creation.

I gained practical experience managing identities, licensing, organizational
attributes, shared resources, delegated permissions, and Exchange Online
mail flow.

The Spiceworks integration also demonstrated how Microsoft 365 can interact
with an external ITSM platform and reinforced the importance of testing
and validating configurations rather than assuming a successful change.

---

# 💼 Real-World Skills Demonstrated

This lab simulates responsibilities commonly performed in IT Support,
Service Desk, and junior Microsoft 365 administration roles, including:

- Employee account provisioning
- License assignment
- Identity and directory administration
- Shared mailbox administration
- Delegated access management
- Exchange Online mail flow configuration
- Email troubleshooting
- Message tracing
- ITSM integration
- Configuration validation
- Technical documentation
