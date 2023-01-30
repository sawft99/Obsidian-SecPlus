---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A form of [[Cloud Computing]]
- Types
	- [[#Software as a Service (SaaS)]]
	- [[#Infrastructure as a Service (Iaas)]]
	- [[#Platform as a Service (PaaS)]]
	- [[#Security as a Service (SECaaS)]]
	- [[#Other Cloud Services]]

```ad-info
title: Cloud Services Comparison
collapse:close
![[CloudTypeCompare1.png]]
```

# Software as a Service (SaaS)
---
- Provides functions needed for a <u>complete service</u> to be delivered
- Functions
	- Hardware
	- Operating system
	- Backend Software
	- Applications
- Example
	- Office 365
		- Email, Word Docs, Power Point

# Infrastructure as a Service (Iaas)
---
- Provides functions needed in order to develop <u>your own software or service</u>
- Functions
	- Hardware
	- Operating System
	- Backend Software
- Still benefit from dynamic allocation
	- Elasticity
- Don't need to worry about hardware or support contracts
- Example
	- A #Linux box provided with Apache

# Platform as a Service (PaaS)
---
- Provides functions needed for a specific service to operate
- Functions
	- Hardware
	- Backend Software
- Example
	- Company developing its own app they may use a development platform service

# Security as a Service (SECaaS)

## About
---
- Provides organization with various types of security services without the need to maintain their own cyber security staff
- Good for small companies, trying to lower costs, and those without the skill
- Outsourcing
	- Simple interface for your own internal IT to use

## Cloud Anti-Malware Solutions
---
- Instead of installing [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] on the computer you would install a utility that is configured to use the cloud provider and service for protection
- Whenever a new [[Viruses|Virus]] signature is created all other clients are also updated to include it
- Reliant on good internet connection to have real time protection
- Some solutions do not scan all files on the computer

## Cloud Anti-[[Spam]] Products
---
- One of the most common and effective
- Allows organizations email to be routed through the cloud first where it is scanned
- Suspect emails can be placed in a quarantine for an admin to review and potentially allow through to ta user

## Cloud Vulnerability Scanner
---
- Traditional scanning took place from the inside of the network
- A cloud based solution has the advantage of scanning externally from the internet to simulate an attacker
- Lower costs because then cloud provider is responsible for hardware and software
	- Also saves time
- Always up to date
- One concern is that <u>vulnerability reports and data are stored on the cloud providers systems</u>

## Cloud Sandboxing
---
- Utilizes separate [[Virtual Networks]] to allow security professionals to test suspicious files, malicious files, and other forms of [[Malware]]
- Often used for Incident Response teams to test files
- Runs in real time

## Cloud Content Filter
---
- [[Proxy Servers#Content Filter]|Content Filter]] that runs in the cloud
- Organizations traffic goes from the organizations network to the cloud provider over a VPN before going out to internet
- Provider can give you the ability to configure policies such as time limits, content, and categories
- Can also deliver reports about what users were doing, threats blocked, etc

# Other Cloud Services
---
- [[Data Loss Prevention (DLP)]]
	- [[Data Loss Prevention (DLP) - Appliance]]
- Continuous [[SecBasics#^45fffd|Monitoring]]
- Access Control
- Identity Management
- Business Continuity
- Disaster Recovery
- More...

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]