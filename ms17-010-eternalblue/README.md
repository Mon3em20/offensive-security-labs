# MS17-010 EternalBlue Exploitation Lab

## Overview

This lab documents the identification and exploitation of the MS17-010 (EternalBlue) vulnerability against a vulnerable Windows 7 machine within an isolated and authorized penetration testing lab environment.

Both automated and manual exploitation techniques were performed to understand the exploitation workflow, vulnerability validation process, and session establishment methodology.

---

## Objectives

- Perform network discovery
- Enumerate SMB services
- Identify MS17-010 vulnerability exposure
- Validate vulnerability presence
- Gain controlled Meterpreter access
- Compare automated and manual exploitation workflows

---

## Lab Environment

- Kali Linux attacker machine
- Vulnerable Windows 7 SP1 target
- VirtualBox isolated lab network

---

## Tools Used

- arp-scan
- Nmap
- Metasploit Framework
- AutoBlue-MS17-010
- Meterpreter
- Kali Linux

---

## Methodology

### 1. Host Discovery
Used arp-scan to identify reachable systems within the local subnet.

### 2. Service Enumeration
Performed Nmap scanning to identify:
- SMB services
- Operating system information
- Open ports
- Vulnerable SMB configurations

### 3. Vulnerability Validation
Validated exposure to:
- MS17-010 (EternalBlue)

through SMB enumeration and Metasploit verification.

### 4. Automated Exploitation
Performed exploitation using:
- Metasploit Framework
- exploit/windows/smb/ms17_010_eternalblue

to establish a Meterpreter session.

### 5. Session Validation
Validated successful access using:
- sysinfo
- Meterpreter session inspection

### 6. Manual Exploitation
Performed manual exploitation using:
- AutoBlue-MS17-010

including:
- shellcode preparation
- payload generation
- exploit execution

---

## Key Findings

- SMB service was publicly exposed on port 445.
- The target system was vulnerable to MS17-010.
- Both automated and manual exploitation methods successfully established controlled access.
- Lack of patch management significantly increased compromise risk.

---

## Skills Demonstrated

- Network Enumeration
- SMB Enumeration
- Vulnerability Validation
- Metasploit Usage
- Windows Exploitation
- Meterpreter Session Handling
- Penetration Testing Methodology

---

## Repository Contents

- Full technical exploitation report
- Enumeration evidence
- Nmap scanning results
- Metasploit exploitation screenshots
- Manual exploitation workflow
- Session validation evidence

---

## Lessons Learned

- Legacy SMB vulnerabilities remain highly critical when systems are unpatched.
- Enumeration accuracy is essential before exploitation attempts.
- Understanding both automated and manual exploitation methods improves technical depth and troubleshooting skills.

---

## Disclaimer

This project was conducted inside an isolated educational lab environment using intentionally vulnerable machines for authorized security testing and learning purposes only.