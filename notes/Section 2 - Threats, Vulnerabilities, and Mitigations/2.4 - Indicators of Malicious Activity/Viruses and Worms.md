# Viruses and Worms

---

## Overview

**Viruses and worms** are two foundational types of malware. While they often achieve similar results (spreading across systems), their methods of propagation are fundamentally different.

---

## 📌 Viruses

### Definition:
A **virus** is a type of malicious code that:
- **Attaches itself** to a legitimate file or program
- **Requires user action** to activate (e.g., opening a file)
- Spreads when the infected file is shared

### Technical Behavior:
- Injects malicious code into host files (e.g., `.exe`, `.docm`)
- Often modifies registry entries for persistence
- Can corrupt or delete data, install backdoors, or disable defenses

### Types:
| Type                 | Description |
|----------------------|-------------|
| **File Infector**    | Attaches to executable files and activates when run |
| **Macro Virus**      | Targets applications with macro capabilities (like MS Word, Excel) |
| **Boot Sector Virus**| Infects the boot sector; activates during system startup |
| **Polymorphic Virus**| Changes its code slightly with each infection to evade AV detection |
| **Metamorphic Virus**| Completely rewrites its own code upon infection (harder to detect) |

---

## 🐛 Worms

### Definition:
A **worm** is a self-replicating program that:
- **Spreads without user interaction**
- Exploits vulnerabilities in network protocols or services

### Technical Behavior:
- Scans networks for vulnerable systems (e.g., open SMB ports, outdated services)
- Spreads via automated scripts or exploits
- Consumes bandwidth, disk space, and CPU

### Famous Examples:
| Worm Name | Method of Propagation | Impact |
|-----------|------------------------|--------|
| **Morris Worm** (1988) | Exploited `sendmail` and weak passwords | One of the first internet worms |
| **Blaster Worm** | RPC DCOM exploit (Windows) | System reboots and network overload |
| **Conficker** | Used SMB and brute force | Infected millions of systems globally |
| **WannaCry** | Exploited EternalBlue (SMBv1) | Combined worm with ransomware payload |

---

##  Detection and Prevention

| Measure                    | Purpose |
|----------------------------|---------|
| **Antivirus/EDR Software** | Scans files for known virus signatures |
| **Patch Management**       | Fixes vulnerabilities worms exploit |
| **Network Segmentation**   | Limits worm spread across internal networks |
| **Firewalls**              | Blocks unauthorized access to services |
| **User Training**          | Reduces virus activation via phishing or macros |

---

##  Key Differences

| Aspect              | Virus                              | Worm                               |
|---------------------|-------------------------------------|-------------------------------------|
| **User Interaction**| Required to spread                  | Not required                        |
| **Infection Method**| Attaches to files/programs          | Self-propagates via networks        |
| **Payload Delivery**| May install additional malware      | May serve as a dropper or DOS tool |
| **Speed**           | Slower (dependent on user actions)  | Rapid spread across networks        |

---

## Summary

Viruses and worms remain relevant despite modern defenses. Viruses rely on user interaction, while worms automate their spread. Both can serve as delivery mechanisms for more advanced threats (e.g., ransomware, spyware). Proper system hardening, user awareness, and up-to-date defenses are essential for containment.

---
