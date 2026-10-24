# Application and Web Application Security - VAPT Project

## Project Overview
This repository contains the Vulnerability Assessment and Penetration Testing (VAPT) project report for the **Simplilearn Advanced Executive Program in Cybersecurity (AEP CS)**. The objective of this assessment was to simulate real-world hacking scenarios on the target **VulnVMa Web Application** to discover hidden directories, configuration flaws, and sensitive data leakage.

## Target Environment
* **Target System:** VulnVMa Web Application
* **Target IP Address:** `192.168.56.3`
* **Attacker Machine:** Kali Linux (`192.168.56.5`)
* **Environment:** Oracle VM VirtualBox (Isolated Host-Only Network)

## Key Findings & Exploits Documented
1. **Information Leakage via `robots.txt` (Flag 2):** Discovered exposed plain-text flags and sensitive directories due to weak configurations.
2. **Hidden Configuration Folders (Flag 5):** Located an exposed `phpinfo()` setup page revealing backend architecture and programming versions.
3. **Front-End Source Code Comments (Flag 4):** Extracted temporary developer notes and tokens left exposed inside the live HTML source code.
4. **Traffic Interception (Flag 6):** Intercepted unencrypted plain-text login parameters in transit using Burp Suite.

## Tools Used
* Kali Linux
* Firefox Developer Tools
* Burp Suite Community Edition
* Oracle VM VirtualBox

