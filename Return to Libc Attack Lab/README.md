📘 Overview

This lab explored the Return-to-libc attack, a powerful variant of buffer overflow that bypasses non-executable stack protections by redirecting control flow to existing libc functions like system(). We worked in a controlled SEED Ubuntu VM environment to analyze vulnerabilities in a Set-UID root program, craft exploit payloads, and defeat various Linux countermeasures.

🧪 Key Lab Tasks

Disabled security features: Turned off ASLR, StackGuard, and stack execution permissions.

Address discovery: Used gdb to locate addresses of system(), exit(), and /bin/sh.

Payload creation: Crafted a malicious input (badfile) using Python to control return flow.

Privilege escalation: Exploited the vulnerable program to spawn a root shell.

Bypass variations:

Without exit() (leads to segmentation fault after shell exit).

Executable name change breaks the exploit due to shifted environment variables.

Advanced bypass: Defeated shell countermeasures using execv() and crafted argument arrays on the stack to invoke /bin/bash -p.

💡 What I Learned

How return-to-libc attacks operate when stacks are non-executable.

The structure and manipulation of call stacks during function invocation.

Tools like GDB for binary analysis and stack inspection.

The critical impact of stack offset alignment, and environment variable manipulation.

Security flaws in using functions like system() and the importance of secure coding practices in C.

🌍 Real-World Applications

Penetration Testing: Demonstrates practical exploitation techniques used in privilege escalation.

Secure Software Development: Teaches why dangerous functions (e.g., strcpy(), system()) must be avoided or hardened.

Cybersecurity Engineering: Provides insight into binary exploitation, memory safety, and how modern OS countermeasures can be circumvented.

Incident Response: Enables recognition of exploitation footprints like stack manipulation and command injection attempts.
