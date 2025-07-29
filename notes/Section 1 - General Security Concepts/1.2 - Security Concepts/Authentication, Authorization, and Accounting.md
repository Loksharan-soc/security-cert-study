# Authentication, Authorization, and Accounting (AAA)

---

## Overview

The AAA framework defines the processes for managing user identity and activity within a secure system:

- **Authentication** – Who are you?
- **Authorization** – What are you allowed to do?
- **Accounting** – What did you do?

---

## 1. Authentication

**Authentication** is the process of verifying the identity of a user, system, or entity.

### Common Authentication Methods

| Method Type        | Examples                          |
|--------------------|-----------------------------------|
| Something you know | Password, PIN                     |
| Something you have | Smart card, token, phone app      |
| Something you are  | Fingerprint, retina scan          |
| Somewhere you are  | IP address, GPS location          |
| Something you do   | Typing rhythm, voice recognition  |

---

## 2. Authorization

**Authorization** determines what an authenticated user is allowed to access or do.

### Common Models

| Model              | Description                              |
|--------------------|------------------------------------------|
| Role-Based Access Control (RBAC) | Access based on user roles           |
| Rule-Based Access Control        | Access granted based on policies     |
| Attribute-Based Access Control (ABAC) | Access based on attributes like department or project |

Authorization is enforced by **permissions, access control lists (ACLs)**, and **policy engines**.

---

## 3. Accounting

**Accounting** is the process of logging and tracking user activity.

### Purpose

- Audit trail for compliance and forensics
- Tracks logins, file access, system changes
- Detects anomalies or abuse

### Tools

- Log files
- SIEM systems
- Remote Authentication Dial-In User Service (RADIUS) logs

---

## Summary

| Component      | Function                                |
|----------------|------------------------------------------|
| Authentication | Verifies identity                        |
| Authorization  | Grants access based on policies          |
| Accounting     | Logs and monitors user activities        |

The AAA framework ensures systems are secure, auditable, and compliant with policy requirements.

---
