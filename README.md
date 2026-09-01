# 🎫 IT Service Desk Incident Management Lab

**osTicket · Docker · MariaDB · Windows 11 · PowerShell · GitHub**

A hands-on IT Service Desk homelab designed to demonstrate practical **Level 1 IT Support and incident management skills** using a self-hosted osTicket environment.

The project simulates a real Service Desk workflow:

> **Identify → Investigate → Troubleshoot → Resolve → Verify → Document**

---

# 🎯 Project Objectives

* Deploy and configure a functional osTicket Service Desk
* Configure departments, help topics, teams, agents, and users
* Simulate realistic IT support incidents
* Practice ticket triage, prioritization, troubleshooting, and documentation
* Demonstrate professional user communication and ticket closure
* Document the environment and workflow using GitHub

---

# 🛠️ Lab Environment

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

Built the underlying Service Desk environment using Docker, Docker Compose, WSL, and MariaDB.

### Setup Evidence

### 01 — Docker Version

![Docker Version](screenshots/setup/01-docker-version.png)

Verified that Docker was installed correctly and available from the Windows environment before deploying the Service Desk application.

### 02 — Docker Hello World

![Docker Hello World](screenshots/setup/02-docker-hello-world.png)

Ran a Docker test container to confirm that the Docker engine was functioning correctly.

### 03 — Docker Compose Configuration

![Docker Compose](screenshots/setup/03-docker-compose-configuration.png)

Created the Docker Compose configuration to define the osTicket application and MariaDB database services.

### 04 — Running Containers

![Containers Running](screenshots/setup/04-containers-running.png)

Verified that the required containers were running successfully and communicating within the Docker environment.

### 05 — osTicket Service Desk

![osTicket](screenshots/setup/05-osticket-dashboard.png)

Accessed the osTicket web interface and confirmed that the Service Desk application was successfully deployed.

### Phase 1 Result

Successfully deployed a functional local osTicket Service Desk environment with MariaDB using Docker Compose and verified application availability.

---

# Phase 2 — osTicket Configuration

Configured the Service Desk structure required to simulate realistic Level 1 incident management.

### Configuration Evidence

### 06 — Admin System Settings

![Admin System Settings](screenshots/admin-config/06-admin-system-settings.png)

Reviewed and configured the core osTicket system settings to establish the basic Service Desk operating environment.

### 07 — Departments

![Departments](screenshots/admin-config/07-departments-configured.png)

Created and configured the appropriate Service Desk department structure for organizing and routing support requests.

### 08 — Help Topics

![Help Topics](screenshots/admin-config/08-help-topics-configured.png)

Configured help topics to categorize common IT support incidents and improve ticket classification during triage.

### 09 — Level I IT Support Team

![IT Support Team](screenshots/admin-config/09-it-support-team.png)

Configured the Level I IT Support team to provide a defined group for handling first-line incidents.

### 10 — Test User

![Test User](screenshots/admin-config/10-test-user-created.png)

Created a simulated end user account to generate realistic Service Desk incidents and test the complete ticket workflow.

### Phase 2 Result

Configured the core Service Desk structure, including **system settings, departments, help topics, support teams, agents, and a simulated end user**.

---

# Phase 3 — Incident Management

Phase 3 demonstrates realistic **Level 1 IT support incidents** using the configured osTicket environment.

Each incident follows a structured workflow:

**Ticket Creation → Categorization → Prioritization → Investigation → Troubleshooting → Resolution → Verification → Closure**

---

## 🎫 Ticket 01 — Microsoft 365 Login Issue

**Incident Type:** Account & Access
**Support Area:** Microsoft 365 / Authentication
**Priority:** High
**User:** Taylor Morgan
**Status:** Closed

### Incident Summary

Taylor Morgan reported an issue signing in to their Microsoft 365 account.

The incident was created and managed through the osTicket Service Desk workflow, demonstrating user creation, ticket intake, internal troubleshooting, customer communication, resolution documentation, and ticket closure.

---

### 01 — User Creation

![Ticket 01 — User Creation](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_User_Creation.png)

Created the simulated user profile for Taylor Morgan in osTicket and verified the account details before creating the incident.

---

### 02 — Ticket Created

![Ticket 01 — Created](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Created.png)

Created the Microsoft 365 login incident and documented the user's reported issue for Service Desk triage and investigation.

---

### 03 — Internal Troubleshooting

![Ticket 01 — Internal Troubleshooting](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Internal_Note.png)

Documented the troubleshooting steps performed internally to investigate the reported Microsoft 365 authentication issue.

---

### 04 — Customer Communication

