---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- A common go to guide is NIST 800-82
- See also
	- [[ICS & SCADA Vulnerabilities]]
	- [[HVAC#ICS & SCADA Systems]]

# Key Controls
---
1. Establish [[SecBasics#^50e62d|Administrative Control]] over [[ICS & SCADA Vulnerabilities#^c4eb25|OT]] by hiring workers with relevant experience
2. Implement the minimum network links by disabling unnecessary links, services, and protocols
	1. Segment from all other networks as much as possible
	2. If there is any crossover it should be minimal and heavily monitored
3. [[Software Development|Develop and Test]] a [[Patch Management]] program for your [[ICS & SCADA Vulnerabilities#^c4eb25|OT]] network\
	1. Can't use more typical options like #Microsoft SCCM
	2. [[Embedded System Vulnerabilities#Programmable Logic Controller (PLC)|Programmable Logic Controller (PLC)]] systems have firmware
	3. You'll need maintenance windows
4. Perform regular [[SecBasics#^45fffd|Audits]] of logical and physical access to a systems to detect possible vulnerabilities
	1. Also not as simple as simply running a NESSUS scan of the network
	2. Need specialists who need to know what to look for
	3. Normal enumeration and vulnerability scanners can cause problems in [[ICS & SCADA Vulnerabilities#^c4eb25|OT]] networks
	4. You don't perform active scanning but rather passive such as with Wireshark or another packet capturing program
	5. Once you have the devices identified you can have targeted scanning

# Objectives
---
- [[Objectives#2.6 - Explain the security implications of embedded and specialized systems|2.6 - Explain the security implications of embedded and specialized systems]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs\|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#5.2 - Explain the importance of applicable regulations, standards, or frameworks that impact organizational security posture|5.2 - Explain the importance of applicable regulations, standards, or frameworks that impact organizational security posture]]