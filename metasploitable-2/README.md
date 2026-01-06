# Metasploitable 2 – VulnHub Walkthrough

## Machine Information
- Platform: VulnHub
- Machine Name: Metasploitable 2
- Difficulty: Easy
- Operating System: Linux
- Objective: Gain root access

---

## Attack Overview
Metasploitable 2 is an intentionally vulnerable Linux system exposing multiple outdated
and insecure services. Enumeration revealed several critical vulnerabilities that could
be exploited to gain remote access and escalate privileges.

---

## Attack Flow
Reconnaissance → Service Enumeration → Remote Exploitation → Privilege Escalation

---

## 1. Reconnaissance
Network scanning revealed multiple open ports and services, indicating a large attack surface.
Service version detection confirmed the presence of outdated software.

---

## 2. Enumeration
Detailed enumeration identified vulnerable services including FTP, SMB, HTTP, and database services.
Several services were found to be running with default or insecure configurations.

---

## 3. Exploitation
Known vulnerabilities in exposed services were exploited to gain remote command execution
and shell access to the target system.

---

## 4. Privilege Escalation
Due to insecure configurations and vulnerable services running with elevated privileges,
root access was achieved without significant resistance.

---

## 5. Root Access
Root-level access was successfully obtained, completing the objective.

---

## 6. Tools Used
- Nmap – Network scanning and service version detection
- Metasploit Framework – Exploiting known service vulnerabilities
- SMBClient – SMB enumeration
- FTP Client – FTP enumeration
- Linux Enumeration Commands

---

## 7. Vulnerabilities Identified & CVSS Scores

### 1. Multiple Outdated Services (RCE)
- Description: Several services were running outdated versions with known remote code execution flaws.
- Impact: Full system compromise
- Attack Vector: Network
- CVSS v3 Score: 9.8 (Critical)

### 2. Default / Weak Credentials
- Description: Services configured with default or weak credentials.
- Impact: Unauthorized access
- Attack Vector: Network
- CVSS v3 Score: 7.5 (High)

### 3. Insecure Service Configuration
- Description: Services running with excessive privileges.
- Impact: Privilege escalation to root
- Attack Vector: Local
- CVSS v3 Score: 6.8 (Medium)

---

## 8. Lessons Learned
- Risks of running outdated software
- Importance of reducing exposed services
- Need for secure configuration and patch management
- Dangers of default credentials

---

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
All testing was conducted in an isolated lab environment using Metasploitable 2.  
No real-world systems were targeted.
