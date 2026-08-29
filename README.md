\# 🎫 IT Service Desk Incident Management Lab



\### osTicket · Docker · Windows 11 · MariaDB · PowerShell



A hands-on \*\*IT Service Desk lab\*\* built to demonstrate practical Level 1 IT Support skills through a locally deployed osTicket environment.



The lab focuses on \*\*incident management, technical troubleshooting, user communication, documentation, and structured problem resolution\*\*.



> \*\*Identify → Investigate → Troubleshoot → Resolve → Verify → Document\*\*



\---



\## 🎯 Project Overview



This project simulates a small-business IT Service Desk where users report technical issues and a support technician manages incidents from \*\*ticket creation through resolution and closure\*\*.



The lab environment is designed around realistic IT support scenarios involving:



\* Account and access issues

\* Windows troubleshooting

\* Network connectivity

\* DNS and VPN problems

\* Software issues

\* Hardware and peripheral problems

\* User onboarding and access requests



\---



\## 🛠️ Technologies \& Tools



| Area             | Technology                      |

| ---------------- | ------------------------------- |

| Ticketing System | osTicket 1.18.4                 |

| Deployment       | Docker Desktop / Docker Compose |

| Database         | MariaDB 10.11                   |

| Host OS          | Windows 11                      |

| Linux Backend    | WSL 2 / Ubuntu                  |

| Troubleshooting  | PowerShell / Command Prompt     |

| Networking       | TCP/IP, IPv4, DNS, DHCP, ICMP   |

| Documentation    | Markdown / Git                  |

| Version Control  | Git / GitHub                    |



\---



\# 🏗️ Lab Environment Setup



The Service Desk environment was deployed locally on a Windows 11 host using Docker Desktop.



\### 1. Docker Environment



\* Installed Docker Desktop

\* Configured the WSL 2-based Docker engine

\* Installed Ubuntu under WSL 2

\* Verified Docker functionality using the `hello-world` container



\### 2. osTicket Deployment



\* Created a dedicated project directory

\* Created a Docker Compose configuration

\* Deployed osTicket 1.18.4

\* Deployed MariaDB 10.11

\* Configured application-to-database connectivity

\* Configured persistent Docker volumes

\* Configured container networking

\* Exposed osTicket through port `8080`



\### 3. Service Desk Environment



Configured a local Service Desk environment named:



\*\*Rikit IT Service Desk\*\*



The environment provides the foundation for managing users, incidents, priorities, categories, troubleshooting, escalation, and ticket closure.



\### 4. Verification



The deployment was verified by:



\* Testing Docker functionality

\* Validating the Docker Compose configuration

\* Confirming MariaDB was running

\* Confirming osTicket was running

\* Verifying container health

\* Accessing the osTicket web interface



\---



\# 📸 Lab Setup Evidence



\### Docker Environment



Docker Desktop was installed and verified on the Windows 11 host.



!\[Docker Version](screenshots/setup/01-docker-version.png)



\### Docker Verification



Docker functionality was verified using the `hello-world` container.



!\[Docker Hello World](screenshots/setup/02-docker-hello-world.png)



\### Docker Compose Configuration



The osTicket application and MariaDB database were configured using Docker Compose.



!\[Docker Compose Configuration](screenshots/setup/03-docker-compose-configuration.png)



\### Running Containers



The osTicket application and MariaDB database containers were successfully deployed and running.



!\[Running Containers](screenshots/setup/04-containers-running.png)



\### osTicket Service Desk



The deployed osTicket Service Desk was successfully accessed through the local web interface.



!\[osTicket Dashboard](screenshots/setup/05-osticket-dashboard.png)



\---



\# 🎫 Incident Management Workflow



Each support incident follows a structured Service Desk lifecycle:



```text

User Reports Issue

&#x20;       ↓

Create Ticket

&#x20;       ↓

Categorize

&#x20;       ↓

Determine Priority

&#x20;       ↓

Gather Information

&#x20;       ↓

Troubleshoot

&#x20;       ↓

Identify Root Cause

&#x20;       ↓

Resolve or Escalate

&#x20;       ↓

Verify Resolution

&#x20;       ↓

Document

&#x20;       ↓

Close Ticket

```



\---



\# 🚦 Incident Prioritization



Incidents are prioritized based on \*\*impact and urgency\*\*.



| Priority         | Example                        |

| ---------------- | ------------------------------ |

| 🔴 P1 — Critical | Major service outage           |

| 🟠 P2 — High     | Multiple users affected        |

| 🟡 P3 — Medium   | Single-user productivity issue |

| 🟢 P4 — Low      | Minor issue or request         |



\---



\# 🗂️ Planned Incident Scenarios



The lab will include realistic Service Desk incidents such as:



| Incident                    | Category         |

| --------------------------- | ---------------- |

| Password Reset              | Account \& Access |

| Account Lockout             | Account \& Access |

