# 🔎 Subdomain Enumeration
- Platform: TryHackMe
- Difficulty: Easy
- Objective: Learn the various ways of discovering subdomains to expand your attack surface of a target.
- Path: Jr. Penetration Tester
## 🧠 Overview

## 🔍 Methodology

--------
### 🩲 Task 1 - Brief
🥅 Goal:
  - To discuss the different ways to discover more potential points of vulnerability

💡 Key Takeway:
- Three subdomain enumeration methods used in those room:
  1. Brute Force
  2. OSINT
  3. Virtual Host
--------
### 🕵️‍♂️ Task 2 - OSINT - SSL/TLS Certificates
🥅 Goal:
- To educate about the importance of SSL/TLS certificates in domains.
💡 Key Takeway:
- SSL/TLS certificates are publicly accessible through domain logs.
  - crt.sh => OSINT tool to finding Certificates
--------
### 🕵️‍♂️ Task 3 - OSINT - Search Engines
🥅 Goal:
- To educate about how to find subdomains with search engines

💡 Key Takeway:
- "site:" narrows the results for finding domains & subdomains.
--------
### 🦍 Task 4 - DNS Bruteforce
🥅 Goal:
- Forcing our way into finding subdomains with automated scripts
💡 Key Takeway:
- dnsrecon -t brt -d acmeitsupport.thm
--------
### 🕵️ Task 5 - OSINT - Sublist3r
🥅 Goal:
- To demonstrate use of Sublist3r

💡 Key Takeway:
- Sublist3r automates OSINT on subdomains by looking through several search engines based on the domain entered in
--------
### 🌐 Task 6 - Virtual Hosts
🥅 Goal:
- Find develpment versions or administration portals of a web app hosted on a publicly accessible web server.

💡 Key Takeway:
- ffuf is a great tool to finding subdomains with wordlists
- -fs filters out the sie selected

## 🧠 Lessons Learned
- Subdomains although not always directly accessible to public are an attack surface hackers & penetration testers can exploit.

🔗 Room Link:
[https://tryhackme.com/room/subdomainenumeration](https://tryhackme.com/room/subdomainenumeration)
