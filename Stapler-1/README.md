# Stapler: 1 – VulnHub Walkthrough

## Machine Information
- Platform: VulnHub
- Machine Name: Stapler: 1
- Difficulty: Medium
- Operating System: Linux
- Objective: Gain root access

---

## 1. Reconnaissance

The target IP address was identified using network discovery techniques.
An Nmap scan was performed to enumerate open ports and running services.

The scan revealed multiple exposed services including FTP, SSH, HTTP, and SMB,
indicating a large attack surface.

---

## 2. Enumeration

### SMB Enumeration
SMB enumeration revealed accessible shares containing files with sensitive information.
Some files contained user-related data which was useful for further attacks.

### Web Enumeration
The web service was enumerated using directory brute-forcing techniques.
Hidden directories and files were discovered, exposing additional information
related to the system and users.

### FTP Enumeration
The FTP service allowed anonymous access, exposing files that contained credentials
and configuration details.

---

## 3. Initial Access

Based on information gathered from enumeration, valid credentials were identified.
These credentials were used to successfully authenticate to the system via SSH,
providing initial user-level access.

---

## 4. Privilege Escalation

Post-exploitation enumeration was performed after gaining shell access.
Insecure sudo configurations and misconfigured permissions were identified.

Privilege escalation techniques were applied, allowing elevation of privileges
from a standard user to root.

---

## 5. Root Access

Root access was successfully obtained, completing the objective of the machine.

---

## 6. Tools Used

- Nmap – Network scanning and service enumeration
- Enum4linux – SMB enumeration
- SMBClient – Accessing SMB shares
- Gobuster / Dirb – Web directory enumeration
- FTP Client – FTP enumeration
- SSH Client – Remote shell access
- Linux Enumeration Commands – Post-exploitation analysis

---

## 7. Vulnerabilities Identified & CVSS Scores

### 1. Anonymous FTP Access
- Description: FTP service allowed anonymous login, exposing sensitive files.
- Impact: Information disclosure leading to credential compromise.
- Attack Vector: Network
- CVSS v3 Score: 7.5 (High)

### 2. Insecure SMB Shares
- Description: SMB shares were accessible without proper access control.
- Impact: Exposure of sensitive user data.
- Attack Vector: Network
- CVSS v3 Score: 7.1 (High)

### 3. Weak Credentials
- Description: Credentials obtained during enumeration were reused for SSH access.
- Impact: Unauthorized system access.
- Attack Vector: Network
- CVSS v3 Score: 7.5 (High)

### 4. Privilege Escalation via Misconfiguration
- Description: Improper sudo permissions allowed privilege escalation to root.
- Impact: Full system compromise.
- Attack Vector: Local
- CVSS v3 Score: 6.8 (Medium)

---

## 8. Lessons Learned

- Risks of exposing multiple unnecessary services
- Importance of proper access controls on FTP and SMB services
- Dangers of credential reuse across services
- Need for secure sudo and permission configurations

---

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
The machine was tested in a controlled lab environment provided by VulnHub.  
No real-world systems were targeted.