| Shared Folder Access        | Permissions      |

| No Internet Connectivity    | Network          |

| DNS Resolution Failure      | Network          |

| VPN Connectivity Issue      | Network          |

| Slow Windows Computer       | Windows          |

| Application Failure         | Software         |

| MFA / Login Issue           | Account \& Access |

| Hardware / Peripheral Issue | Hardware         |



Each completed incident will include:



\*\*User Report → Investigation → Troubleshooting → Root Cause → Resolution → Verification → Closure\*\*



\---



\# 🔎 Troubleshooting Approach



I use an evidence-based troubleshooting methodology rather than applying random fixes.



```text

Understand the Problem

&#x20;       ↓

Gather Information

&#x20;       ↓

Reproduce / Test

&#x20;       ↓

Isolate the Cause

&#x20;       ↓

Identify Root Cause

&#x20;       ↓

Apply the Fix

&#x20;       ↓

Verify the Result

&#x20;       ↓

Document the Solution

&#x20;       ↓

Escalate When Required

```



\---



\# 💻 Example Troubleshooting Tools



\### Network Configuration



```powershell

ipconfig /all

```



\### Connectivity Testing



```powershell

ping 8.8.8.8

```



\### DNS Testing



```powershell

nslookup google.com

```



\### Route Testing



```powershell

tracert google.com

```



\### PowerShell Connectivity



```powershell

Test-Connection google.com

```



\### Windows Services



```powershell

Get-Service

```



\### System Events



```powershell

Get-WinEvent -LogName System -MaxEvents 20

```



\---



\# 📝 Ticket Documentation



Each completed incident will be documented using a consistent format:



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



This demonstrates the ability to maintain clear and professional technical documentation.



\---



\# 🚨 Escalation



A Service Desk technician should recognize when an incident requires higher-level support.



\### Network / NOC



\* Multiple users affected

\* Switch or router failure

\* VLAN or routing problems

\* Major connectivity outage



\### Systems Administration



\* Server failure

\* Complex Active Directory issues

\* Group Policy infrastructure problems

\* Privileged access requirements



\### Security



\* Suspected compromised accounts

\* Malware

\* Suspicious authentication activity

\* Potential security incidents



> Effective IT support is not only about fixing problems—it is also about knowing \*\*when and where to escalate\*\*.



\---



\# 🏆 Skills Demonstrated



\### Service Desk



Incident management · Ticket triage · Prioritization · User communication · Documentation · Escalation



\### Troubleshooting



Windows · Networking · DNS · Connectivity · Account \& access · Root-cause analysis



\### Technical



Windows 11 · PowerShell · TCP/IP · IPv4 · DNS · DHCP · ICMP



\### Tools



osTicket · Docker · Docker Compose · WSL · Git · GitHub



\---



\# 📂 Repository Structure



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



\---



\# 🔐 Security \& Lab Disclaimer



This is a \*\*personal learning and portfolio environment\*\*.



The lab uses simulated users, systems, incidents, and business scenarios. No real customer information or confidential company data is used.



Credentials, passwords, secret keys, and other sensitive configuration values are \*\*not included in the public repository\*\*.



\---



\# 💼 Career Relevance



This project demonstrates practical skills relevant to:



\* IT Support Technician

\* Service Desk Analyst

\* Help Desk Technician

\* Desktop Support Technician

\* Technical Support Specialist

\* IT Support Specialist

\* NOC Technician

\* Network Support Technician



\---



\# 👤 About



\*\*Rikit Thapa\*\*



Computer Systems Networking Technician focused on entry-level \*\*IT Support, Service Desk, Desktop Support, and NOC\*\* opportunities.



\*\*Certifications:\*\* CCNA · Microsoft Azure Fundamentals (AZ-900) · Fortinet Certified Associate in Cybersecurity



\*\*Technical Focus:\*\* Windows · Active Directory · Microsoft 365 · Networking · PowerShell · Troubleshooting · Service Desk



\---



\## 🔗 Professional Links



\* 💻 \*\*GitHub:\*\* \[github.com/rikit03](https://github.com/rikit03)

\* 🌐 \*\*Portfolio:\*\* \[rikit03.github.io/portfolio](https://rikit03.github.io/portfolio)

\* 🔗 \*\*LinkedIn:\*\* \[linkedin.com/in/rikit-thapa-294ab028a](https://www.linkedin.com/in/rikit-thapa-294ab028a)

\* 📄 \*\*Resume:\*\* \[View Resume](https://github.com/rikit03/rikit03.github.io/blob/main/resume.pdf)

\* 📧 \*\*Email:\*\* \[rikitthapa2003@outlook.com](mailto:rikitthapa2003@outlook.com)



\---



\*\*Built and documented by Rikit Thapa\*\*



\*Personal homelab and simulated IT Service Desk environment created for hands-on learning and portfolio demonstration.\*



