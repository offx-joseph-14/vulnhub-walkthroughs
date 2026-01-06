# Metasploitable 3 – VulnHub Walkthrough

## Machine Information
- Platform: VulnHub
- Machine Name: Metasploitable 3
- Difficulty: Medium
- Operating System: Windows
- Objective: Gain administrative access

---

## Attack Overview
Metasploitable 3 is a modern vulnerable environment designed to simulate real-world
enterprise systems. Enumeration identified misconfigurations and vulnerable services
leading to remote access and privilege escalation.

---

## Attack Flow
Reconnaissance → Service Enumeration → Exploitation → Privilege Escalation

---

## 1. Reconnaissance
Network scanning identified exposed services including web services and Windows-based components.
Service enumeration confirmed the presence of vulnerable configurations.

---

## 2. Enumeration
Web and service enumeration revealed misconfigured applications and weak security controls,
providing opportunities for exploitation.

---

## 3. Exploitation
Identified vulnerabilities were exploited to gain initial access to the system.
Remote access was successfully established.

---

## 4. Privilege Escalation
Post-exploitation analysis revealed insecure permissions and misconfigurations,
allowing escalation to administrative privileges.

---

## 5. Administrative Access
Administrator-level access was obtained, completing the objective.

---

## 6. Tools Used
- Nmap – Network and service discovery
- Metasploit Framework – Exploitation of vulnerable services
- Burp Suite – Web application analysis
- Windows Enumeration Techniques
- PowerShell (Post-Exploitation Enumeration)

---

## 7. Vulnerabilities Identified & CVSS Scores

### 1. Vulnerable Web Application
- Description: Web services exposed vulnerabilities leading to remote access.
- Impact: Unauthorized system access
- Attack Vector: Network
- CVSS v3 Score: 8.8 (High)

### 2. Insecure Windows Configuration
- Description: Misconfigured permissions allowed privilege escalation.
- Impact: Administrative access
- Attack Vector: Local
- CVSS v3 Score: 7.0 (High)

---

## 8. Lessons Learned
- Importance of secure Windows configuration
- Risks of misconfigured enterprise services
- Need for proper access control and monitoring
- Value of defense-in-depth strategies

---

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
All testing was performed in a controlled lab environment using Metasploitable 3.  
No production or real-world systems were involved.
