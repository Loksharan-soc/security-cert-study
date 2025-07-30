# Malicious Updates

---

## Overview

**Malicious updates** are software updates intentionally crafted to introduce vulnerabilities, malware, or backdoors into a system. These updates can be delivered by attackers or malicious insiders, or result from compromised update mechanisms.

---

## How Malicious Updates Work

- Systems regularly check for software updates.
- If the update source or process is compromised:
  - Malicious code is installed with high privileges.
  - Backdoors or spyware may be silently activated.
- These attacks exploit **trust** in the update mechanism.

---

## Attack Vectors

| Vector                        | Description |
|-------------------------------|-------------|
| **Compromised Update Server** | Attackers inject malicious code into update packages. |
| **DNS Hijacking**             | Redirects update requests to a fake server. |
| **Man-in-the-Middle (MITM)**  | Intercepts and alters update data in transit. |
| **Signed but Malicious Updates** | Insider uses valid credentials or stolen signing keys. |

---

## Notable Examples

- **CCleaner Attack (2017)**: Legitimate software update was used to distribute malware to millions.
- **SolarWinds Orion**: Attackers inserted malicious code into signed software updates, compromising many government and enterprise systems.

---

## Prevention Techniques

- **Digital Signatures**: Ensure all updates are cryptographically signed and verified.
- **TLS Encryption**: Secure communication channels for update delivery.
- **Code Audits**: Regularly audit source code and build environments.
- **Update Validation**: Monitor for unexpected changes post-update.
- **Principle of Least Privilege**: Run update services with minimal permissions.

---

## Summary

Malicious updates compromise systems by exploiting trusted software delivery mechanisms. Secure development, distribution, and verification practices are essential to mitigate this threat.

---
