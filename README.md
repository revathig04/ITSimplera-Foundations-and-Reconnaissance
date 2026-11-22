# Red Team Assignment 1: Metasploitable 2 Recon and Enumeration

Practical work for the Red Team Cyber Security course at ITsimpleara.
Everything was done only inside my own isolated lab.

## Lab setup
- Attacker: Kali Linux (192.168.56.10)
- Target: Metasploitable 2 (192.168.56.102)
- Network: VirtualBox Host-only (192.168.56.0/24), no internet during active scans

## What I did
1. Lab setup and isolation proof
2. Passive recon on scanme.nmap.org: whois, nslookup, dig, theHarvester
3. Active recon: Nmap host discovery, -sV and -sC scans
4. Enumeration: HTTP (nikto, gobuster) and SMB (enum4linux, smbclient)
5. Vulnerability analysis with CVE, CVSS and MITRE ATT&CK mapping
6. Mini penetration test report
7. Case study: Colonial Pipeline (2021)

## Key findings
- 23 open ports on the target
- vsftpd 2.3.4 (CVE-2011-2523)
- Samba 3.0.20 (CVE-2007-2447)
- Open root shell on port 1524
- SMB null session and weak password policy

No exploitation was performed in this assignment.

## Folders
- `screenshots/`: command outputs with hostname and date
- `scans/`: nmap_meta.txt, enum4linux.txt
- `report/`: final PDF report

## Tools
Nmap, Nikto, Gobuster, enum4linux, smbclient, theHarvester

## Disclaimer
For educational use only. Do not test any system without written permission.
