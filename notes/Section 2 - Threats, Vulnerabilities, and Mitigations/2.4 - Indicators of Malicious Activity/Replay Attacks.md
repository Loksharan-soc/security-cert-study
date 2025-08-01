# Replay Attacks

---

**Replay Attacks** involve intercepting valid data transmissions and fraudulently retransmitting them to gain unauthorized access or manipulate data.

---

## How a Replay Attack Works

1. **Capture** – An attacker records a legitimate data transmission (e.g., login request or transaction).
2. **Delay (Optional)** – The attacker waits until an opportune moment.
3. **Replay** – The attacker resends the intercepted message, hoping the system will accept it as valid.

---

## Example Scenarios

| Scenario                          | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| **Authentication Replay**        | Attacker replays a login request to impersonate a user.                     |
| **Financial Transactions**       | A transaction message is repeated to cause a duplicate charge.              |
| **Session Token Reuse**          | Reuse of an intercepted token to access a web session.                      |

---

## Why It Works

- Systems may not check if messages are **unique** or **fresh**.
- Weak or **no encryption** allows easy capture of data.
- **No session expiration** or **lack of timestamps** means replayed messages are still accepted.

---

## Countermeasures

| Technique                        | Description                                                                |
|----------------------------------|----------------------------------------------------------------------------|
| **Timestamps**                   | Adds freshness to messages, allowing systems to reject old ones.           |
| **Nonces (Number used once)**    | Random values in each session make replays ineffective.                    |
| **Session Tokens**               | Short-lived, unique tokens that expire after use or inactivity.            |
| **Mutual Authentication**        | Both client and server verify identity, reducing impersonation chances.    |
| **Encrypted Channels**           | Prevents attackers from easily reading or capturing usable data.           |
| **Replay Protection Protocols**  | Protocols like Kerberos and TLS include replay protection mechanisms.      |

---

## Example Protocol Protections

| Protocol     | Replay Prevention Mechanism                    |
|--------------|------------------------------------------------|
| **Kerberos** | Uses timestamps and tickets with lifetimes     |
| **TLS**      | Includes session keys and random values        |
| **OAuth2**   | Implements short-lived tokens and scopes       |

---

## Summary

- A replay attack reuses valid communication to gain unauthorized access.
- Common in poorly designed authentication or transaction systems.
- Prevention relies on making each communication unique, time-sensitive, and encrypted.

---
