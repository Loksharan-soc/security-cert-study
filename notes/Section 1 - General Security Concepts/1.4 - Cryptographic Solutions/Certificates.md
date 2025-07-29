# Certificates

---

## What are Digital Certificates?

Digital certificates are electronic documents used to prove the ownership of a public key. They bind public keys to entities (individuals, organizations, or devices) through a trusted third party.

---

## Key Components of a Certificate

| Component          | Description                              |
|--------------------|------------------------------------------|
| Subject            | Entity the certificate belongs to        |
| Public Key         | The public key of the subject            |
| Issuer             | Certificate Authority (CA) issuing the certificate |
| Validity Period    | Start and end dates for certificate validity |
| Serial Number      | Unique identifier for the certificate    |
| Signature          | Digital signature from the CA            |

---

## Certificate Authorities (CAs)

- Trusted entities that issue and sign certificates.
- Validate identity before issuing certificates.
- Manage certificate revocation and renewal.

---

## Certificate Formats

- **X.509** is the most common standard.
- Certificates may be in formats like PEM, DER, or PFX.

---

## Certificate Lifecycle

| Stage              | Description                                 |
|--------------------|---------------------------------------------|
| Request            | Entity requests a certificate from CA       |
| Issuance           | CA verifies identity and issues certificate |
| Usage              | Certificates are used for authentication, encryption, or signing |
| Renewal            | Certificates are renewed before expiration  |
| Revocation         | Certificates can be revoked if compromised  |

---

## Revocation Methods

- **Certificate Revocation List (CRL)**: List of revoked certificates.
- **Online Certificate Status Protocol (OCSP)**: Real-time revocation status checking.

---

## Summary

Certificates are foundational to secure communications, establishing trust by linking public keys to verified identities through trusted authorities.

---
