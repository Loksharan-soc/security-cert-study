# Indicators of Compromise (IOCs)

---

Indicators of Compromise (IOCs) are pieces of forensic data that identify potential malicious activity on a system or network. They help cybersecurity professionals detect, respond to, and mitigate security breaches.

---

## What Are IOCs?

IOCs are evidence left behind by attackers. They are used to:

- Detect intrusions
- Identify the type of attack
- Understand the attack’s origin and impact
- Respond effectively to incidents

---

## Common Types of IOCs

| IOC Type                    | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **File Hashes**             | Unique identifiers (e.g., MD5, SHA256) of malicious files.                 |
| **IP Addresses**            | Known malicious or suspicious IPs involved in the attack.                  |
| **Domain Names / URLs**     | Malicious sites used for command-and-control or phishing.                  |
| **Email Addresses**         | Sender addresses from phishing or spam emails.                             |
| **Registry Changes**        | Unexpected modifications to system registry keys.                         |
| **File Names / Paths**      | Suspicious or unusual files placed by malware.                            |
| **Processes / Services**    | Unexpected running processes or services.                                 |
| **Network Traffic Patterns**| Unusual outbound/inbound traffic patterns or protocols.                   |
| **Log Entries**             | Authentication failures, privilege escalations, and other suspicious logs.|

---

## Sources of IOC Data

| Source                     | Purpose                                                                 |
|----------------------------|-------------------------------------------------------------------------|
| **Antivirus Tools**        | Detect malware signatures.                                              |
| **Endpoint Detection and Response (EDR)** | Monitors system activity for threats.                  |
| **SIEM Systems**           | Aggregates and analyzes logs from multiple sources.                     |
| **Threat Intelligence Feeds** | Provides real-time data on known threats.                         |
| **Firewall / IDS / IPS Logs** | Monitors and logs suspicious network activity.                     |

---

## IOC Use Cases

1. **Threat Hunting** – Proactively searching for signs of compromise.
2. **Incident Response** – Investigating and containing breaches.
3. **Forensics** – Understanding how an attack happened and what was affected.
4. **Alert Tuning** – Fine-tuning detection systems to avoid false positives and negatives.

---

## IOC vs IOA

| Indicator of Compromise (IOC) | Indicator of Attack (IOA)               |
|-------------------------------|-----------------------------------------|
| Evidence that an attack occurred | Evidence that an attack is in progress |
| Reactive                      | Proactive                                |
| Based on known threats        | Focuses on behaviors and tactics        |

---

## Limitations

- **Can be outdated** — IOCs tied to past attacks may not help detect new ones.
- **Evasion** — Skilled attackers can obfuscate IOCs.
- **False Positives** — Not all suspicious indicators mean a real threat.

---

## Best Practices

- Regularly update IOC databases
- Correlate multiple IOCs before concluding a breach
- Use automated tools for real-time monitoring and response
- Combine IOCs with IOAs for deeper insights

---

## Summary

- IOCs help detect and investigate cyber incidents.
- They include technical artifacts such as IPs, hashes, domains, and log entries.
- Effective use of IOCs improves detection, response, and security posture.

---
