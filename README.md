# IT Service Desk & Incident Management Lab

A hands-on IT Service Desk lab designed to simulate a real-world Level 1 IT Support environment using **osTicket, Docker, WSL/Ubuntu, and MariaDB**.

This project demonstrates practical experience with ticket management, incident investigation, troubleshooting, customer communication, resolution, documentation, and ticket lifecycle management.

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

# 🎯 Project Objectives

This lab was created to demonstrate practical IT Service Desk and Level 1 IT Support skills, including:

* Incident and ticket management
* User account administration
* Microsoft 365 troubleshooting
* Windows troubleshooting
* Customer communication
* Internal documentation
* Ticket prioritization
* SLA awareness
* Incident resolution
* Ticket closure
* Technical documentation
* Git and GitHub

---

# Phase 1 — Environment Setup & osTicket Deployment

## Objective

Build and deploy a functional IT Service Desk environment using Docker, WSL/Ubuntu, MariaDB, and osTicket.

## Tasks Completed

### 1. WSL / Ubuntu Environment

Configured **WSL 2 with Ubuntu** to provide the Linux environment used for the Service Desk lab.

### 2. Docker Environment

Configured Docker to run the required containers for the Service Desk environment.

### 3. MariaDB Database

Configured MariaDB as the database backend for osTicket.

### 4. osTicket Installation

Deployed **osTicket 1.18.4** and connected it to the MariaDB database.

### 5. Initial System Verification

Verified that osTicket was successfully deployed and accessible through the web interface.

## Phase 1 Screenshots

The Phase 1 setup screenshots are stored in:

```text
screenshots/setup/
```

These screenshots document the environment setup, Docker deployment, database configuration, and working osTicket installation.

---

# Phase 2 — osTicket Administration & Configuration

## Objective

Configure osTicket to simulate a realistic corporate IT Service Desk environment.

---

## 2.1 System Configuration

Configured the basic osTicket system settings required for the Service Desk environment.

This included system identity, ticket settings, email configuration, and general help desk options.

---

## 2.2 Departments

Created departments to organize incoming IT support requests.

Example departments:

* IT Support
* System Administration

Departments allow tickets to be routed to the appropriate support team.

---

## 2.3 Help Topics

Created Help Topics to categorize common Service Desk incidents.

Examples:

* Microsoft 365 / Email
* Password Reset
* Network / VPN
* Hardware
* Software

Help Topics help agents classify and route incoming incidents efficiently.

---

## 2.4 Staff / Agents

Created Service Desk staff accounts and configured their department assignments.

This demonstrates basic IT support team administration and role-based access.

---

## 2.5 Priorities & SLA

Configured ticket priorities and Service Level Agreement expectations.

Example priorities:

* Low
* Normal
* High
* Emergency

This demonstrates how incidents can be prioritized according to urgency and business impact.

---

## 2.6 Test Users

Created test customer accounts to simulate employees submitting IT support requests.

For Ticket 01, the test customer is:

**Tony Stark**

---

## Phase 2 Screenshots

The Phase 2 configuration screenshots are stored in:

```text
screenshots/admin-config/
```

These screenshots document the configuration of departments, Help Topics, staff/agents, priorities, SLA settings, and test users.

---

# Phase 3 — Incident Management & Ticket Scenarios

## Objective

Simulate realistic Level 1 Service Desk incidents from initial ticket creation through investigation, troubleshooting, customer communication, resolution, and closure.

Each incident follows a structured Service Desk workflow:

```text
Ticket Creation
      ↓
Classification
      ↓
Prioritization
      ↓
Investigation
      ↓
Troubleshooting
      ↓
Customer Communication
      ↓
Resolution
      ↓
Ticket Closure
      ↓
Documentation
```

---

# 🎫 Ticket 01 — Microsoft 365 Login Issue

## Customer

**Tony Stark**

## Issue

Tony Stark reported that he was unable to sign in to his Microsoft 365 account.

## Category

**Microsoft 365 / Email**

## Priority

**High**

## Incident Type

**User Authentication / Account Access**

---

## Incident Summary

Tony Stark contacted the IT Service Desk after experiencing a Microsoft 365 login problem.

The Service Desk agent documented the incident, investigated the account, performed troubleshooting, communicated with the customer, documented the resolution, and closed the ticket after the issue was resolved.

---

# 🔧 Ticket 01 Troubleshooting Process

### 1. Ticket Submission

The customer submitted a Service Desk ticket reporting the Microsoft 365 login problem.

The incident was recorded in osTicket and assigned to the appropriate IT Support team.

### 2. Ticket Investigation

The support agent reviewed the ticket details and investigated the user's account and authentication issue.

### 3. Internal Troubleshooting

The agent documented troubleshooting activities using an internal note so the investigation was recorded for the IT Support team.

### 4. Customer Communication

The customer was updated regarding the troubleshooting process and asked to test Microsoft 365 access again.

### 5. Resolution

The Microsoft 365 login issue was resolved and the customer was able to access the service successfully.

