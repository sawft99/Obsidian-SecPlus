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
	- Live VM Migration
- [[Virtualization#Virtual Machine Types|Virtual Machines]] are separate and segmented by default
- Exploiting one VM does not necessarily mean they can move to another

# VM Escape

## About
---
- An attack that allows an attacker to break out of a normally isolated [[Virtualization#Virtual Machine Types|Virtual Machine]] by interacting directly with the [[Hypervisors]]
- Can migrate out and to another  [[Virtualization#Virtual Machine Types|Virtual Machine]]
- Difficult
- Exploit physical resources between [[Virtualization#Virtual Machine Types|Virtual Machines]]

## Mitigating
---
- Have [[Virtualization#Virtual Machine Types|Virtual Machines]] hosted on same physical server as other [[Virtualization#Virtual Machine Types|Virtual Machines]] in the same network or network segment

# Data Remnants
---
- Contents of a [[Virtualization#Virtual Machine Types|Virtual Machine]] that exist as deleted files on a cloud-based server after deprovisioning a [[Virtualization#Virtual Machine Types|Virtual Machine]]
- Data can be recovered by attackers which will compromise [[SecBasics#^9c173d|Confidentiality]]
- Cloud providers can introduce these threats because the physical server is not controlled by your company

# Privilege Elevation

## About
---
- Occurs when a user is able to grant themselves the ability to run functions as a higher level user
	- Such as root or admin
- Bad on a [[Virtualization#Virtual Machine Types|Virtual Machine]] but it can be worse on a physical server or [[Hypervisors]] due to access to multiple [[Virtualization#Virtual Machine Types|Virtual Machines]]
- See also [[Active Intercept & Privilege Escalation]]

## Mitigating
---
- Keep server up to date with latest [[Updates and Patches]]

# Live Migration
---

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document