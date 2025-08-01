# Segmentation and Access Control

---

Segmentation and access control are critical components of network security, helping to reduce the attack surface, limit lateral movement, and ensure that users and systems only access what they’re authorized to.

---

## Network Segmentation

**Definition**: Dividing a network into smaller subnetworks (segments) to improve performance and security.

### Benefits:
- **Limits attack scope**: Compromise in one segment doesn't give access to the whole network.
- **Improves traffic management**: Reduces congestion and increases visibility.
- **Enhances containment**: Threats or malware are isolated to a single segment.

### Types of Segmentation:

| Type                  | Description                                         |
|-----------------------|-----------------------------------------------------|
| **Physical**          | Uses separate hardware (e.g., different switches). |
| **Logical (VLANs)**   | Uses virtual LANs to segment traffic logically.     |
| **Software-defined**  | Implemented via policies in SDN environments.       |
| **Microsegmentation** | Fine-grained segmentation at workload/application level. |

---

## Access Control

**Definition**: Restricting access to systems, data, or network resources based on policies.

### Access Control Models:

| Model                   | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| **MAC (Mandatory)**     | Access based on classification levels (e.g., top secret).                   |
| **DAC (Discretionary)** | Owners decide who has access to their resources.                            |
| **RBAC (Role-Based)**   | Access based on user roles within an organization.                          |
| **ABAC (Attribute-Based)** | Access based on attributes like department, time of day, location.     |

---

## Principles of Access Control

- **Least Privilege**: Users get the minimum access necessary for their job.
- **Need to Know**: Access only to information required to perform tasks.
- **Separation of Duties**: No single user has control over all aspects of a process.
- **Implicit Deny**: Access is denied unless explicitly granted.

---

## Access Control Techniques

| Technique            | Description                                                  |
|----------------------|--------------------------------------------------------------|
| **ACLs (Access Control Lists)** | Rules applied to network devices to filter traffic.         |
| **Firewalls**         | Enforce policies on inbound/outbound traffic.               |
| **Authentication Systems** | Verify identity before granting access.               |
| **Multifactor Authentication (MFA)** | Adds layers to authentication.               |
| **Single Sign-On (SSO)** | Allows access to multiple resources with one login.       |

---

## Combining Segmentation and Access Control

- **Network ACLs on Segments**: Block unauthorized traffic between zones.
- **User Roles in Segments**: Control what each user can access within a segment.
- **Segmentation + MFA**: Limits access even if credentials are stolen.
- **Microsegmentation + Identity**: Enforces access at the user/workload level.

---

## Summary

- Segmentation isolates network components to limit breaches.
- Access control ensures only authorized users can access sensitive resources.
- Together, they create layered, defense-in-depth protection.

---
