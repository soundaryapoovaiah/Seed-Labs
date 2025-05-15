Lab Overview

This project focuses on evaluating security risks using the OWASP Risk Rating Methodology to determine the most effective software upgrade path for a business. Two software packages were evaluated: Microsoft Office and Adobe Acrobat Reader, both of which were outdated and prone to exploitation. The analysis was based on two adversary scenarios:

Advanced Targeted Attack: A skilled attacker aims to steal intellectual property.

Opportunistic Attack: A general attacker exploits system vulnerabilities to steal or ransom user PII.

📊 Key Tasks Threat Modeling: Factored in attacker skill, motive, opportunity, and size.

Risk Calculation: Combined likelihood and impact based on OWASP guidelines.

Exploit Analysis: Used Metasploit module rankings to evaluate software version vulnerabilities.

Upgrade Evaluation: Considered software upgrade costs and compatibility risks.

✅ Final Recommendations Scenario 1 (Targeted IP Theft): Upgrade to Microsoft Office 2010 due to its significantly improved security profile and lower exploitability.

Scenario 2 (PII Ransom Threat): Upgrade to Adobe Acrobat Reader 11, which addresses numerous high-severity vulnerabilities found in earlier versions.

💡 What I Learned This lab reinforced my understanding of:

Security risk assessment frameworks, especially OWASP's methodology.

Threat agent profiling and calculating vulnerability likelihood using real-world exploit databases like Metasploit.

Data-driven decision-making in cybersecurity, where cost-benefit analysis balances risk reduction and operational overhead.

Communicating technical findings effectively in a structured, business-aligned report.

🌐 Real-World Applications In a professional setting, these skills are essential for roles like Security Analyst, DevSecOps Engineer, or IT Risk Consultant.

The ability to interpret vulnerability data and recommend actionable mitigations can protect organizations from financial and reputational damage.

Understanding exploit patterns through platforms like Metasploit helps proactively defend systems against known attack vectors.

This approach can be scaled for broader enterprise vulnerability management, compliance auditing, and incident response planning.
