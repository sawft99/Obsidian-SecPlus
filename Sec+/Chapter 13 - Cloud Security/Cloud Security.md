---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- In many cloud based services you may be using the same physical host as another client/tenant/customer/etc.. and are only segmented by [[Virtualization]]

# Vulnerabilities & Concerns
---
- If they physical server crashes it can effect you and anyone else on the same physical server
	- [[SecBasics#^51b6d8|Availability]]
- If one company isn't securing their virtual environment on the server, then all other organizations on the same physical host could be vulnerable
	- This type of collective data is known as 'Collocated Data'

# Prevention
---
- Ensure you configure, manage, and [[SecBasics#^45fffd|Audit]] user access to the virtual servers
- Ensure cloud server has [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]], [[Routers#Access Control List (ACL)|Access Control List (ACL)]], [[Updates and Patches]] especially in an [[As a Service#Infrastructure as a Service (Iaas)|Infrastructure as a Service (Iaas)]] setup

# Maintaining Availability
---
- You want to ensure/preserve Failover, Redundancy, [[Virtualization#^a6ee8d|Elasticity]]
	- Avoid [[Denial of Service (DoS)]]
- Balance resources across all servers
- A main feature of [[Cloud Computing]] is [[Virtualization#^a6ee8d|Elasticity]]

# Security Practices
---
- Secure in many the same ways as physical servers
- Strong Passwords, [[SecBasics#^45fffd|Authentication]], [[Disk Encryption#^501400|Encryption]]
- Security policies
	- Company policy saying what is ok to use and not use
- Ensure a virtual server is deprovisioned once you are no longer using it
	- Avoid [[Threats to VMs#Data Remnants|Data Remnants]]
	- Otherwise data could potentially be available to others

# Objectives
---
- [[Objectives#2.5 - Given a scenario, implement cybersecurity resilience|2.5 - Given a scenario, implement cybersecurity resilience]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]