# Web Developer – VulnHub Walkthrough

## Machine Information
- Difficulty: Easy–Medium
- OS: Linux
- Objective: Root access

## Attack Summary
Web enumeration revealed exposed directories and credentials within application files.
These credentials enabled SSH access, followed by privilege escalation.

## Tools Used
- Nmap – Network scanning and service discovery
- Gobuster – Web directory enumeration
- Burp Suite – Web application analysis
- SSH Client – Remote system access

## Vulnerabilities & CVSS

## Vulnerabilities Identified & CVSS Scores

### 1. Sensitive Information Disclosure (Web Application)
- Description: Application files exposed sensitive credentials due to improper access controls.
- Impact: Credential compromise leading to unauthorized access.
- Attack Vector: Network
- CVSS v3 Score: 7.1 (High)

### 2. Weak Credential Management
- Description: Hardcoded or reused credentials were identified and abused.
- Impact: Unauthorized SSH access to the system.
- Attack Vector: Network
- CVSS v3 Score: 7.5 (High)

### 3. Privilege Escalation
- Description: Misconfigured permissions allowed escalation from user to root.
- Impact: Full system compromise.
- Attack Vector: Local
- CVSS v3 Score: 6.8 (Medium)

## Lessons Learned
- Secure storage of credentials
- Proper web application hardening

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
The machine was tested in a controlled lab environment provided by VulnHub.  
No real-world systems were targeted.
