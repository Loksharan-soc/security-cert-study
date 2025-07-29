# Key Exchange

---

## What is Key Exchange?

Key exchange is the process by which two parties securely share cryptographic keys to enable encrypted communication.

---

## Common Key Exchange Methods

| Method                 | Description                                       |
|------------------------|-------------------------------------------------|
| Diffie-Hellman (DH)    | Allows two parties to generate a shared secret over an insecure channel without directly transmitting the key |
| Elliptic Curve Diffie-Hellman (ECDH) | A variant of DH using elliptic curve cryptography, offering stronger security with smaller keys |
| RSA Key Exchange       | Uses asymmetric encryption to securely exchange symmetric keys |

---

## Purpose

- Establish a **shared secret key** for symmetric encryption.
- Ensure confidentiality even if communication is intercepted.

---

## Considerations

- Protect against **man-in-the-middle (MITM) attacks** (often mitigated by authentication).
- Use ephemeral keys for **perfect forward secrecy**.

---

## Summary

Secure key exchange protocols enable encrypted communication by allowing parties to agree on secret keys securely, forming the foundation for secure sessions.

---
