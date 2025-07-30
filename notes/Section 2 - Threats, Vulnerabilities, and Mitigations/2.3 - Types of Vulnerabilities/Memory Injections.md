# Memory Injections

---

## Overview

**Memory injection attacks** occur when malicious code is inserted directly into a system’s memory. These attacks allow the code to execute without being written to disk, making detection by traditional antivirus systems difficult.

---

## Common Types of Memory Injection

| Technique                | Description |
|---------------------------|-------------|
| **DLL Injection**         | Injects a malicious Dynamic Link Library (DLL) into a running process. The DLL executes with the same privileges as the host process. |
| **Shellcode Injection**   | Inserts custom machine code (shellcode) into memory, then redirects execution to it. Often used in buffer overflow exploits. |
| **Process Hollowing**     | Suspends a legitimate process, replaces its memory with malicious code, then resumes it. Used by malware to masquerade as trusted processes. |
| **Reflective DLL Injection** | Loads a DLL into memory without using the Windows loader. Leaves no trace on disk. |
| **Code Injection**        | General term for placing code into another process’s memory space, typically using system APIs like `WriteProcessMemory` and `CreateRemoteThread`. |

---

## Characteristics

- **Fileless**: No files are written to disk, reducing the chance of detection.
- **Stealthy**: Runs in the context of legitimate processes.
- **Persistent**: Can be used to maintain long-term access or for privilege escalation.

---

## Prevention and Detection

- **Endpoint Detection and Response (EDR)**: Detects suspicious in-memory behavior.
- **Memory Scanning**: Monitors running processes for anomalies.
- **Behavioral Analysis**: Looks for signs of abnormal application behavior.
- **Code Signing**: Allows only signed and trusted code to execute.
- **Application Whitelisting**: Prevents unauthorized applications from running.

---

## Summary

Memory injection attacks allow malicious code to execute directly in RAM, bypassing many traditional defenses. Modern protection relies on behavior-based detection and memory analysis rather than just file scanning.

---
