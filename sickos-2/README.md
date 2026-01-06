# SickOS: 2 – VulnHub Walkthrough

## Machine Information
- Difficulty: Medium
- OS: Linux

## Attack Summary
Web enumeration exposed insecure CGI scripts allowing command execution.
The attacker gained shell access and escalated privileges.

## Tools Used
- Nmap
- Gobuster
- Burp Suite
- Netcat

## Vulnerabilities & CVSS

1. Insecure CGI Script  
CVSS: 9.8 (Critical)

2. Privilege Escalation via Misconfiguration  
CVSS: 6.8 (Medium)

## Lessons Learned
- Disable unnecessary CGI scripts
- Harden server permissions

⚠️ Disclaimer  
This walkthrough is for educational purposes only.  
The machine was tested in a controlled lab environment provided by VulnHub.  
No real-world systems were targeted.
