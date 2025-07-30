# Zero-day Vulnerabilities

---

## Overview

A **zero-day vulnerability** is a software flaw that is unknown to the software vendor or public at the time it's discovered by attackers. Because no patch or fix is available, it presents a high risk and can be exploited immediately.

---

## Key Characteristics

| Aspect                  | Description |
|-------------------------|-------------|
| **Unknown to Vendor**   | The vendor has "zero days" to fix it since they are unaware. |
| **No Available Patch**  | Makes defense difficult because typical protections may not exist. |
| **High Value to Attackers** | Often used in targeted attacks (e.g., nation-state espionage, cybercrime). |
| **Short Detection Window** | Exploits can cause damage quickly before being identified or mitigated. |

---

## How Zero-day Exploits Work

1. A researcher or attacker discovers a vulnerability.
2. The attacker creates an exploit before the vendor is aware.
3. The exploit is launched, often in targeted attacks.
4. Once disclosed, vendors work to create and distribute a patch.
5. Once patched, it becomes a known (n-day) vulnerability.

---

## Detection Challenges

- **Signature-based tools** often fail since no known signature exists yet.
- **Behavioral analysis** and **anomaly detection** are more effective.
- Threat intelligence and user behavior analytics (UBA) help detect unusual patterns.

---

## Real-World Examples

- **Stuxnet** used multiple zero-day vulnerabilities to target Iranian nuclear systems.
- **EternalBlue**, a zero-day exploit later leaked, was used in major ransomware attacks like WannaCry and NotPetya.

---

## Mitigation Strategies

| Method                        | Description |
|-------------------------------|-------------|
| **Patch Management**          | Apply patches immediately once available. |
| **Application Whitelisting**  | Prevent unauthorized apps from running. |
| **Intrusion Detection/Prevention Systems (IDS/IPS)** | Monitor for suspicious activity. |
| **Threat Intelligence Feeds** | Stay updated on emerging threats. |
| **Defense in Depth**          | Use multiple layers of security to reduce exposure. |

---

## Summary

Zero-day vulnerabilities pose a serious threat due to their stealth and potential damage. Organizations must use proactive detection strategies, stay informed, and apply layered security to minimize the impact.

---
