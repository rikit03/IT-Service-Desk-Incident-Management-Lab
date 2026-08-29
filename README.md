# 🎫 IT Service Desk Incident Management Lab

**osTicket • Docker • Windows 11 • PowerShell • Networking • Incident Management**

A hands-on Service Desk lab designed to demonstrate practical **Level 1 IT Support, incident management, troubleshooting, documentation, and user communication** skills through a locally deployed osTicket environment.

The project simulates a small-business IT Service Desk where users report technical issues and a support technician follows a structured process from **ticket intake to resolution and closure**.

> **Identify → Investigate → Troubleshoot → Resolve → Verify → Document**

---

## 🎯 Project Objectives

This lab demonstrates the ability to:

* Create and manage support tickets
* Gather relevant technical information
* Categorize and prioritize incidents
* Troubleshoot Windows, network, software, hardware, and access issues
* Identify probable root causes
* Apply appropriate resolutions
* Verify that issues are resolved
* Communicate clearly with users
* Document technical work professionally
* Recognize when escalation is required
* Follow a consistent ticket lifecycle

---

# 🏢 Business Scenario

A small organization requires a centralized IT Service Desk to handle employee technical issues.

Users submit incidents involving:

* Account and password problems
* Windows issues
* Network connectivity
* DNS and VPN problems
* Software issues
* Hardware/peripheral problems
* Shared resource access
* MFA and authentication

The Service Desk technician investigates each incident, documents the troubleshooting process, resolves or escalates the issue, verifies the result, and closes the ticket.

---

# 🛠️ Technologies & Tools

| Area              | Technologies / Tools                   |
| ----------------- | -------------------------------------- |
| Ticketing         | osTicket                               |
| Deployment        | Docker Desktop, Docker Compose         |
| Container Backend | WSL 2, Ubuntu 24.04                    |
| Operating System  | Windows 11                             |
| Database          | MariaDB 10.11                          |
| Troubleshooting   | PowerShell, Command Prompt             |
| Windows Tools     | Event Viewer, Device Manager, Services |
| Networking        | TCP/IP, IPv4, DNS, DHCP, ICMP          |
| Testing           | Ping, Tracert, Nslookup                |
| Documentation     | Markdown, Git, GitHub                  |
| Evidence          | Screenshots and ticket documentation   |

---

# 🏗️ Lab Environment Setup

The Service Desk environment was deployed locally on a Windows 11 host.

### 1. Docker Environment

* Installed Docker Desktop
* Enabled the WSL 2-based Docker engine
* Installed Ubuntu 24.04 LTS under WSL 2
* Verified Docker functionality using the `hello-world` container

### 2. osTicket Deployment

* Created a dedicated project directory
* Created a Docker Compose configuration
* Deployed osTicket 1.18.4
* Deployed MariaDB 10.11
* Configured application-to-database connectivity
* Configured persistent Docker volumes
* Configured container networking
* Exposed osTicket through a local web port

### 3. Service Desk Environment

Configured a local Service Desk environment named:

**Rikit IT Service Desk**

The environment is designed to simulate a real IT support operation with technicians, users, departments, categories, priorities, and incident workflows.

### 4. Verification

The deployment was verified by:

* Confirming Docker Engine functionality
* Confirming MariaDB container operation
* Confirming osTicket container operation
* Verifying container health
* Accessing osTicket through the local web interface
* Confirming successful application/database communication

---

# 🎫 Incident Management Workflow

Every incident follows a consistent support lifecycle:

```text
User Reports Issue
        ↓
Create Ticket
        ↓
Categorize
        ↓
Determine Priority
        ↓
Gather Information
        ↓
Troubleshoot
        ↓
Identify Root Cause
        ↓
Resolve or Escalate
        ↓
Verify Resolution
        ↓
Document
        ↓
Close Ticket
```

---

# 🚦 Incident Prioritization

Priority is determined using **business impact and urgency**.

