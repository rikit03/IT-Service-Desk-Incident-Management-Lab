# IT Service Desk & Incident Management Lab

A hands-on IT Service Desk lab built to simulate a real-world Level 1 IT Support environment using **osTicket, Docker, WSL/Ubuntu, and MariaDB**.

The project demonstrates practical experience with ticket creation, incident investigation, troubleshooting, customer communication, resolution, documentation, and ticket lifecycle management.

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
| Ticket Management | osTicket                |
| Version Control   | Git / GitHub            |

---

# 📌 Project Objectives

This lab was created to demonstrate practical IT Support and Service Desk skills, including:

* Incident and ticket management
* User account administration
* Microsoft 365 troubleshooting
* Windows and application troubleshooting
* Customer communication
* Internal documentation
* Ticket prioritization
* SLA awareness
* Incident resolution
* Ticket closure and lifecycle management
* Technical documentation
* Git and GitHub project management

---

# Phase 1 — Environment Setup & osTicket Deployment

## Objective

Set up a functional IT Service Desk environment using Docker, WSL/Ubuntu, MariaDB, and osTicket.

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

Verified that osTicket was accessible and functioning correctly through the web interface.

## Phase 1 Screenshots

Screenshots for the environment setup are located in:

```text
screenshots/setup/
```

These screenshots document the setup and deployment process, including the working osTicket environment.

---

# Phase 2 — osTicket Administration & Configuration

## Objective

Configure osTicket to simulate a realistic corporate IT Service Desk.

---

## 2.1 System Configuration

Configured the basic osTicket system settings required for the Service Desk environment.

This included system identity, ticket settings, email configuration, and general help desk options.

---

## 2.2 Departments

Created departments to organize incoming IT support requests.

Example:

* IT Support
* System Administration

This demonstrates how tickets can be routed to the appropriate support team.

---

## 2.3 Help Topics

Created help topics to categorize common Service Desk incidents.

Examples:

* Microsoft 365 / Email
* Password Reset
* Network / VPN
* Hardware
* Software

Help Topics allow agents to quickly categorize and route incoming incidents.

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

This demonstrates how Service Desk teams can prioritize incidents based on business impact and urgency.

---

## 2.6 Test Users

Created test customer accounts to simulate real employees submitting IT support requests.

For Ticket 01, the customer/test user is:

**Tony Stark**

---

## Phase 2 Screenshots

Screenshots for osTicket administration and configuration are located in:

```text
screenshots/admin-config/
```

They document the configuration of departments, staff, help topics, priorities, SLA settings, and test users.

---

# Phase 3 — Incident Management & Ticket Scenarios

## Objective

Simulate realistic Level 1 Service Desk incidents from ticket creation through troubleshooting, customer communication, resolution, and closure.

Each ticket follows a structured incident management workflow:

```text
Ticket Creation
      ↓
Incident Classification
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

Microsoft 365 / Email

## Priority

High

## Incident Type

User Authentication / Account Access

---

## Troubleshooting Process

### 1. Ticket Submission

The customer submitted a Service Desk ticket reporting an inability to access Microsoft 365.

The incident was recorded in osTicket and assigned to the appropriate IT Support team.

### 2. Ticket Investigation

The support agent reviewed the ticket details and investigated the user's account and authentication issue.

### 3. Internal Troubleshooting

Internal notes were added to document troubleshooting steps without exposing technical information to the customer.

### 4. Customer Communication

The customer was updated regarding the troubleshooting process and requested to test the Microsoft 365 login again.

### 5. Resolution

The login issue was resolved and the customer was able to access Microsoft 365 successfully.

### 6. Ticket Closure

After confirming the resolution, the ticket was closed and the incident lifecycle was completed.

---

# 📸 Ticket 01 Evidence

All Ticket 01 screenshots are stored in:

```text
tickets/
└── ticket-01-microsoft-365-login/
```

---

## Screenshot 01 — User Creation

**File:** `Phase3_Ticket01_User_Creation.png`

Shows the creation/configuration of **Tony Stark** as the test customer used for the incident scenario.

---

## Screenshot 02 — Ticket Created

**File:** `Phase3_Ticket01_Created.png`

Shows Tony Stark's Microsoft 365 login issue being submitted as a new Service Desk ticket.

---

## Screenshot 03 — Internal Note

**File:** `Phase3_Ticket01_Internal_Note.png`

Shows the IT Support agent documenting internal troubleshooting activities and investigation steps.

---

## Screenshot 04 — Customer Reply

**File:** `Phase3_Ticket01_Customer_Reply.png`

Shows communication with Tony Stark after troubleshooting, keeping the customer informed about the incident.

---

## Screenshot 05 — Resolution

**File:** `Phase3_Ticket01_Resolution.png`

Shows the documented resolution of the Microsoft 365 login problem and confirmation that the issue was addressed.

---

## Screenshot 06 — Ticket Closed

**File:** `Phase3_Ticket01_Closed.png`

Shows the completed ticket after the resolution was confirmed and the incident was formally closed.

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

# 🎯 Real-World Service Desk Workflow

This project demonstrates the type of workflow commonly used by Level 1 IT Support and Service Desk teams:

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

Additional realistic Service Desk incidents will be added to Phase 3, including scenarios such as:

* Password reset
* VPN connectivity issue
* Windows workstation issue
* Software installation problem
* Network connectivity issue
* Printer troubleshooting

Each scenario will follow the same structured incident management lifecycle and include supporting screenshots and documentation.

---

# 📌 Project Status

| Phase                            | Status      |
| -------------------------------- | ----------- |
| Phase 1 — Environment Setup      | ✅ Completed |
| Phase 2 — osTicket Configuration | ✅ Completed |
| Phase 3 — Ticket 01              | ✅ Completed |
| Phase 3 — Additional Tickets     | 🔄 Planned  |

---

# 👨‍💻 Project Purpose

This project was created as a practical IT Service Desk portfolio project to demonstrate hands-on experience with **incident management, troubleshooting, customer support, ticket documentation, and IT support administration**.

It is designed to reflect the workflow and responsibilities of a **Level 1 Service Desk / IT Support Technician** in a real-world environment.
