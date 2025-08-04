# States of Data

## Overview

Data exists in different states throughout its lifecycle, and each state requires specific security controls to protect confidentiality, integrity, and availability.

---

## Three Primary States of Data

| State              | Description                                  | Security Considerations                         |
|--------------------|----------------------------------------------|------------------------------------------------|
| **Data at Rest**    | Data stored on physical media or storage devices. | Encryption, access controls, backups, physical security. |
| **Data in Transit** | Data moving across networks or between devices.    | Encryption (e.g., TLS, VPN), integrity checks, secure protocols. |
| **Data in Use**     | Data actively being processed or accessed by applications or users. | Endpoint security, memory protection, access control. |

---

## Data Lifecycle and Security

- Data moves between these states frequently.
- Security controls must adapt as data transitions.
- Weaknesses in any state can lead to compromise.

---

## Protection Techniques per State

| State           | Protection Methods                                           |
|-----------------|--------------------------------------------------------------|
| Data at Rest    | Full disk encryption (FDE), database encryption, physical locks. |
| Data in Transit | TLS/SSL, VPNs, SSH, secure APIs.                             |
| Data in Use     | Anti-malware, application whitelisting, data masking, secure coding practices. |

---

## Summary

Protecting data requires understanding its state and applying appropriate security controls tailored to each. Failure to secure any state can expose data to breaches or loss.
