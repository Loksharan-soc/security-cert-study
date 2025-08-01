# On-Path Attacks

---

**On-Path Attacks**, formerly known as **Man-in-the-Middle (MitM)** attacks, occur when an attacker intercepts or alters communication between two parties without their knowledge.

---

## How On-Path Attacks Work

| Step              | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Interception**  | Attacker places themselves between two communicating parties.               |
| **Eavesdropping** | Attacker silently monitors communication, collecting sensitive information. |
| **Modification**  | Attacker alters the contents of the messages being transmitted.             |

---

## Common On-Path Techniques

| Method                        | Description                                                                 |
|-------------------------------|-----------------------------------------------------------------------------|
| **ARP Spoofing**              | Attacker sends fake ARP responses to associate their MAC with another IP.   |
| **DNS Spoofing**              | Redirects user requests to malicious sites by altering DNS responses.       |
| **HTTPS Spoofing**            | Tricks users into thinking they are on a secure site (fake certs, etc).     |
| **Wi-Fi Evil Twin**           | Attacker mimics a legitimate wireless network to intercept traffic.         |
| **Session Hijacking**         | Takes control of an active session using stolen session tokens or cookies.  |
| **SSL Stripping**             | Downgrades HTTPS to HTTP to intercept unencrypted communication.            |

---

## Tools Commonly Used

| Tool             | Purpose                                            |
|------------------|----------------------------------------------------|
| **Ettercap**     | ARP spoofing, DNS spoofing, packet manipulation    |
| **Bettercap**    | Advanced MitM framework supporting many techniques |
| **Wireshark**    | Packet analysis and inspection                     |

---

## Impact of On-Path Attacks

- Theft of login credentials and session cookies
- Redirection to malicious websites
- Injection of malicious content
- Bypass of encryption if done successfully

---

## Mitigation Techniques

| Strategy                     | Description                                                        |
|------------------------------|--------------------------------------------------------------------|
| **Encryption (TLS/SSL)**     | Ensures confidentiality even if traffic is intercepted.            |
| **Certificate Pinning**      | Validates the server certificate to detect fake ones.              |
| **Static ARP Entries**       | Prevents ARP spoofing in smaller environments.                     |
| **DNSSEC**                   | Protects the integrity of DNS responses.                           |
| **Use of VPNs**              | Encrypts traffic from endpoint to VPN server.                      |
| **User Awareness**           | Training to avoid fake Wi-Fi networks and certificate warnings.    |

---

## Summary

- On-path attacks are stealthy and can compromise data integrity and confidentiality.
- They exploit protocol weaknesses or network misconfigurations.
- Layered defense using encryption, proper configuration, and user vigilance is key.

---
