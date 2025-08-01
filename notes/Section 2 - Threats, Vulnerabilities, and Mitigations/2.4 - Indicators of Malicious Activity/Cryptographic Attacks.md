# Cryptographic Attacks

---

Cryptographic attacks aim to break or weaken the encryption mechanisms used to protect data. These attacks exploit weaknesses in algorithms, implementations, or key management.

---

## Common Types of Cryptographic Attacks

| Attack Type                  | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| **Brute-force Attack**       | Attempts every possible key until the correct one is found.                 |
| **Dictionary Attack**        | Uses a list of likely passwords or keys to guess the correct one.          |
| **Birthday Attack**          | Exploits the probability of hash collisions due to the birthday paradox.   |
| **Rainbow Table Attack**     | Uses precomputed hash tables to reverse cryptographic hashes.              |
| **Man-in-the-Middle (MITM)** | Intercepts communication to capture or alter encrypted data.               |
| **Downgrade Attack**         | Forces the use of a weaker encryption method during a handshake.           |
| **Side-channel Attack**      | Exploits physical characteristics (timing, power usage) to extract secrets.|
| **Replay Attack**            | Reuses captured data transmissions (e.g., authentication tokens).          |
| **Chosen Ciphertext Attack** | Attacker can choose ciphertexts to be decrypted and observe outputs.       |

---

## Attack Focus Areas

### 1. **Weak Encryption**
- Use of outdated algorithms like DES or MD5 makes encryption susceptible.
- Modern standards: AES, RSA (2048+ bits), SHA-256, ECC.

### 2. **Poor Key Management**
- Weak, reused, or improperly stored keys can be guessed or stolen.
- Always generate keys securely and rotate them periodically.

### 3. **Improper Implementation**
- Errors in applying cryptographic libraries can expose systems.
- Always use vetted libraries (e.g., OpenSSL, libsodium).

---

## Hashing Attacks

| Attack Type       | Description                                 |
|-------------------|---------------------------------------------|
| **Collision**     | Two inputs produce the same hash.           |
| **Preimage**      | Attacker finds input that matches a hash.   |
| **Second Preimage** | Attacker finds a second input with same hash. |

---

## Defenses Against Cryptographic Attacks

| Defense                     | Description                                                              |
|-----------------------------|--------------------------------------------------------------------------|
| **Use Strong Algorithms**   | Prefer AES, SHA-2, RSA, ECC; avoid MD5, SHA-1.                           |
| **Salting Hashes**          | Adds randomness to hashes to defeat rainbow table attacks.              |
| **Key Rotation**            | Regularly update keys to reduce exposure.                               |
| **Secure Key Storage**      | Store keys in HSMs or encrypted key vaults.                             |
| **TLS Best Practices**      | Enforce strong cipher suites and disable legacy protocols.              |
| **Input Validation**        | Prevent injection attacks that bypass crypto protections.               |
| **Constant-time Algorithms**| Prevent timing attacks (especially in password comparison).             |

---

## Summary

- Cryptographic attacks target weaknesses in encryption algorithms, key management, or implementation.
- Brute-force, MITM, replay, and hash attacks are among the most common.
- Strong algorithms, key handling, and up-to-date libraries significantly reduce the risk.

---
