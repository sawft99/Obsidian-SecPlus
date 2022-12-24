---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Unique vulnerabilities
	- VM Escape
	- Data Remnants
	- [[Active Intercept & Privilege Escalation|Privilege Escalation]]
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
- Have [[Virtualization#Virtual Machine Types|Virtual Machines]] hosted on same physical server as other [[Virtualization#Virtual Machine Types|Virtual Machines]]
 in the same network or network segment

# Data Remnants
---
- Contents of a [[Virtualization#Virtual Machine Types|Virtual Machine]] that exist as deleted files on a cloud-based server after deprovisioning a [[Virtualization#Virtual Machine Types|Virtual Machine]]

# Objectives
---
- [[Objectives#2.2 - Summarize virtualization and cloud computing concepts|2.2 - Summarize virtualization and cloud computing concepts]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document