![Ticket 01 — Customer Communication](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Customer_Reply.png)

Provided the user with an update on the troubleshooting progress and maintained clear communication throughout the incident.

---

### 05 — Resolution

![Ticket 01 — Resolution](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Resolution.png)

Documented the corrective action taken and verified that the Microsoft 365 login issue had been resolved successfully.

---

### 06 — Ticket Closed

![Ticket 01 — Closed](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Closed.png)

Confirmed the incident was resolved, documented the final outcome, and closed the ticket following the Service Desk workflow.

---

### Ticket 01 Result

**Outcome: Resolved and closed successfully.**

This incident demonstrates practical Level 1 Service Desk skills including:

* Incident intake and ticket creation
* User and account identification
* Ticket categorization
* Priority assignment
* Initial troubleshooting
* Internal ticket documentation
* Customer communication
* Resolution and verification
* Professional ticket closure

---

# 📋 Planned Incidents

Additional realistic incidents will be added to Phase 3 as they are completed.

| Incident              | Support Area                   | Status      |
| --------------------- | ------------------------------ | ----------- |
| Microsoft 365 Login   | Authentication / Microsoft 365 | ✅ Completed |
| Password Reset        | Account & Access               | 🔲 Planned  |
| Account Lockout       | Account & Access               | 🔲 Planned  |
| Shared Folder Access  | Permissions                    | 🔲 Planned  |
| Internet Connectivity | Networking                     | 🔲 Planned  |
| DNS Resolution        | Networking                     | 🔲 Planned  |

Each completed incident will include supporting evidence demonstrating:

**Creation → Investigation → Troubleshooting → Resolution → Verification → Closure**

---

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

### Example Windows and Networking Tools

```powershell
ipconfig /all
ping
nslookup
tracert
Test-Connection
Get-Service
Get-WinEvent
```

These tools are used to gather information, isolate common endpoint and connectivity problems, validate fixes, and support incident documentation.

---

# 📝 Ticket Documentation

Each ticket is documented using a consistent Service Desk format:

* User-reported issue
* Impact and priority
* Troubleshooting performed
* Findings
* Root cause
* Resolution
* Verification
* User communication
* Closure notes

The goal is to make every ticket understandable to another technician reviewing the incident later.

---

# 🚨 Escalation

Issues outside the scope of Level 1 support will be documented and escalated appropriately.

### Network / NOC

* Network-wide outages
* VLAN or routing issues
* Switch/router problems

### Systems Administration

* Server failures
* Complex Active Directory issues
* Group Policy problems
* Privileged access requirements

### Security

* Suspected compromised accounts
* Malware
* Suspicious authentication activity

Level 1 support focuses on resolving common endpoint, account, application, and connectivity incidents while escalating issues that require elevated access or specialized expertise.

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
│   │   ├── 01-docker-version.png
│   │   ├── 02-docker-hello-world.png
│   │   ├── 03-docker-compose-configuration.png
│   │   ├── 04-containers-running.png
│   │   └── 05-osticket-dashboard.png
│   │
│   └── admin-config/
│       ├── 06-admin-system-settings.png
│       ├── 07-departments-configured.png
│       ├── 08-help-topics-configured.png
│       ├── 09-it-support-team.png
│       └── 10-test-user-created.png
│
├── tickets/
│   ├── ticket-01-microsoft-365-login/
│   │   ├── Phase3_Ticket01_User_Creation.png
│   │   ├── Phase3_Ticket01_Created.png
│   │   ├── Phase3_Ticket01_Internal_Note.png
│   │   ├── Phase3_Ticket01_Customer_Reply.png
│   │   ├── Phase3_Ticket01_Resolution.png
│   │   └── Phase3_Ticket01_Closed.png
│   │
│   ├── ticket-02-password-reset/
│   ├── ticket-03-account-lockout/
│   ├── ticket-04-shared-folder-access/
│   ├── ticket-05-internet-connectivity/
│   └── ticket-06-dns-resolution/
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
* No sensitive production information is included

---

# 💼 Career Relevance

This project demonstrates practical skills relevant to:

**IT Support Technician · Service Desk Analyst · Help Desk Technician · Desktop Support Technician · Technical Support Specialist · NOC Technician**

The project focuses on practical first-line support activities including **ticket management, troubleshooting, user communication, documentation, prioritization, and escalation**.

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
* LinkedIn: https://linkedin.com/in/rikit-thapa-294ab028

---

**Built and documented by Rikit Thapa**

*Personal homelab and simulated IT Service Desk environment created for hands-on learning and portfolio demonstration.*
