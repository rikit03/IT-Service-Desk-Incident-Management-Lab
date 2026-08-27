# IT Service Desk Incident Management Lab

> A hands-on Service Desk simulation demonstrating incident intake, ticket prioritization, troubleshooting, escalation, resolution, and professional technical documentation.

---

## 👤 Project Author

**Rikit Thapa**

Computer Systems Networking Technician  
CCNA | Microsoft Azure Fundamentals (AZ-900) | Fortinet Certified Associate in Cybersecurity

---

## 🎯 Project Overview

This project simulates a Level 1 IT Service Desk environment where users report common technical issues and support technicians are responsible for investigating, troubleshooting, documenting, and resolving incidents.

The lab focuses on the complete incident lifecycle:

**Report → Categorize → Prioritize → Investigate → Troubleshoot → Resolve → Verify → Document → Close**

The goal is to demonstrate practical Service Desk skills rather than simply listing technical knowledge.

> **Important:** This is a personal training lab using simulated users, incidents, and test environments. No production systems or real customer information are used.

---

# 🏢 Simulated Service Desk Environment

The lab represents a small organization's internal IT support operation.

```text
                    Employee
                       │
                       │ Reports Issue
                       ▼
              ┌──────────────────┐
              │   Service Desk    │
              │                   │
              │ Ticket Intake     │
              │ Categorization    │
              │ Prioritization    │
              └─────────┬────────┘
                        │
                        ▼
                Initial Investigation
                        │
             ┌──────────┴──────────┐
             │                     │
          Resolved              Escalate
             │                     │
             ▼                     ▼
       User Verification      Level 2 / NOC
             │
             ▼
        Documentation
             │
             ▼
        Ticket Closure
