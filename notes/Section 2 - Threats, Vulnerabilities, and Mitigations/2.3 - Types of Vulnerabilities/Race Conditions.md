# Race Conditions

---

## Overview

A **race condition** is a software vulnerability that occurs when the behavior of a system depends on the timing or sequence of events, particularly when multiple processes or threads access shared resources simultaneously.

---

## How Race Conditions Work

- Two or more operations **compete** to access or modify shared data.
- The final outcome depends on the **order** of execution.
- Attackers exploit timing gaps to manipulate behavior, such as:
  - Gaining unauthorized access
  - Overwriting data
  - Escalating privileges

---

## Real-World Example

1. User requests a file to be written (`temp.txt`).
2. Application checks user permissions.
3. Before the write occurs, the attacker replaces `temp.txt` with a symbolic link to a protected system file.
4. Application writes to the linked system file with elevated privileges.

---

## Common Targets

| Target                        | Risk                                      |
|-------------------------------|-------------------------------------------|
| File Systems                  | Symbolic link attacks, TOCTOU vulnerabilities |
| Authentication Systems        | Bypassing checks during login or access |
| Memory                        | Manipulating variables between checks and use |

> **TOCTOU**: Time Of Check To Time Of Use – a common pattern exploited in race conditions.

---

## Prevention Techniques

- **Atomic Operations**: Ensure that checks and actions happen as one uninterruptible step.
- **Thread Synchronization**: Use locks, semaphores, or mutexes to control access to shared resources.
- **Avoid Shared State**: Minimize dependency on shared data in concurrent systems.
- **Input Re-validation**: Re-check permissions or data immediately before critical operations.

---

## Summary

Race conditions occur when timing differences in concurrent processes lead to unpredictable or exploitable behavior. Preventing them requires careful synchronization and secure design practices.

---
