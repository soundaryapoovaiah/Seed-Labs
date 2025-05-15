📘 Overview
This lab focused on exploring how environment variables, Set-UID programs, and various program execution methods (e.g., system(), execve()) can influence software behavior and introduce security risks. Using the SEED Labs framework, we analyzed how attackers can manipulate Unix/Linux system behavior through environment variables, affecting program control, privileges, and system integrity.

🧪 Lab Tasks Covered
Task 1: Manipulating and understanding environment variables using printenv, export, and unset.

Task 2: Analyzing environment variable inheritance from parent to child processes.

Task 3: Studying how execve() handles environment variables.

Task 4: Comparing behavior of system() with regard to environment handling.

Task 5: Observing how Set-UID programs interact with user-defined environment variables.

Task 6: Demonstrating how PATH manipulation can redirect Set-UID program execution to malicious scripts.

Task 7: Investigating the role of LD_PRELOAD and how dynamic linking behaves in Set-UID programs.

Task 8: Comparing the security of system() vs. execve() in Set-UID contexts, and how command injection is possible.

Task 9: Identifying capability leaking, where privileges remain after setuid() due to open file descriptors.

🎓 What I Learned
Through hands-on experimentation, I gained a deep understanding of:

The security implications of environment variables in privileged and non-privileged execution contexts.

How Set-UID mechanisms can be exploited if environment and program behaviors are not properly sanitized.

Why functions like system() pose significant risks in security-critical programs and how execve() offers a safer alternative.

The importance of privilege management, especially when handling files and user input in privileged programs.

How dynamic linker behavior and shared library loading (LD_PRELOAD) can create attack vectors if not restricted.

🌐 Real-World Applications
DevSecOps & Systems Programming: Helps build secure software that doesn't expose unnecessary privileges or paths to exploitation.

Penetration Testing: Skills in privilege escalation, environment exploitation, and injection attacks are foundational for red teaming and vulnerability assessments.

Secure Coding: Enforces secure use of system calls and correct privilege dropping practices in backend/server-side development.

OS & Kernel-level Security: Offers insight into how the Unix permission and execution model can be hardened against common security flaws.