| Priority         | Example                             | Typical Action              |
| ---------------- | ----------------------------------- | --------------------------- |
| 🔴 P1 — Critical | Major service outage                | Immediate escalation        |
| 🟠 P2 — High     | Multiple users affected             | High-priority investigation |
| 🟡 P3 — Medium   | Single user unable to work normally | Standard investigation      |
| 🟢 P4 — Low      | Minor issue or inconvenience        | Normal queue                |

Factors considered include:

* Number of users affected
* Business impact
* Urgency
* Service availability
* Available workarounds

---

# 🗂️ Incident Categories

### 👤 Account & Access

* Password reset
* Account lockout
* Login failure
* MFA issue
* Permission problem

### 🖥️ Windows

* Slow computer
* Windows login issue
* Service failure
* System configuration

### 🌐 Network

* No internet access
* DNS failure
* Wi-Fi connectivity
* IP configuration
* VPN connectivity

### 💿 Software

* Application failure
* Installation problem
* Application configuration

### 🖱️ Hardware

* Keyboard/mouse issue
* Monitor problem
* Peripheral failure
* Device troubleshooting

---

# 🔎 Troubleshooting Methodology

The lab uses evidence-based troubleshooting rather than applying random fixes.

### 1. Identify

Determine exactly what the user is experiencing.

### 2. Gather Information

Collect information such as:

```text
Username
Computer name
Operating system
IP address
Error message
Application
Time of incident
Recent changes
Affected service
```

### 3. Isolate

Determine where the failure occurs.

For example:

```text
Computer
   ↓
Network Adapter
   ↓
IP Configuration
   ↓
Default Gateway
   ↓
DNS
   ↓
Internet / Service
```

### 4. Resolve

Apply a fix based on the evidence gathered.

### 5. Verify

Confirm that the original issue has been resolved.

### 6. Document

Record:

* Symptoms
* Investigation
* Evidence
* Root cause
* Resolution
* Verification
* User communication

---

# 🎫 Incident Scenarios

The lab includes realistic Service Desk scenarios:

| Ticket  | Incident                    | Category         | Priority |
| ------- | --------------------------- | ---------------- | -------- |
| INC0001 | Password Reset              | Account & Access | P3       |
| INC0002 | Account Lockout             | Account & Access | P3       |
| INC0003 | Shared Folder Access        | Permissions      | P3       |
| INC0004 | No Internet Connectivity    | Network          | P2/P3    |
| INC0005 | DNS Resolution Failure      | Network          | P3       |
| INC0006 | Windows Application Issue   | Software         | P3       |
| INC0007 | Slow Windows Computer       | Windows          | P3       |
| INC0008 | VPN Connectivity Issue      | Network          | P2/P3    |
| INC0009 | MFA / Login Issue           | Account & Access | P2/P3    |
| INC0010 | Hardware / Peripheral Issue | Hardware         | P4       |

> Priority may change depending on the simulated business impact and number of affected users.

---

# 📝 Ticket Documentation

Each incident is documented using a consistent support format.

```text
Ticket ID
Date
Category
Priority
Status

User Report
───────────
What did the user report?

Impact
──────
Who or what was affected?

Investigation
─────────────
What information was gathered?

Troubleshooting
───────────────
What tests were performed?

Root Cause
──────────
What caused the issue?

Resolution
──────────
What was done to resolve the issue?

Verification
────────────
How was the fix confirmed?

User Communication
──────────────────
How was the user informed?

Closure Notes
─────────────
Final ticket summary
```

---

# 🔧 Troubleshooting Commands

Commands are used only when relevant to the incident.

### Network Configuration

```powershell
ipconfig /all
```

### Connectivity

```powershell
ping 8.8.8.8
```

### DNS Testing

```powershell
nslookup google.com
```

### Route Testing

```powershell
tracert google.com
```

### PowerShell Connectivity

```powershell
Test-Connection google.com
```

### System Information

```powershell
Get-ComputerInfo
```

### Services

```powershell
Get-Service
```

### Windows Event Logs

```powershell
Get-WinEvent -LogName System -MaxEvents 20
```

---

