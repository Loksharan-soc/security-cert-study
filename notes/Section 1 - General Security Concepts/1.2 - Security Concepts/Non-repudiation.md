# Non-repudiation


---

## What is Non-repudiation?

**Non-repudiation** ensures that a party in a communication cannot deny the authenticity of their signature, message, or transaction.

It provides **proof of origin**, **proof of integrity**, and **proof of delivery**, which can be used to resolve disputes or verify events.

---

## Why It Matters

- Prevents **denial of actions** by users or systems.
- Supports **accountability and auditability** in secure systems.
- Essential for **legal, financial, and forensic** contexts.

---

## How Non-repudiation is Enforced

| Mechanism                  | Role in Non-repudiation                        |
|----------------------------|------------------------------------------------|
| **Digital Signatures**     | Verify sender identity and message integrity   |
| **Public Key Infrastructure (PKI)** | Ensures trust and certificate validity     |
| **Logging & Auditing**     | Track user actions and access history          |
| **Time Stamps**            | Show when actions occurred                     |
| **Receipts & Confirmations** | Proof of delivery and acknowledgment          |

---

## Example Scenario

- Alice signs an email using her **private key**.
- Bob verifies it using Alice's **public key**.
- Bob knows:
  - Alice authored the email (authenticity),
  - It wasn’t altered in transit (integrity),
  - Alice can’t deny sending it (non-repudiation).

---

## Key Points

- Relies heavily on **cryptographic techniques**.
- Tied closely to **digital identity** and **logging**.
- **Non-repudiation = No denial possible.**

---

## Summary

Non-repudiation ensures actions or communications **cannot be denied** later by the entities involved. It's a vital component in any secure system requiring trust, verification, and accountability.

---