### 6. Ticket Closure

After confirming the resolution with the customer, the ticket was closed and the incident lifecycle was completed.

---

# 📸 Ticket 01 Evidence

All Ticket 01 evidence is stored in:

```text
tickets/
└── ticket-01-microsoft-365-login/
```

---

## Screenshot 01 — User Creation

**File:** `Phase3_Ticket01_User_Creation.png`

Shows the creation of **Tony Stark** as the test customer used for the Microsoft 365 incident scenario.

![Ticket 01 - User Creation](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_User_Creation.png)

---

## Screenshot 02 — Ticket Created

**File:** `Phase3_Ticket01_Created.png`

Shows the Microsoft 365 login issue being submitted as a new Service Desk ticket for Tony Stark.

![Ticket 01 - Created](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Created.png)

---

## Screenshot 03 — Internal Troubleshooting

**File:** `Phase3_Ticket01_Internal_Note.png`

Shows the IT Support agent documenting internal troubleshooting activities and investigation steps.

![Ticket 01 - Internal Troubleshooting](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Internal_Note.png)

---

## Screenshot 04 — Customer Communication

**File:** `Phase3_Ticket01_Customer_Reply.png`

Shows communication with Tony Stark during the troubleshooting process and keeps the customer informed about the incident.

![Ticket 01 - Customer Communication](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Customer_Reply.png)

---

## Screenshot 05 — Resolution

**File:** `Phase3_Ticket01_Resolution.png`

Shows the documented resolution of the Microsoft 365 login issue after troubleshooting was completed.

![Ticket 01 - Resolution](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Resolution.png)

---

## Screenshot 06 — Ticket Closed

**File:** `Phase3_Ticket01_Closed.png`

Shows the completed ticket after the resolution was confirmed and the incident was formally closed.

![Ticket 01 - Ticket Closed](tickets/ticket-01-microsoft-365-login/Phase3_Ticket01_Closed.png)

---

# 📂 Project Structure

```text
IT-Service-Desk-Incident-Management-Lab/
│
├── README.md
├── .gitignore
│
├── screenshots/
│   │
│   ├── setup/
│   │
│   └── admin-config/
│
└── tickets/
    │
    └── ticket-01-microsoft-365-login/
        │
        ├── Phase3_Ticket01_User_Creation.png
        ├── Phase3_Ticket01_Created.png
        ├── Phase3_Ticket01_Internal_Note.png
        ├── Phase3_Ticket01_Customer_Reply.png
        ├── Phase3_Ticket01_Resolution.png
        └── Phase3_Ticket01_Closed.png
```

---

# 🧰 Skills Demonstrated

## Service Desk

* Incident Management
* Ticket Lifecycle Management
* Ticket Classification
* Ticket Prioritization
* SLA Awareness
* Customer Communication
* Internal Documentation
* Incident Resolution
* Ticket Closure

## Technical Support

* Microsoft 365 troubleshooting
* User account troubleshooting
* Authentication troubleshooting
* Windows troubleshooting
* Basic networking troubleshooting
* VPN troubleshooting
* Password and account support

## IT Administration

* osTicket administration
* Department management
* Staff/agent management
* Help Topic configuration
* Priority configuration
* SLA configuration
* Test user creation

## Tools & Technologies

* osTicket
* Docker
* Docker Compose
* WSL 2
* Ubuntu
* MariaDB
* PowerShell
* Git
* GitHub

---

# 🔄 Real-World Service Desk Workflow

This project demonstrates the workflow commonly used by Level 1 IT Support and Service Desk teams:

1. Receive user incident
2. Create and document ticket
3. Identify affected service
4. Categorize the incident
5. Assign priority
6. Investigate the issue
7. Perform troubleshooting
8. Document internal actions
9. Communicate with the user
10. Apply or recommend a resolution
11. Confirm the issue is resolved
12. Close and document the ticket

---

# 🚀 Future Ticket Scenarios

Additional realistic Service Desk incidents will be added to Phase 3.

Planned scenarios include:

* Password reset
* VPN connectivity issue
* Windows workstation issue
* Software installation problem
* Network connectivity issue
* Printer troubleshooting

Each ticket will follow the same structured incident management lifecycle and include supporting screenshots and documentation.

---

# 📊 Project Status

| Phase                            | Status      |
| -------------------------------- | ----------- |
| Phase 1 — Environment Setup      | ✅ Completed |
| Phase 2 — osTicket Configuration | ✅ Completed |
| Phase 3 — Ticket 01              | ✅ Completed |
| Phase 3 — Additional Tickets     | 🔄 Planned  |

---

# 🎯 Project Purpose

This project was created as a practical IT Service Desk portfolio project to demonstrate hands-on experience with:

* Incident management
* Technical troubleshooting
* Customer support
* Ticket documentation
* User administration
* IT Service Desk operations
* Problem resolution
* Ticket lifecycle management

The project is designed to reflect the responsibilities and workflow of a **Level 1 Service Desk Analyst / IT Support Technician** in a real-world environment.
