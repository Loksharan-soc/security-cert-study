# Intrusion Prevention

## Overview

Intrusion Prevention Systems (IPS) are security tools designed to detect and **actively block** malicious activities in real-time. They extend the functionality of Intrusion Detection Systems (IDS) by not just identifying but also responding to threats automatically.

---

## Key Concepts

| Term                         | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **IPS vs. IDS**             | IDS monitors and alerts; IPS monitors and takes action to block threats.   |
| **Inline Deployment**       | IPS sits directly in the traffic path, analyzing and filtering packets.    |
| **Signature-based Detection** | Matches known attack patterns; effective for known threats.                |
| **Anomaly-based Detection** | Identifies deviations from normal behavior to detect unknown threats.     |
| **Policy-based Detection**  | Applies rules defined by the organization to trigger alerts/actions.       |

---

## Intrusion Prevention Techniques

- **Packet Dropping**: Malicious traffic is blocked before reaching its destination.
- **Connection Termination**: IPS may close a suspicious session (e.g., TCP connection).
- **Rate Limiting**: Throttles traffic to mitigate denial-of-service patterns.
- **Resetting Connections**: Sends TCP resets to both ends of a connection.

---

## Types of IPS

| Type            | Description                                         |
|-----------------|-----------------------------------------------------|
| **Network-based** | Monitors traffic across the entire network.        |
| **Host-based**   | Installed on individual endpoints (e.g., servers).  |
| **Wireless**     | Protects wireless networks and devices.            |
| **Network Behavior Analysis (NBA)** | Detects anomalies in traffic patterns. |

---

## Summary

Intrusion Prevention is a proactive security layer that stops attacks in real-time. A well-tuned IPS improves an organization’s ability to respond automatically to threats while minimizing false positives and ensuring continued availability.
