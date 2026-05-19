# Attacktive Directory — TryHackMe Walkthrough

Comprehensive Active Directory penetration testing walkthrough completed on the TryHackMe platform.

This lab simulates a real-world enterprise Active Directory attack chain involving enumeration, Kerberos attacks, credential discovery, privilege escalation, and full domain compromise techniques commonly encountered during red-team engagements and penetration testing assessments.

---

## Platform Information

- Platform: TryHackMe
- Room: Attacktive Directory
- Category: Active Directory Security
- Difficulty: Medium
- Environment: Windows Active Directory Domain

---

## Project Overview

The assessment targeted a simulated Windows Active Directory environment and focused on identifying weaknesses in authentication, credential management, and privilege delegation.

The engagement included:
- Active Directory Enumeration
- Kerberos User Enumeration
- AS-REP Roasting
- SMB Enumeration
- Credential Discovery
- DCSync Attacks
- NTDS Extraction
- Pass-the-Hash Authentication
- Full Domain Compromise

---

## Attack Methodology

### 1. Network Enumeration
Performed service discovery and identification of Active Directory services using:
- Nmap
- SMB Enumeration
- LDAP Enumeration
- WinRM Discovery

### 2. Kerberos Enumeration
Enumerated valid domain usernames using:
- Kerbrute
- Kerberos AS-REQ responses

### 3. AS-REP Roasting
Identified accounts without Kerberos pre-authentication enabled and retrieved crackable AS-REP hashes using:
- Impacket GetNPUsers.py
- JohnTheRipper

### 4. SMB Enumeration
Enumerated SMB shares and discovered sensitive credential files using:
- smbclient
- enum4linux

### 5. Credential Discovery
Recovered and decoded Base64-encoded credentials stored insecurely within SMB shares.

### 6. Privilege Escalation
Performed a DCSync attack using:
- Impacket secretsdump.py

Extracted NTDS credential hashes from the domain controller.

### 7. Pass-the-Hash Attack
Authenticated remotely as Administrator using:
- Evil-WinRM
- NTLM Hash Authentication

### 8. Full Domain Compromise
Retrieved all challenge flags confirming complete administrative compromise of the domain environment.

---

## Tools Used

- Nmap
- enum4linux
- Kerbrute
- Impacket
- JohnTheRipper
- smbclient
- Evil-WinRM
- Kali Linux

---

## Skills Demonstrated

- Active Directory Enumeration
- Kerberos Exploitation
- AS-REP Roasting
- SMB Enumeration
- Credential Attacks
- DCSync Attacks
- NTDS Extraction
- Pass-the-Hash
- Privilege Escalation
- Windows Domain Security

---

## Key Learning Outcomes

- Understanding enterprise Active Directory attack surfaces
- Identifying insecure Kerberos configurations
- Exploiting weak credential management practices
- Performing privilege escalation in Windows domains
- Simulating realistic penetration testing attack chains
- Understanding post-exploitation techniques in Active Directory environments

