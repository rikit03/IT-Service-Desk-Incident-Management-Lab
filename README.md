# 🎫 IT Service Desk Incident Management Lab

### osTicket · Docker · MariaDB · Windows 11 · PowerShell

A hands-on **IT Service Desk lab** built to demonstrate practical Level 1 IT support skills using a self-hosted osTicket environment.

The project simulates a real Service Desk workflow — from receiving and categorizing incidents to troubleshooting, documenting resolutions, verifying fixes, and closing tickets.

> **Identify → Investigate → Troubleshoot → Resolve → Verify → Document**

---

## 🎯 Objectives

* Build and configure a functional Service Desk environment
* Deploy osTicket using Docker and Docker Compose
* Configure a MariaDB backend
* Manage support tickets and user requests
* Practice incident prioritization and categorization
* Document troubleshooting and resolutions
* Demonstrate escalation and professional user communication

---

## 🛠️ Lab Environment

| Component                   | Configuration                   |
| --------------------------- | ------------------------------- |
| Host OS                     | Windows 11                      |
| Ticketing System            | osTicket 1.18.4                 |
| Deployment                  | Docker Desktop / Docker Compose |
| Database                    | MariaDB 10.11                   |
| Linux Environment           | WSL 2 / Ubuntu                  |
| Scripting & Troubleshooting | PowerShell                      |
| Version Control             | Git / GitHub                    |

---

## 🏗️ Environment Setup

### Docker

Docker Desktop was installed on the Windows 11 host and configured with the WSL 2 backend.

Docker functionality was verified using the Docker `hello-world` container.

### osTicket

The Service Desk environment was deployed using Docker Compose with:

* osTicket 1.18.4
* MariaDB 10.11
* Docker networking
* Persistent storage volumes
* Application-to-database connectivity
* Local port mapping on `8080`

The deployed Service Desk is accessible through the local web interface.

### Service Desk

**Environment:** Rikit IT Service Desk

The environment provides the foundation for creating users, managing incidents, assigning priorities, documenting troubleshooting, and closing tickets.

---

# 📸 Setup Evidence

### 01 — Docker Environment

Docker installation and version verification on Windows 11.

![Docker Version](screenshots/setup/01-docker-version.png)

### 02 — Docker Verification

Docker functionality verified using the `hello-world` container.

![Docker Hello World](screenshots/setup/02-docker-hello-world.png)

### 03 — Docker Compose Configuration

Docker Compose configuration used to define the osTicket and MariaDB services.

![Docker Compose Configuration](screenshots/setup/03-docker-compose-configuration.png)

### 04 — Running Containers

The osTicket application and MariaDB database containers running successfully.

![Running Containers](screenshots/setup/04-containers-running.png)

### 05 — osTicket Service Desk

Successfully accessed the deployed osTicket Service Desk through the local web interface.

![osTicket Dashboard](screenshots/setup/05-osticket-dashboard.png)

---

# 🎫 Incident Management Workflow

Each incident follows a structured Service Desk process:

```text
User Reports Issue
        ↓
Create Ticket
        ↓
Categorize & Prioritize
        ↓
Gather Information
        ↓
Investigate
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

# 🗂️ Incident Scenarios

The lab will use realistic entry-level IT support scenarios, including:

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

Each completed ticket will document:

**User Report → Investigation → Troubleshooting → Root Cause → Resolution → Verification → Closure**

---

# 🚦 Incident Prioritization

Tickets are prioritized according to **impact and urgency**.

| Priority         | Example                        |
| ---------------- | ------------------------------ |
| 🔴 P1 — Critical | Major service outage           |
| 🟠 P2 — High     | Multiple users affected        |
| 🟡 P3 — Medium   | Single-user productivity issue |
| 🟢 P4 — Low      | Minor issue or request         |

---

# 🔎 Troubleshooting Methodology

Technical issues are approached using a structured troubleshooting process:

```text
Understand the Problem
        ↓
Gather Information
        ↓
Reproduce / Test
        ↓
Isolate the Cause
        ↓
Identify Root Cause
        ↓
Apply the Fix
        ↓
Verify the Result
        ↓
Document the Resolution
        ↓
Escalate When Required
```

---

# 💻 Troubleshooting Tools

Examples of commands used during support investigations:

```powershell
ipconfig /all
ping 8.8.8.8
nslookup google.com
tracert google.com
Test-Connection google.com
Get-Service
Get-WinEvent -LogName System -MaxEvents 20
```

These tools support investigations involving:

* Network configuration
* Connectivity
* DNS
* Routing
* Windows services
* System events

---

# 📝 Ticket Documentation

Each completed ticket will contain:

```text
Ticket ID
Category
Priority
Status

User Report
Investigation
Troubleshooting
Root Cause
Resolution
Verification
User Communication
Closure Notes
```

The goal is to demonstrate clear, professional, and repeatable Service Desk documentation.

---

# 🚨 Escalation

Incidents are escalated when they exceed the scope of first-line support.

### Network / NOC

* Multiple users affected
* Switch or router failure
* VLAN or routing issues
* Major connectivity outages

### Systems Administration

* Server failures
* Complex Active Directory issues
* Group Policy infrastructure problems
* Privileged access requirements

### Security

* Suspected compromised accounts
* Malware
* Suspicious authentication activity
* Potential security incidents

---

# 🏆 Skills Demonstrated

**Service Desk:**
Incident Management · Ticket Triage · Prioritization · User Communication · Documentation · Escalation

**Troubleshooting:**
Windows · Networking · DNS · Connectivity · Account & Access · Root-Cause Analysis

**Technical:**
PowerShell · TCP/IP · IPv4 · DNS · DHCP · ICMP

**Tools:**
osTicket · Docker · Docker Compose · WSL · Git · GitHub

---

# 📂 Repository Structure

```text
IT-Service-Desk-Incident-Management-Lab/
│
├── README.md
│
├── screenshots/
│   └── setup/
│       ├── 01-docker-version.png
│       ├── 02-docker-hello-world.png
│       ├── 03-docker-compose-configuration.png
│       ├── 04-containers-running.png
│       └── 05-osticket-dashboard.png
│
├── tickets/
│
└── documentation/
```

---

# 🔐 Security

This is a personal learning and portfolio environment.

* All users and incidents are simulated
* No customer or company data is used
* Credentials are excluded from the public repository
* Docker configuration containing passwords remains local
* Screenshots are reviewed to avoid exposing sensitive information

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

---

# 👤 About

**Rikit Thapa**

Computer Systems Networking Technician focused on entry-level **IT Support, Service Desk, Desktop Support, and NOC** opportunities.

### Certifications

CCNA · Microsoft Azure Fundamentals (AZ-900) · Fortinet Certified Associate in Cybersecurity

### Technical Focus

Windows · Active Directory · Microsoft 365 · Networking · PowerShell · Troubleshooting · Service Desk

---

# 🔗 Professional Links

* 💻 **GitHub:** [github.com/rikit03](https://github.com/rikit03)
* 🌐 **Portfolio:** [rikit03.github.io/portfolio](https://rikit03.github.io/portfolio)
* 🔗 **LinkedIn:** [linkedin.com/in/rikit-thapa-294ab028a](https://www.linkedin.com/in/rikit-thapa-294ab028a)
* 📄 **Resume:** [View Resume](https://github.com/rikit03/rikit03.github.io/blob/main/resume.pdf)
* 📧 **Email:** [rikitthapa2003@outlook.com](mailto:rikitthapa2003@outlook.com)

---

**Built and documented by Rikit Thapa**

*Personal homelab and simulated IT Service Desk environment created for hands-on learning and portfolio demonstration.*
