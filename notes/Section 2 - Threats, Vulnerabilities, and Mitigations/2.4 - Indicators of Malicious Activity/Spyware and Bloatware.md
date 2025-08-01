# Spyware and Bloatware

---

## 🕵️ Spyware

### Definition:
**Spyware** is malicious software designed to secretly monitor a user’s activities and collect sensitive information without their knowledge or consent.

### Technical Behavior:
- Runs stealthily in the background
- Captures keystrokes (keyloggers)
- Monitors browsing behavior and website history
- Exfiltrates credentials, credit card numbers, or corporate data
- Often bundled with free software or installed through phishing/malicious ads

### Common Types:
| Type           | Description |
|----------------|-------------|
| **Keyloggers** | Record every keystroke typed on a device |
| **Screen Scrapers** | Capture screenshots at intervals or on certain actions |
| **Credential Harvesters** | Extract saved passwords or intercept login credentials |
| **Adware (with spyware)** | Delivers ads and secretly monitors user behavior |

---

## 🧱 Countermeasures

| Measure                      | Description |
|------------------------------|-------------|
| **Antispyware Tools**        | Specialized software to detect and remove spyware |
| **Browser Protections**      | Extensions or settings to block trackers/scripts |
| **Least Privilege Principle**| Limits spyware impact if installed |
| **Application Whitelisting** | Prevents unauthorized software execution |
| **Regular Auditing**         | Detects unauthorized processes or services |

---

## 🪀 Bloatware

### Definition:
**Bloatware** refers to unnecessary or unwanted software pre-installed by manufacturers or carriers. It is not necessarily malicious but can reduce performance or create vulnerabilities.

### Characteristics:
- Occupies disk space and memory
- May run at startup and slow down the system
- Can include trialware, vendor utilities, or redundant apps
- Often difficult to remove through standard uninstall methods

### Risks:
- Increases attack surface if not updated
- May include privacy-invasive components
- Can mask other malware (in shady OEM builds)

---

## 🧽 Mitigation of Bloatware

| Action                     | Description |
|----------------------------|-------------|
| **Fresh OS Installation**  | Clean installs without vendor add-ons |
| **PowerShell Scripts**     | Remove built-in Windows apps (e.g., `Get-AppxPackage`) |
| **Group Policy Settings**  | Prevent reinstallation after updates |
| **Endpoint Management Tools** | Remove or prevent bloatware in enterprise deployments |

---

## Summary

While **spyware** is malicious and targets user privacy, **bloatware** is typically unwanted and reduces usability or performance. Both should be removed or mitigated to maintain a secure and efficient environment.

---
