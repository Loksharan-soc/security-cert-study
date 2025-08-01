# Wireless Attacks

---

Wireless networks are susceptible to various threats due to the open nature of radio communication. Attackers can exploit vulnerabilities in protocols, configurations, or user behavior.

---

## Common Wireless Attack Types

| Attack Type           | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| **Evil Twin**          | Rogue AP that mimics a legitimate one to intercept traffic.                |
| **Rogue Access Point** | Unauthorized AP connected to a network, often used to bypass security.     |
| **Disassociation Attack** | Sends spoofed frames to disconnect users from an AP (DoS).             |
| **Jamming**            | Intentionally interfering with wireless signals (Denial of Service).       |
| **Replay Attack**      | Re-transmits captured packets to gain unauthorized access.                 |
| **WPS Attacks**        | Exploits flaws in Wi-Fi Protected Setup to brute-force PINs.               |
| **Bluejacking/Bluesnarfing** | Bluetooth-based attacks to send unsolicited messages or steal data. |

---

## Evil Twin Attack

- Attacker sets up a fake AP using the same SSID as the real one.
- Victim unknowingly connects and shares sensitive data.
- Often paired with phishing pages or traffic sniffing tools.

---

## Rogue Access Points

- May be installed maliciously or by unaware employees.
- Bypasses firewall and NAC controls.
- Can expose internal networks to external threats.

---

## Disassociation & Deauthentication Attacks

- Uses spoofed **802.11 management frames** to disconnect clients.
- Tools like `aireplay-ng` can automate this.
- Disrupts service and may aid in capturing WPA/WPA2 handshakes.

---

## Jamming

- Overwhelms the wireless spectrum with noise or continuous traffic.
- Can be used to force clients to connect to an Evil Twin AP.

---

## WPS Attacks

- WPS uses an 8-digit PIN which is **brute-forceable**.
- Tools like `Reaver` can exploit WPS-enabled routers in hours.
- WPS should be **disabled** on all APs.

---

## Bluetooth Attacks

| Attack        | Description                                                  |
|---------------|--------------------------------------------------------------|
| **Bluejacking**   | Sends unsolicited messages via Bluetooth.              |
| **Bluesnarfing**  | Unauthorized access to Bluetooth-enabled device data.  |

---

## Mitigation Strategies

| Control                          | Purpose                                               |
|----------------------------------|--------------------------------------------------------|
| **Disable WPS**                  | Prevent brute-force attacks.                          |
| **Strong WPA3/WPA2 Encryption**  | Use secure protocols, avoid WEP and open networks.     |
| **MAC Filtering**                | Allows only known devices (limited effectiveness).     |
| **Monitoring Tools**            | Detect rogue APs, Evil Twins, and signal anomalies.    |
| **Network Segmentation**        | Isolate wireless from sensitive internal networks.     |
| **User Education**              | Prevent connections to unknown or suspicious APs.      |

---

## Summary

- Wireless attacks can be passive (sniffing) or active (disassociation, jamming).
- Secure configuration, monitoring, and disabling risky features like WPS are essential.
- Physical proximity of attackers makes wireless security uniquely challenging.

---
