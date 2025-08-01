# Password Attacks

---

Password attacks attempt to gain unauthorized access by exploiting weak, reused, or poorly protected passwords. These attacks can be automated and are one of the most common cybersecurity threats.

---

## Common Types of Password Attacks

| Attack Type              | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Brute-force Attack**   | Tries all possible combinations until the correct password is found.        |
| **Dictionary Attack**    | Uses a predefined list of common words and passwords to guess credentials.  |
| **Credential Stuffing**  | Reuses credentials from previous breaches to try them on other systems.     |
| **Password Spraying**    | Tries a few common passwords across many accounts to avoid detection.       |
| **Phishing**             | Tricks users into revealing passwords through fake websites or emails.      |
| **Keylogging**           | Records keystrokes to capture user credentials.                             |
| **Shoulder Surfing**     | Observes a user typing their password in person.                            |
| **Social Engineering**   | Manipulates users into revealing their credentials.                         |

---

## Techniques and Tools Used

| Tool / Method        | Usage                                                                 |
|----------------------|-----------------------------------------------------------------------|
| **Hydra, John the Ripper** | Popular brute-force and password cracking tools.              |
| **Hashcat**           | GPU-accelerated password cracker, often used against password hashes. |
| **Rainbow Tables**    | Precomputed hash lookup tables used to reverse weak password hashes. |

---

## Password Storage Attacks

Attackers may attempt to:

- Steal password hashes from a compromised database.
- Reverse weakly hashed passwords using brute-force or rainbow tables.
- Exploit unsalted hashes which are vulnerable to dictionary and rainbow table attacks.

---

## Best Practices for Defense

| Defense Mechanism           | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **Use Strong Passwords**    | Enforce length and complexity (e.g., 12+ characters with mix of symbols).   |
| **Multi-Factor Authentication (MFA)** | Adds an extra layer beyond just passwords.                       |
| **Account Lockout Policies**| Prevents unlimited login attempts (e.g., 5 failed attempts).                |
| **Salting Password Hashes** | Adds unique data before hashing to protect against precomputed attacks.     |
| **Rate Limiting / Throttling** | Slows down brute-force attacks.                                        |
| **Monitor Login Activity**  | Detect and alert on suspicious login patterns.                             |
| **Avoid Password Reuse**    | Each account should have a unique password.                               |
| **User Training**           | Educate users on phishing and secure password practices.                   |

---

## Summary

- Password attacks exploit weak, reused, or stolen credentials.
- Attackers use automated tools and social techniques.
- Strong password policies, MFA, salting, and user education are key defenses.

---
