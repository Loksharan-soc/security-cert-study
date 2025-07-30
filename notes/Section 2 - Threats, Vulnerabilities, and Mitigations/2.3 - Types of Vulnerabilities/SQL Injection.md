# SQL Injection

---

## Overview

**SQL Injection (SQLi)** is a web application attack where an attacker manipulates SQL queries by injecting malicious input. It allows attackers to access, modify, or delete database contents without authorization.

---

## How SQL Injection Works

- User input is improperly validated or sanitized.
- Malicious input alters the structure of SQL queries.
- Can lead to unauthorized data access or full control over the database.

**Example**:
```sql
SELECT * FROM users WHERE username = 'admin' AND password = '1234';
```

If input is:
```sql
' OR '1'='1
```

Final query becomes:
```sql
SELECT * FROM users WHERE username = '' OR '1'='1' AND password = '1234';
```
This always returns `true`, bypassing authentication.

---

## Types of SQL Injection

| Type                  | Description |
|-----------------------|-------------|
| **In-band SQLi**      | Uses the same communication channel for injection and results. Most common type. |
| **Blind SQLi**        | No visible output, but behavior changes are observed to infer information. |
| **Out-of-band SQLi**  | Uses separate channels (e.g., DNS, HTTP) to extract data. Used when standard responses are not available. |

---

## Potential Impacts

- Unauthorized data disclosure  
- Data manipulation or deletion  
- Authentication bypass  
- Complete system compromise  
- Denial of service (DoS)

---

## Prevention Techniques

- **Use Parameterized Queries / Prepared Statements**  
  Safely separate user input from SQL logic.
- **Input Validation**  
  Reject or sanitize suspicious characters (e.g., `'`, `--`, `;`).
- **Least Privilege Access**  
  Restrict database user permissions.
- **Web Application Firewalls (WAF)**  
  Detect and block malicious patterns.
- **Code Reviews & Penetration Testing**  
  Identify vulnerable points before attackers do.

---

## Summary

SQL Injection is a critical and common web vulnerability. Mitigating it requires strong input validation, use of secure coding practices, and limiting database privileges.

---
