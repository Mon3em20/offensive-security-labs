# Jangow Enumeration Lab

## Overview

This lab documents the enumeration and credential discovery process performed against the JANGOW 1.0.1 vulnerable machine within a controlled and authorized penetration testing environment.

The assessment focused on network discovery, service enumeration, directory brute-forcing, sensitive file inspection, and credential identification through exposed artifacts.

---

## Objectives

- Discover exposed services
- Enumerate accessible web resources
- Identify hidden directories and files
- Analyze backup/configuration artifacts
- Validate discovered credentials

---

## Lab Environment

- Kali Linux (VirtualBox)
- JANGOW 1.0.1 vulnerable VM
- Host-only isolated lab network

---

## Tools Used

- Nmap
- Gobuster
- Dirb
- Firefox Developer Tools
- Kali Linux

---

## Methodology

### 1. Network Discovery
Performed host discovery and port scanning to identify reachable services and open ports.

### 2. Service Enumeration
Enumerated exposed FTP and HTTP services using:
- Nmap service detection
- Manual inspection

### 3. Web Enumeration
Conducted directory and content discovery using:
- Gobuster
- Dirb

### 4. Artifact Inspection
Analyzed:
- backup files
- configuration files
- directory listings
- exposed source artifacts

### 5. Credential Discovery
Identified exposed credentials through insecurely accessible backup/configuration data.

### 6. Authentication Validation
Validated discovered credentials through successful authentication testing in the lab environment.

---

## Key Findings

- FTP and HTTP services were publicly exposed.
- Directory brute-forcing revealed sensitive application paths.
- Misconfigured backup/configuration files exposed authentication data.
- Insecure directory listing behavior increased attack surface visibility.
- Credential exposure enabled successful authentication validation.

---

## Skills Demonstrated

- Network Enumeration
- Service Enumeration
- Web Content Discovery
- Directory Brute-Forcing
- Credential Discovery
- Manual Web Inspection
- Penetration Testing Methodology

---

## Repository Contents

- Full technical report
- Enumeration evidence
- Nmap scan results
- Directory discovery screenshots
- Credential discovery documentation
- Authentication validation evidence

---

## Lessons Learned

- Misconfigured backups and exposed configuration files can lead to credential disclosure.
- Enumeration is one of the most critical phases in penetration testing.
- Directory brute-forcing can uncover hidden attack surface components.

---

## Disclaimer

This project was conducted inside an isolated educational lab environment using intentionally vulnerable machines for authorized security testing and learning purposes only.