# DNS Attacks

---

The Domain Name System (DNS) is critical for translating human-readable domain names into IP addresses. Due to its central role in internet communication, DNS is a common target for attacks.

---

## Common DNS Attack Types

| Attack Type             | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| **DNS Poisoning / Spoofing** | Injecting false DNS data into a resolver’s cache, redirecting users to malicious sites. |
| **Pharming**            | Redirecting a legitimate website’s traffic to a fake site, often using DNS poisoning. |
| **DNS Amplification**   | A DDoS technique where small DNS queries result in large responses, flooding the victim. |
| **DNS Tunneling**       | Encodes malicious or hidden data inside DNS queries/responses to bypass security controls. |
| **Typosquatting (URL Hijacking)** | Attacker registers a misspelled domain to capture misdirected traffic. |
| **Zone Transfer Attacks** | Exploits misconfigured DNS servers to retrieve zone files containing sensitive info. |

---

## DNS Poisoning (Cache Poisoning)

- A rogue DNS response is inserted into the DNS resolver’s cache.
- Causes redirection of users to malicious websites.
- Often used in **man-in-the-middle (MitM)** attacks.

### Example

Legitimate query:  
`example.com` → `93.184.216.34`  
Spoofed response:  
`example.com` → `5.6.7.8` (attacker-controlled IP)

---

## DNS Amplification

- The attacker sends a DNS query with a **spoofed victim IP** to open resolvers.
- The resolver sends large DNS responses to the victim.
- Causes **volumetric DDoS**.

| Feature       | Details                                 |
|---------------|------------------------------------------|
| Amplification | Small query → large response (e.g., TXT, ANY records) |
| Protocols     | DNS over UDP is commonly used            |

---

## DNS Tunneling

- Hides command-and-control or data exfiltration traffic inside DNS queries.
- Can bypass firewalls that allow DNS but block other protocols.
- Tools: `iodine`, `dnscat2`, etc.

---

## Mitigation Strategies

| Strategy                     | Description                                              |
|------------------------------|----------------------------------------------------------|
| **DNSSEC**                  | Digitally signs DNS data to prevent tampering.            |
| **Response Rate Limiting**  | Throttles DNS response rates to mitigate amplification.   |
| **Use Secure Resolvers**    | Avoid open or misconfigured DNS servers.                  |
| **Split DNS**               | Internal vs. external DNS zones are handled separately.   |
| **Monitoring and Logging**  | Watch for unusual DNS patterns, tunneling behavior.       |

---

## Summary

- DNS is both essential and vulnerable.
- Attacks include spoofing, tunneling, and amplification.
- Defense involves secure configurations, DNSSEC, and traffic monitoring.

---
