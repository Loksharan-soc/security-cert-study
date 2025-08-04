# Other Infrastructure Concepts

---

This section covers advanced and supporting infrastructure elements essential to a secure and efficient IT environment.

---

## Load Balancers

- Distribute incoming network traffic across multiple servers.
- Ensure **availability**, **scalability**, and **fault tolerance**.
- Types:
  - **Layer 4 (Transport Layer)**: Balances based on IP and TCP/UDP.
  - **Layer 7 (Application Layer)**: Balances based on HTTP/HTTPS, content-aware.

---

## Proxies

| Type         | Description                                                |
|--------------|------------------------------------------------------------|
| **Forward Proxy** | Sits between client and internet. Controls and monitors outbound traffic. |
| **Reverse Proxy** | Sits in front of servers. Handles incoming requests on behalf of servers.  |
| **Transparent Proxy** | Intercepts traffic without requiring configuration on client devices. |

**Benefits:**
- Anonymity
- Content filtering
- Caching for performance
- Traffic control and logging

---

## Jump Servers (Jump Boxes)

- Special-purpose systems used to **access and manage devices** in separate security zones.
- Enforce **access control** and **auditing**.
- Common in segmented networks (e.g., production vs dev environments).

---

## DNS and DHCP Infrastructure

| Protocol | Purpose |
|---------|---------|
| **DNS (Domain Name System)** | Translates domain names into IP addresses. |
| **DHCP (Dynamic Host Configuration Protocol)** | Assigns IP addresses dynamically to devices. |

**Security Measures:**
- Use secure DNS (DNSSEC)
- DHCP snooping to prevent rogue servers

---

## NTP (Network Time Protocol)

- Ensures all systems have **synchronized time**.
- Critical for logging, authentication, and certificate validation.
- Use trusted NTP servers (internal or secure external).

---

## Directory Services

- Centralized user and device management.
- Examples: **Active Directory (AD)**, **LDAP**
- Provide:
  - Authentication & Authorization
  - Group policy enforcement
  - Role-based access control

---

## Remote Access Services

- Allow secure connections to internal networks and services.
- Methods:
  - **VPN**
  - **Remote Desktop Protocol (RDP)**
  - **Secure Shell (SSH)**
- Always implement multi-factor authentication (MFA) and monitoring.

---

## Bastion Hosts

- A hardened system designed to withstand attacks.
- Exposed to the public internet but tightly controlled.
- Often used as gateways for administrative access.

---

## Summary

- Supporting infrastructure includes components like proxies, DNS/DHCP, time servers, and jump servers.
- These services must be **secured**, **monitored**, and **properly configured** to protect the network environment.
- They enable secure, efficient communication, access control, and resource distribution across the organization.

---
