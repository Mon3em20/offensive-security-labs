# Shopify Reconnaissance Lab

## Overview

This project demonstrates passive reconnaissance and OSINT techniques performed against the publicly accessible domain `shopify.com` within an educational and authorized lab environment.

The objective was to practice information gathering, DNS analysis, subdomain enumeration, and technology fingerprinting using industry-standard reconnaissance methodologies.

---

## Scope

- Passive reconnaissance only
- No exploitation or intrusive scanning
- Publicly available information sources
- Educational and authorized use only

---

## Topics Covered

- WHOIS analysis
- DNS record enumeration
- IPv4/IPv6 resolution
- Passive subdomain enumeration
- Technology stack fingerprinting
- Cloud infrastructure identification
- OSINT collection

---

## Tools Used

- Kali Linux
- Sublist3r
- crt.sh
- DNSDumpster
- dig
- nslookup
- WhatWeb
- Wappalyzer
- WHOIS

---

## Methodology

### 1. WHOIS Enumeration
Collected publicly available domain registration and registrar information using WHOIS queries.

### 2. DNS Resolution
Performed IPv4 (A) and IPv6 (AAAA) lookups using:
- dig
- nslookup

### 3. Passive Subdomain Enumeration
Enumerated subdomains using:
- Sublist3r
- crt.sh
- DNSDumpster

### 4. Batch DNS Analysis
Resolved discovered subdomains using automated DNS queries and analyzed associated IP addresses.

### 5. Technology Fingerprinting
Identified:
- CDN providers
- Web frameworks
- Security headers
- JavaScript frameworks
- Hosting infrastructure

using:
- WhatWeb
- Wappalyzer

---

## Key Findings

- Shopify infrastructure is heavily protected by Cloudflare.
- Multiple subdomains were identified through passive enumeration.
- Security headers including HSTS and X-Content-Type-Options were observed.
- Public technology stack indicators revealed the usage of:
  - React
  - Ruby on Rails
  - Cloudflare
  - Stripe
  - TailwindCSS

---

## Repository Contents

- Technical reconnaissance report
- Enumeration evidence
- DNS analysis
- Technology fingerprinting screenshots
- Supporting screenshots and findings

---

## Lessons Learned

- Passive reconnaissance can reveal significant infrastructure details without active exploitation.
- DNS enumeration provides valuable visibility into exposed services and infrastructure segmentation.
- Technology fingerprinting helps identify attack surface components and defensive technologies.

---

## Disclaimer

This project was conducted in a controlled educational context using passive reconnaissance techniques only. No unauthorized exploitation, intrusion, or harmful activity was performed.