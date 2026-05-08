# Linux Privilege Escalation Lab

## Overview

This lab demonstrates the process of identifying and exploiting privilege escalation vectors within a vulnerable Linux environment in an isolated and authorized penetration testing lab.

The assessment included network enumeration, web exploitation, reverse shell establishment, SUID enumeration, and privilege escalation through insecure SUID program abuse.

---

## Objectives

- Discover target systems
- Enumerate exposed services
- Identify vulnerable web functionality
- Establish remote shell access
- Enumerate SUID binaries
- Escalate privileges through insecure SUID configurations

---

## Lab Environment

- Kali Linux attacker machine
- Vulnerable Linux target
- Isolated VirtualBox lab network

---

## Tools Used

- arp-scan
- Nmap
- Gobuster
- Dirb
- curl
- Bash
- Kali Linux

---

## Methodology

### 1. Network Enumeration
Performed host discovery using:
- arp-scan

to identify reachable systems in the lab environment.

### 2. Service Enumeration
Used Nmap service detection to identify:
- HTTP services
- SMB services
- RPC services

and analyze exposed attack surface components.

### 3. Web Enumeration
Performed directory and file discovery using:
- Gobuster
- Dirb

which revealed an exposed `shell.php` endpoint.

### 4. Command Execution Validation
Validated remote command execution capabilities through controlled HTTP parameter testing.

### 5. Reverse Shell Establishment
Established a reverse shell session using:
- curl
- bash reverse shell techniques

including URL-encoded payload handling.

### 6. SUID Enumeration
Enumerated SUID binaries using:
- find / -perm -4000

to identify potential privilege escalation vectors.

### 7. Privilege Escalation
Abused an insecure SUID binary to obtain elevated privileges through controlled script execution.

---

## Key Findings

- Vulnerable web functionality enabled remote command execution.
- Reverse shell access was successfully established.
- Misconfigured SUID binaries introduced privilege escalation risk.
- Weak privilege separation significantly increased compromise impact.

---

## Skills Demonstrated

- Linux Enumeration
- Web Exploitation
- Reverse Shell Handling
- SUID Enumeration
- Linux Privilege Escalation
- Bash Usage
- Penetration Testing Methodology

---

## Repository Contents

- Full technical lab report
- Enumeration evidence
- Web exploitation workflow
- Reverse shell validation
- SUID enumeration screenshots
- Privilege escalation evidence

---

## Lessons Learned

- Improperly secured SUID binaries can introduce severe privilege escalation vulnerabilities.
- Enumeration quality directly impacts successful exploitation opportunities.
- Reverse shell handling and privilege escalation require strong Linux fundamentals.

---

## Disclaimer

This project was conducted inside an isolated educational lab environment using intentionally vulnerable systems for authorized security testing and learning purposes only.