# Cron PATH Hijacking Privilege Escalation Lab

## Overview

This lab demonstrates the process of exploiting insecure cron job configurations and PATH hijacking vulnerabilities within a vulnerable Linux environment in an isolated and authorized penetration testing lab.

The assessment included reconnaissance, service enumeration, web exploitation, reverse shell establishment, shell stabilization, cron job analysis, and privilege escalation through insecure PATH handling.

---

## Objectives

- Perform network and service enumeration
- Identify vulnerable web functionality
- Establish reverse shell access
- Analyze cron job configurations
- Identify insecure PATH usage
- Escalate privileges through PATH hijacking

---

## Lab Environment

- Kali Linux attacker machine
- Vulnerable Linux target
- Isolated VirtualBox lab network

---

## Tools Used

- arp-scan
- Nmap
- DIRB
- curl
- Netcat
- Bash
- John the Ripper
- Kali Linux

---

## Methodology

### 1. Network Discovery
Performed ARP-based host discovery to identify reachable systems within the lab environment.

### 2. Service Enumeration
Used Nmap service detection to identify:
- HTTP services
- Samba services
- RPC services
- NFS exposure

### 3. Web Enumeration
Performed directory and file enumeration using:
- DIRB

which identified an exposed `shell.php` endpoint vulnerable to command execution.

### 4. Reverse Shell Establishment
Established reverse shell access through controlled command execution and Netcat listener configuration.

### 5. Shell Stabilization
Improved shell usability through:
- PTY spawning
- Terminal environment configuration

to obtain a more stable interactive shell.

### 6. Cron Job Enumeration
Analyzed scheduled tasks through:
- `/etc/crontab`

and identified vulnerable cron script execution behavior.

### 7. PATH Hijacking Exploitation
Exploited insecure PATH handling behavior within a cron-executed script to achieve privilege escalation in the lab environment.

---

## Key Findings

- Vulnerable web functionality enabled remote command execution.
- Insecure cron job configuration increased privilege escalation exposure.
- Improper PATH handling allowed execution of attacker-controlled binaries.
- Weak privilege separation significantly increased compromise impact.

---

## Skills Demonstrated

- Linux Enumeration
- Web Exploitation
- Reverse Shell Handling
- Shell Stabilization
- Cron Job Analysis
- PATH Hijacking
- Linux Privilege Escalation
- Penetration Testing Methodology

---

## Repository Contents

- Full technical lab report
- Enumeration evidence
- Reverse shell workflow
- Shell stabilization process
- Cron job analysis
- Privilege escalation evidence

---

## Lessons Learned

- Cron jobs running with elevated privileges can introduce severe security risks when improperly configured.
- PATH hijacking remains an effective privilege escalation vector in insecure environments.
- Proper privilege separation and secure script execution practices are critical for Linux system security.

---

## Disclaimer

This project was conducted inside an isolated educational lab environment using intentionally vulnerable systems for authorized security testing and learning purposes only.