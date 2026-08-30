# 🎫 IT Service Desk Incident Management Lab

**osTicket · Docker · MariaDB · Windows 11 · PowerShell · GitHub**

A hands-on IT Service Desk homelab designed to demonstrate practical **Level 1 IT Support and incident management skills** using a self-hosted osTicket environment.

The project simulates a real Service Desk workflow:

> **Identify → Investigate → Troubleshoot → Resolve → Verify → Document**

---

## 🎯 Project Objectives

* Deploy and configure a functional osTicket Service Desk
* Configure departments, help topics, teams, agents, and users
* Simulate realistic IT support incidents
* Practice ticket triage, prioritization, troubleshooting, and documentation
* Demonstrate professional user communication and ticket closure
* Document the environment and workflow using GitHub

---

## 🛠️ Lab Environment

| Component         | Technology              |
| ----------------- | ----------------------- |
| Host OS           | Windows 11              |
| Ticketing System  | osTicket 1.18.4         |
| Deployment        | Docker / Docker Compose |
| Database          | MariaDB 10.11           |
| Linux Environment | WSL 2 / Ubuntu          |
| Scripting         | PowerShell              |
| Version Control   | Git / GitHub            |

---

# Phase 1 — Environment Setup

Built the underlying Service Desk environment using Docker and Docker Compose.

### Setup Evidence

**01 — Docker Version**

![Docker Version](screenshots/setup/01-docker-version.png)

**02 — Docker Hello World**

![Docker Hello World](screenshots/setup/02-docker-hello-world.png)

**03 — Docker Compose Configuration**

![Docker Compose](screenshots/setup/03-docker-compose-configuration.png)

**04 — Running Containers**

![Containers Running](screenshots/setup/04-containers-running.png)

**05 — osTicket Service Desk**

![osTicket](screenshots/setup/05-osticket-dashboard.png)

### Phase 1 Result

Successfully deployed a local osTicket environment with MariaDB using Docker Compose and verified application availability through the web interface.

---

# Phase 2 — osTicket Configuration

Configured the Service Desk structure required for realistic incident management.

### Configuration Evidence

**06 — Admin System Settings**

![Admin System Settings](screenshots/admin-config/06-admin-system-settings.png)

**07 — Departments**

![Departments](screenshots/admin-config/07-departments-configured.png)

**08 — Help Topics**

![Help Topics](screenshots/admin-config/08-help-topics-configured.png)

**09 — Level I IT Support Team**

![IT Support Team](screenshots/admin-config/09-it-support-team.png)

**10 — Test User**

![Test User](screenshots/admin-config/10-test-user-created.png)

### Phase 2 Result

Configured the basic Service Desk structure, including **departments, help topics, support teams, agents, and a simulated end user**.

---

# Phase 3 — Incident Management

Phase 3 demonstrates realistic **Level 1 IT Service Desk incident management** using the configured osTicket environment.

Each incident follows a structured Service Desk workflow:

**Ticket Creation → Categorization → Prioritization → Investigation → Troubleshooting → Resolution → Verification → Closure**

---

## 🎫 Ticket 01 — Microsoft 365 Login Issue

**User:** Taylor Morgan
**Category:** Account & Access / Authentication
**Priority:** High
**Status:** Closed

### Incident

Taylor Morgan reported being unable to sign in to their Microsoft 365 account and access Outlook and Microsoft Teams.

### Troubleshooting

The incident was investigated using a structured first-line troubleshooting approach. Account authentication and access were reviewed, the issue was addressed, and access was successfully restored.

### Resolution

Microsoft 365 account access was restored and successfully verified. The user was informed that Outlook and Microsoft Teams access were working again.

### Ticket Evidence

**01 — User / Ticket Submission**

![Ticket 01 Submission](tickets/ticket-01-microsoft-365-login/01-ticket-submission.png)

**02 — Ticket Details**

![Ticket 01 Details](tickets/ticket-01-microsoft-365-login/02-ticket-details.png)

**03 — Internal Troubleshooting**

![Ticket 01 Internal Note](tickets/ticket-01-microsoft-365-login/03-internal-troubleshooting.png)

**04 — Customer Communication**

