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
- Uses a [[Virtual Private Network (VPN)|VPN]]
	- A form of a [[Cloud Types#Public Cloud|Public Cloud]] service
		- AWS
		- Azure web services
		- Google cloud
- Isolated from other customers by [[VLAN]]
- Typically used for provision in customer facing apps or corporate apps that need to be accessed from geographically remote sites
	- Something in a [[Network Zones#DMZ|DMZ]] could be a good fit for a VPC

# Cloud vs. On Premise

## Cloud
---

| Pros                                                                                                              | Cons                                                                                 |
| ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Less capital expense depending on your [[Cloud Types]] and [[As a Service]] setups                                | You don't have physical access. It is someone else's data center. You're accessing a [[Virtualization]] environment                     |
| Use of AI and Machine Learning because these typically require a lot of resources that most businesses won't have | May not be able to use depending on compliance or regulations you are trying to meet |
|                                                                                                                   | ![[Misc#^d2ea95]]                                                                    |

## On Premise
---

| Pros                                    | Cons                          |
| --------------------------------------- | ----------------------------- |
| ![[Misc#^851f11]]                       | 100% your responsibility      |
| More control of configuration and setup | More support you need to have |
|                                         | Additional capital expense                              |

# Objectives
---
- [[Objectives#1.2 - Given a scenario, analyze potential indicators to determine the type of attack|1.2 - Given a scenario, analyze potential indicators to determine the type of attack]]
- [[Objectives#1.6 - Explain the security concerns associated with various types of vulnerabilities|1.6 - Explain the security concerns associated with various types of vulnerabilities]]
- [[Objectives#2.1 - Explain the importance of security concepts in an enterprise environment|2.1 - Explain the importance of security concepts in an enterprise environment]]
- [[Objectives#2.2 - Summarize virtualizatio4n and cloud computing concepts|2.2 - Summarize virtualizatio4n and cloud computing concepts]]
- [[Objectives#2.4 - Summarize authentication and authorization design concepts|2.4 - Summarize authentication and authorization design concepts]]
- [[Objectives#2.5 - Given a scenario, implement cybersecurity resilience|2.5 - Given a scenario, implement cybersecurity resilience]]
- [[Objectives#3.6 - Given a scenario, apply cybersecurity solutions to the cloud|3.6 - Given a scenario, apply cybersecurity solutions to the cloud]]