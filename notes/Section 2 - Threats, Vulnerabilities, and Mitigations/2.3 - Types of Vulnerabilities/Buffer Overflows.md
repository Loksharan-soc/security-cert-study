# Buffer Overflows

---

## Overview

A **buffer overflow** occurs when a program writes more data to a memory buffer than it can hold. This can overwrite adjacent memory, leading to crashes, unexpected behavior, or the execution of malicious code.

---

## How It Works

- Applications allocate fixed-size memory buffers.
- If more data than expected is written, it overflows into adjacent memory.
- Attackers exploit this to:
  - **Crash** programs (denial of service).
  - **Inject shellcode** or other malicious instructions.
  - **Redirect execution flow**, e.g., by overwriting return addresses.

---

## Types of Buffer Overflows

| Type                     | Description |
|--------------------------|-------------|
| **Stack Overflow**       | Occurs in the call stack; can overwrite return addresses or function pointers. |
| **Heap Overflow**        | Targets dynamically allocated memory in the heap; often used to corrupt objects or data structures. |
| **Integer Overflow**     | Involves calculations that exceed the maximum value of a data type, leading to memory mismanagement. |

---

## Real-World Example

- An attacker sends an input string longer than what a buffer can handle.
- The excess data includes executable code (shellcode).
- Control flow is hijacked, and the shellcode executes with the program’s privileges.

---

## Prevention Techniques

- **Input Validation**: Limit and sanitize all user input.
- **Bounds Checking**: Ensure buffers are not exceeded.
- **Stack Canaries**: Special values placed on the stack to detect overwrites.
- **DEP (Data Execution Prevention)**: Prevents execution in non-code memory areas.
- **ASLR (Address Space Layout Randomization)**: Randomizes memory addresses to make targeting harder.
- **Safe Libraries**: Use functions that limit input sizes (e.g., `strncpy` instead of `strcpy`).

---

## Summary

Buffer overflows exploit poor memory management to execute malicious code or crash systems. Preventing them requires strong coding practices, runtime protections, and proper input validation.

---
