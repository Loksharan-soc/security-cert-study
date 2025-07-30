# Operating System Vulnerabilities

---

## Overview

Operating system (OS) vulnerabilities are weaknesses or flaws in the core system software that attackers can exploit to gain unauthorized access, execute malicious code, or disrupt operations.

---

## Common OS Vulnerabilities

| Vulnerability                  | Description |
|-------------------------------|-------------|
| **Privilege Escalation**       | Exploiting bugs to gain elevated permissions (e.g., from user to admin). |
| **Unpatched Systems**          | Systems missing security updates are vulnerable to known exploits. |
| **Insecure Default Configurations** | Factory settings that are too permissive (e.g., open ports, default credentials). |
| **Weak File Permissions**      | Improper access controls on sensitive files or directories. |
| **Buffer Overflows**           | Overwriting memory to execute arbitrary code. |
| **Race Conditions**            | Exploiting timing issues to manipulate operations. |

---

## Attack Methods

- Exploiting known vulnerabilities with **public exploits**.
- Deploying **rootkits** to hide presence and maintain control.
- Using **malicious scripts** to automate privilege escalation.
- Dropping **persistence mechanisms** to survive reboots.

---

## Examples

- **EternalBlue** exploit (used by WannaCry ransomware) targeted unpatched versions of Windows.
- Linux privilege escalation bugs in kernel modules.

---

## Mitigation Strategies

- **Regular Patching**: Keep the OS and kernel up to date.
- **Configuration Hardening**: Disable unused services, enforce strong permissions.
- **Use of Security Tools**:
  - Host-based firewalls
  - Antivirus/anti-malware
  - Integrity checkers
- **Access Controls**: Implement least privilege and user separation.
- **Security Audits**: Regularly scan for vulnerabilities.

---

## Summary

Operating system vulnerabilities are prime targets for attackers. Strong patch management, secure configurations, and proactive monitoring are essential to minimize exposure.

---
