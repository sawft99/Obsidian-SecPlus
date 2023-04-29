---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Simple Network Management Protocol (SNMP)
- A TCP/IP protocol that aids in monitoring network attached devices and computers
- Components
	- [[#Managed Devices]]
	- [[#Agents]]
	- [[#Network Management Systems (NMS)]]

# Managed Devices
---
- Computers and other network attached devices monitored through the use of [[#Agents]] by [[#Network Management Systems]] ^2eb04c

# Agents
---
- Software that is loaded onto [[#Managed Devices]] to redirect information to [[#Network Management Systems]] ^764d46

# Network Management Systems (NMS)
---
- Software run on one or more servers to control the monitoring of [[#Managed Devices]] ^7c97fe

# Process
---
- [[#Network Management Systems (NMS)]] can send a <u>GET</u> request to [[#Managed Devices]]
- Those devices can send a <u>SET</u> request in response
- A <u>TRAP</u> request allows the [[#Network Management Systems (NMS)]] to received unsolicited requests

```ad-example
title: SNMP Example
collapse:close

![[SNMPEx1.png]]
```

# Versions

## SNMP v1/v2
---
- Considered insecure because of the use of community strings
- Default as Public (Read Only) or Private (Read & Write)

## SNMP v3
---
- A version of SNMP that provides [[SecBasics#^48ae1d|Integrity]], [[Authentication]], and [[Disk Encryption#^501400|Encryption]] of the messages being sent over the network ^9edfcc
- Integrity check uses #Hashing 
- Encryption used is DES
	- Not very secure but better than nothing or [[#SNMP v1/v2]]

# Management

## In Band
---
- Sending communications, including management traffic,  over the same network as the primary/corporate network  ^80a201
- Considered <u>less secure</u>

## Out of Band
---
- A secondary network where all management occurs separate form the primary/corporate network ^e7d05e
- Considered more secure since it can [[SDLC Principles#Minimize Attack Surface|Minimize Attack Surface]] and result in less exposure

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]