---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Internet facing host
	- Any host that accepts inbound connections from the internet ^195140
	- Such as a Web or email server in the [[Network Zones#DMZ|DMZ]]
	- A computer that is able to access the internet is not necessarily an IFH
	- It would need to be designed to accept inbound traffic from the internet
- Bastion Host
	- Hosts or servers in the [[Network Zones#DMZ|DMZ]] which are not configured with any services that run on the [[Network Zones#LAN|LAN]] ^045841
	- Such as Active Directory
- Jumpbox
	- Hardened host that provides access to other hosts within the [[Network Zones#DMZ|DMZ]] ^6b6444
	- Only the Jumpbox can/should communicate between the [[Network Zones#LAN|LAN]] and [[Network Zones#DMZ|DMZ]]
	- Can be a [[Virtualization#Virtual Machine Types|Virtual Machine]] or physical
		- With virtual you could build the VM from an [[Unnecessary Applications#Baseline Image|Baseline Image]] or template, destroy it, and then recreate it the next time you need it
	- Jumpbox and management workstation should have no [[Unnecessary Applications]] and kept minimal while also being fully hardened

# Objectives
---
- [[Objectives#3.5 - Given a scenario, implement secure mobile solutions|3.5 - Given a scenario, implement secure mobile solutions]]