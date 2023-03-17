---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Several different types of common servers
	- [[#File Servers]]
	- [[#Email Servers]]
	- [[#Web Servers]]
	- [[#Domain Controller]]

# File Servers
---
- Used to store, transfer, migrate, synchronize, and archive files for your organization ^320f57
- Can be any computer
	- #Windows , #OSX , or #Linux
- Ensure
	- [[Disk Encryption#^501400|Encryption]] for data at rest
	- [[SecBasics#^45fffd|Monitored & Logged]]
	- [[IDS#HIDS|HIDS]]
	- [[Data Loss Prevention (DLP) - Appliance]]

# Email Servers
---
- #Windows uses Exchange
- #Linux , #OSX , and #Windows can all use
	- POP3
	- IMAP
	- SMTP
- Ensure
	- [[Hardening]]
	- [[Spam]] Filter
	- [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] that scans not just the server but also any incoming mail and attachments
		- Sent or received

# Web Servers
---
- Hosts various web services such as a website
- #WIndows - IIS
- #OSX or #Linux - Apache
- Open by default to internet
- Ensure
	- [[Network Zones#DMZ|DMZ]]
	- Behind [[Firewalls]]
	- [[SecBasics#^45fffd|Monitored & Logged]]
	- [[SecBasics#^45fffd|Audited]]
	- [[Updates and Patches]]
- Visit [[SecBasics#MITRE ATT&CK Framework|MITRE]] [CVE website](https://cve.mitre.org) if you are unsure about what patches should be installed

# File Transfer Protocol (FTP) Servers
---
- Special type of [[#File Servers|File Server]] that is used to host files for distribution across the internet ^6b4e30
- Can allow
	- Anonymous login
		- Good for if you need to distribution software
	- Username and password login
		- Remote offices download files over internet
		- Restricting to employees
- Ensure
	- TLS encryption
	- <u>FTP not encrypted by default</u>
- By default on port 20 and 21

# Domain Controller
---
- #Windows - #ActiveDirectory
- #Linux - LDAP Server
- Server that host a central repository for all of the user accounts and their associated passwords for the network ^d87424
- Attackers often target for [[Active Intercept & Privilege Escalation|Privilege Escalation]] and #LateralMovement
- #ActiveDirectory relies on Kerberos for [[SecBasics#^45fffd|Authentication]]
	- The [[SecBasics#^45fffd|Authentication]] mechanism on a Domain Controller that uses a ticket granting system for #ActiveDirectory ^1b60d6
- Common attack called "Golden Ticket"
	- Uses Mimikatz to exploit Kerberos to generate a type of skeleton key
- Ensure
	- [[Updates and Patches]]
	- [[Hardening]]
	- [[Firewalls|Firewalled]]

# Objectives
---
- [[Objectives#1.7 - Summarize the techniques used in security assessments|1.7 - Summarize the techniques used in security assessments]]
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.8 - Given a scenario, implement authentication and authorization solutions|3.8 - Given a scenario, implement authentication and authorization solutions]]