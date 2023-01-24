---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- [[Virtualization]] can introduce unique vulnerabilities
	- [[#VM Escape]]
	- [[#Data Remnants]]
	- [[#Privilege Elevation]]
	- [[#Live Migration]]
	-
- [[Virtualization#Virtual Machine Types|Virtual Machines]] are separate and segmented by default
- Exploiting one VM does not necessarily mean they can move to another

# VM Escape

## About
---
- An attack that allows an attacker to break out of a normally isolated [[Virtualization#Virtual Machine Types|Virtual Machine]] by interacting directly with the [[Hypervisors]] ^a2ffe1
- Can migrate out and to another [[Virtualization#Virtual Machine Types|Virtual Machine]]
- Difficult
- Exploit physical resources between [[Virtualization#Virtual Machine Types|Virtual Machines]]

## Mitigating
---
- Have [[Virtualization#Virtual Machine Types|Virtual Machines]] hosted on same physical server as other [[Virtualization#Virtual Machine Types|Virtual Machines]] in the same network or network segment

# Data Remnants
---
- Contents of a [[Virtualization#Virtual Machine Types|Virtual Machine]] that exist as deleted files on a cloud-based server after deprovisioning a [[Virtualization#Virtual Machine Types|Virtual Machine]] ^07f11c
- Data can be recovered by attackers which will compromise [[SecBasics#^9c173d|Confidentiality]]
- <u>Cloud providers can introduce these</u> threats because the physical server is not controlled by your company
- See also [[Cloud Security#Security Practices|Cloud Security]]

# Privilege Elevation

## About
---
- When a user is able to grant themselves the ability to run functions as a higher level user ^32adea
	- Such as root or admin
- Bad on a [[Virtualization#Virtual Machine Types|Virtual Machine]] but it can be worse on a physical server or [[Hypervisors]] due to access to multiple [[Virtualization#Virtual Machine Types|Virtual Machines]]
- See also [[Active Intercept & Privilege Escalation]]

## Mitigating
---
- Keep server up to date with latest [[Updates and Patches]]

# Live Migration
---
- Occurs when a [[Virtualization#Virtual Machine Types|Virtual Machine]] is moved from one physical server to another over the network ^6413ed
- If an attacker can place themselves between the two physical server they can perform a type of #MITM attack
- Capturing data as it is transferred if it is not encrypted
- This can compromise [[SecBasics#^9c173d|Confidentiality]] of data

# Compromised Containers
---
- All containers are sharing the same single OS
- If the OS on the host computer is compromised then all of the [[Hypervisors#Application Containerization|Containers]] can also be compromised

```ad-info
title: Containers
collapse:close
![[Container1.png]]
```

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]