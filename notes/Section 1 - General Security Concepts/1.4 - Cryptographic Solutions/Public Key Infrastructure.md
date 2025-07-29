# Public Key Infrastructure

---

## What is Public Key Infrastructure (PKI)?

PKI is a framework that manages digital certificates and public-key encryption to enable secure communication and identity verification over networks.

---

## Components of PKI

| Component              | Description                                    |
|------------------------|------------------------------------------------|
| Certificate Authority (CA) | Trusted entity that issues and manages certificates |
| Registration Authority (RA) | Verifies identities before certificates are issued |
| Digital Certificates    | Electronic documents binding public keys to identities |
| Public/Private Keys     | Key pair used for encryption and digital signatures |
| Certificate Revocation List (CRL) | List of revoked or invalid certificates           |

---

## How PKI Works

1. User or device generates a **key pair** (public and private keys).
2. Public key is sent to the **CA** to request a certificate.
3. CA verifies identity (via RA) and issues a **digital certificate**.
4. Certificates are used to **encrypt data** or **verify signatures**.
5. Other parties use the CA’s public key to validate certificates.

---

## Uses of PKI

- Secure web browsing (TLS/SSL).
- Email encryption and signing.
- Code signing.
- VPN authentication.
- Document signing.

---

## Certificate Formats

- X.509 is the most common standard.
- Contains information like issuer, subject, validity period, and public key.

---

## Certificate Revocation

- Certificates can be revoked before expiry if compromised.
- CRLs and Online Certificate Status Protocol (OCSP) are used to check revocation status.

---

## Summary

PKI enables trusted, secure communication by managing keys and certificates, providing mechanisms for encryption, authentication, and non-repudiation.

---
