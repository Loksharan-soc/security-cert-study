# Hashing and Digital Signatures

---

## Hashing

### What is Hashing?

Hashing is the process of transforming data into a fixed-size string of characters, which is typically a digest that represents the original data uniquely.

### Characteristics

- Fixed output size regardless of input size.
- Deterministic: same input always produces the same hash.
- One-way function: cannot reverse to get original data.
- Small changes in input produce significantly different hashes (avalanche effect).

### Common Hash Algorithms

| Algorithm         | Notes                         |
|-------------------|-------------------------------|
| MD5               | Outdated, vulnerable to collisions |
| SHA-1             | Deprecated, weak collisions    |
| SHA-2 (SHA-256, SHA-512) | Widely used, secure          |
| SHA-3              | Newer standard, strong security |

---

## Digital Signatures

### What is a Digital Signature?

A digital signature is a cryptographic mechanism used to verify the authenticity and integrity of a message, software, or digital document.

### How it Works

- The sender creates a hash of the message.
- The hash is encrypted with the sender's **private key**.
- The recipient decrypts the signature using the sender’s **public key**.
- The recipient hashes the original message and compares it with the decrypted hash.
- If they match, the message is authentic and unaltered.

### Benefits

- Provides **non-repudiation**.
- Ensures **integrity** of the message.
- Confirms **authenticity** of the sender.

---

## Summary

Hashing creates a unique fingerprint of data, while digital signatures combine hashing and asymmetric encryption to provide authenticity, integrity, and non-repudiation.

---
