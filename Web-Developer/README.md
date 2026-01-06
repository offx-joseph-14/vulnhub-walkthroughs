# Web Developer – VulnHub Walkthrough

## Machine Information
- Difficulty: Easy–Medium
- OS: Linux
- Objective: Root access

## Attack Summary
Web enumeration revealed exposed directories and credentials within application files.
These credentials enabled SSH access, followed by privilege escalation.

## Tools Used
- Nmap
- Gobuster
- Burp Suite
- SSH

## Vulnerabilities & CVSS

1. Sensitive Information Disclosure (Web App)  
CVSS: 7.1 (High)

2. Weak Credential Management  
CVSS: 7.5 (High)

3. Privilege Escalation  
CVSS: 6.8 (Medium)

## Lessons Learned
- Secure storage of credentials
- Proper web application hardening

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
The machine was tested in a controlled lab environment provided by VulnHub.  
No real-world systems were targeted.
