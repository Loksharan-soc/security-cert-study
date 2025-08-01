# Denial of Service (DoS)

---

Denial of Service (DoS) attacks aim to make a system, service, or network resource unavailable to its intended users by overwhelming it with traffic or exploiting vulnerabilities.

---

## Types of DoS Attacks

| Type                    | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| **Volume-based attacks**| Overwhelm bandwidth with massive traffic (e.g., UDP floods, ICMP floods).   |
| **Protocol attacks**    | Exploit weaknesses in Layer 3/4 protocols (e.g., SYN flood, Ping of Death). |
| **Application-layer DoS**| Target specific applications or services (e.g., HTTP GET floods).          |
| **Logic/Software DoS**  | Exploit bugs or limitations in software (e.g., malformed packets).          |

---

## Distributed Denial of Service (DDoS)

A DDoS attack is a coordinated DoS attack launched from multiple compromised systems (often part of a botnet), significantly increasing the attack’s impact.

| Aspect              | Description                                                 |
|---------------------|-------------------------------------------------------------|
| **Botnets**         | Networks of malware-infected devices controlled remotely.   |
| **Amplification**   | Uses protocols like DNS or NTP to magnify traffic volume.   |
| **Reflection**      | Spoofs IP addresses to bounce responses off legitimate servers. |

---

## Common Attack Vectors

- Internet-facing web servers and APIs  
- Network infrastructure (routers, firewalls)  
- VoIP and DNS services  

---

## Impacts

- Service outages and downtime  
- Lost revenue and reputation  
- Increased infrastructure costs  
- Difficulty in distinguishing legitimate traffic  

---

## Mitigation Techniques

| Strategy                     | Description                                                              |
|------------------------------|--------------------------------------------------------------------------|
| **Rate limiting**            | Restricts the number of requests per client or IP.                      |
| **Web application firewalls (WAFs)** | Filters and blocks suspicious HTTP traffic.                     |
| **Intrusion detection/prevention systems (IDS/IPS)** | Identify and block known DoS patterns.       |
| **Geo-blocking / blacklists**| Prevents access from known malicious sources.                           |
| **Cloud-based DDoS protection**| Services like Cloudflare or Akamai absorb large-scale attacks.        |
| **Redundancy and load balancing**| Distributes load across multiple servers to absorb traffic surges. |

---

## Real-World Example

- **GitHub (2018)** was hit with a record-breaking 1.35 Tbps DDoS attack using Memcached reflection.
- **Dyn DNS (2016)**: A DDoS attack on DNS infrastructure disrupted access to major sites like Twitter and Netflix.

---

## Summary

- DoS/DDoS attacks focus on disrupting availability.
- Can be simple (ICMP flood) or complex (multi-vector DDoS).
- Defense involves layered, proactive network and application security.

---