# 📸 Evidence & Documentation

The project uses screenshots and technical documentation to demonstrate the work performed.

Evidence includes:

* osTicket configuration
* Ticket creation
* Ticket investigation
* Internal notes
* User communication
* Troubleshooting commands
* Technical findings
* Resolution
* Verification
* Ticket closure

Example structure:

```text
screenshots/
├── ticketing-system/
├── troubleshooting/
└── resolutions/
```

No real customer information, passwords, credentials, or confidential data are used.

---

# 🚨 Escalation

A Level 1 technician should recognize when an issue requires higher-level support.

### Network / NOC

Escalate issues such as:

* Multiple users affected
* Switch/router failure
* VLAN or routing problems
* Major connectivity outage
* Infrastructure-level DNS/DHCP problems

### Systems Administration

Escalate:

* Server failures
* Complex Active Directory issues
* Group Policy infrastructure problems
* Privileged access requirements

### Security

Escalate:

* Suspected compromised accounts
* Malware detection
* Suspicious authentication activity
* Potential security incidents

> Effective IT support is not only about fixing problems—it is also about knowing **when and where to escalate**.

---

# 📊 Service Desk Metrics

The project can track basic support metrics such as:

| Metric                | Purpose                    |
| --------------------- | -------------------------- |
| Tickets Created       | Measure workload           |
| Tickets Resolved      | Measure resolution volume  |
| Resolution Time       | Measure efficiency         |
| Escalated Tickets     | Measure escalation rate    |
| Category Distribution | Identify common issues     |
| Priority Distribution | Understand business impact |

---

# 📂 Repository Structure

```text
IT-Service-Desk-Incident-Management-Lab/
│
├── README.md
│
├── tickets/
│   ├── INC0001-password-reset.md
│   ├── INC0002-account-lockout.md
│   ├── INC0003-shared-folder-access.md
│   └── ...
│
├── screenshots/
│   ├── ticketing-system/
│   ├── troubleshooting/
│   └── resolutions/
│
└── documentation/
    ├── incident-management-process.md
    └── troubleshooting-methodology.md
```

---

# 🏆 Skills Demonstrated

**Service Desk:**
Incident management · Ticket triage · Prioritization · User communication · Ticket closure

**Troubleshooting:**
Windows · Networking · DNS · Connectivity · Account/access issues · Root-cause analysis

**Technical:**
Windows 11 · PowerShell · TCP/IP · IPv4 · DNS · DHCP · ICMP

**Tools:**
osTicket · Docker · Docker Compose · WSL · Git · GitHub

**Professional:**
Technical documentation · Evidence-based troubleshooting · Escalation · Problem solving

---

# 💼 Career Relevance

This project demonstrates practical skills relevant to:

* IT Support Technician
* Service Desk Analyst
* Help Desk Technician
* Desktop Support Technician
* Technical Support Specialist
* IT Support Specialist
* NOC Technician
* Network Support Technician

---

# 📈 Future Improvements

Planned enhancements include:

* Active Directory integration
* Microsoft 365 / Entra ID incidents
* SLA-based ticket scenarios
* Network monitoring scenarios
* PowerShell diagnostic reports
* Expanded service desk metrics
* Additional escalation workflows

---

# 🔐 Security & Lab Disclaimer

This is a **personal learning and portfolio environment**.

The lab uses simulated users, systems, incidents, and business scenarios. No real customer information or confidential company data is used.

Credentials and secrets are kept outside the public repository.

---

# 👤 About

**Rikit Thapa**

Computer Systems Networking Technician focused on entry-level **IT Support, Service Desk, Desktop Support, and NOC** opportunities.

**Certifications:** CCNA · AZ-900 · Fortinet Certified Associate in Cybersecurity

**Technical Focus:** Windows · Active Directory · Microsoft 365 · Networking · PowerShell · Troubleshooting · Service Desk

---

**Built and documented by Rikit Thapa**

*Personal homelab and simulated IT Service Desk environment created for hands-on learning and portfolio demonstration.*
