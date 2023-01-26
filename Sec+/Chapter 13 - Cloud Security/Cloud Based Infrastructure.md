---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[Cloud Computing]] can be riskier than locally hosting
- It CAN be as secure as a local setup but it has to be configured properly

# Virtual Private Cloud (VPC)
---
- A private network segment made available to a single cloud consumer within a [[Cloud Types#Public Cloud|Public Cloud]] ^266cc0
- Considered an [[As a Service#Infrastructure as a Service (Iaas)|Infrastructure as a Service (Iaas)]] setup
- Lets you provision [[Virtual Networks]] and [[Virtualization|Virtual Servers]]
- <u>Not as secure</u> as a [[Cloud Types#Private Cloud|Private Cloud]]
	- Can be a way to still achieve a higher level of security vs a [[Cloud Types#Public Cloud|Public Cloud]] but with less expense
	- Still using shared hardware so you could have [[Threats to VMs#Data Remnants|Data Remnants]]
- You are responsible for [[Subnetting]], [[Routers|Routing]]. [[Updates and Patches]], administration, security, load balancing, disaster recovery, backups, software installs, monitoring, account management, provisioning, and other aspects
	- In a way you own the servers, but not any of the actual hardware
- Uses a Virtual Private Network (VPN)
	- A form of a [[Cloud Types#Public Cloud|Public Cloud]] service
		- AWS
		- Azure web services
		- Google cloud
- Isolated from other customers by [[VLAN]]
- Typically used for provision int customer facing apps or corporate apps that need to be accessed from geographically remote sites
	- Something in a [[Network Zones#DMZ|DMZ]] could be a good fit for a VPC



# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.2 - Summarize virtualizatio4n and cloud computing concepts|2.2 - Summarize virtualizatio4n and cloud computing concepts]]
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#2.5 - Given a scenario, implement cybersecurity resilience|2.5 - Given a scenario, implement cybersecurity resilience]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [x] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document