![Ticket 01 Customer Reply](tickets/ticket-01-microsoft-365-login/04-customer-communication.png)

**05 — Resolution**

![Ticket 01 Resolution](tickets/ticket-01-microsoft-365-login/05-resolution.png)

**06 — Ticket Closed**

![Ticket 01 Closed](tickets/ticket-01-microsoft-365-login/06-ticket-closed.png)

### Ticket 01 Result

Successfully created, categorized, prioritized, investigated, documented, resolved, and closed a simulated Microsoft 365 authentication incident while maintaining professional ticket documentation and user communication.

---

## 🔜 Upcoming Incidents

Additional incidents will be added to demonstrate a broader range of Level 1 troubleshooting skills:

| Incident                    | Support Area     |
| --------------------------- | ---------------- |
| Password Reset              | Account & Access |
| Account Lockout             | Account & Access |
| Shared Folder Access        | Permissions      |
| Internet Connectivity       | Networking       |
| DNS Resolution              | Networking       |
| VPN Connectivity            | Remote Access    |
| Slow Computer               | Windows          |
| Application Failure         | Software         |
| MFA / Login Issue           | Authentication   |
| Hardware / Peripheral Issue | Hardware         |


# 🔎 Troubleshooting Approach

Incidents are handled using a structured first-line troubleshooting methodology:

```text
Understand the Issue
        ↓
Gather Information
        ↓
Perform Initial Checks
        ↓
Isolate the Cause
        ↓
Apply the Fix
        ↓
Verify the Resolution
        ↓
Document the Work
        ↓
Escalate if Required
```

Example Windows and networking tools:

```powershell
ipconfig /all
ping
nslookup
tracert
Test-Connection
Get-Service
Get-WinEvent
```

---

# 📝 Ticket Documentation

Tickets will contain concise, professional documentation such as:

* User-reported issue
* Impact and priority
* Troubleshooting performed
* Findings
* Root cause
* Resolution
* Verification
* User communication
* Closure notes

---

# 🚨 Escalation

Issues outside the scope of Level 1 support will be documented and escalated appropriately.

Examples:

**Network / NOC**

* Network-wide outage
* VLAN or routing issues
* Switch/router problems

**Systems Administration**

* Server failures
* Complex Active Directory issues
* Group Policy problems
* Privileged access requirements

**Security**

* Suspected compromised accounts
* Malware
* Suspicious authentication activity

---

# 🏆 Skills Demonstrated

### Service Desk

Incident Management · Ticket Triage · Prioritization · Documentation · User Communication · Escalation

### Technical Support

Windows · Networking · DNS · TCP/IP · Account & Access · Basic PowerShell

### Tools

osTicket · Docker · Docker Compose · MariaDB · WSL · Git · GitHub

---

# 📂 Repository Structure

```text
IT-Service-Desk-Incident-Management-Lab/
│
├── README.md
├── docker-compose.yml
│
├── screenshots/
│   ├── setup/
│   └── admin-config/
│
├── tickets/
│
└── documentation/
```

---

# 🔐 Security

This is a personal homelab and portfolio project.

* All users and incidents are simulated
* No real customer or company information is used
* Credentials and secrets are excluded from the repository
* Screenshots are reviewed before publication

---

# 💼 Career Relevance

This project demonstrates practical skills relevant to:

**IT Support Technician · Service Desk Analyst · Help Desk Technician · Desktop Support Technician · Technical Support Specialist · NOC Technician**

---

# 👤 About

**Rikit Thapa**

Computer Systems Networking Technician focused on entry-level **IT Support, Service Desk, Desktop Support, and NOC** opportunities.

### Certifications

**CCNA · Microsoft Azure Fundamentals (AZ-900) · Fortinet Certified Associate in Cybersecurity**

### Technical Focus

**Windows · Active Directory · Microsoft 365 · Networking · PowerShell · Troubleshooting · Service Desk**

---

## 🔗 Professional Links

* GitHub: https://github.com/rikit03
* Portfolio: https://rikit03.github.io/portfolio
* LinkedIn: https://linkedin.com/in/rikit-thapa-294ab028a

---

**Built and documented by Rikit Thapa**

*Personal homelab and simulated IT Service Desk environment created for hands-on learning and portfolio demonstration.*
