---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Technique used to scan devices and determine its "state" prior to being allowed access onto a given network ^5b18fa
	- Such as if OS patches are installed or [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]] is up to date
- Protects against known and unknown devices
- Can be used in internal network or a VPN connected device
- A device waits in a kind of "holding area" while its state is being determined
- Once it passes the check it can enter the network and access what it is supposed
- If it does not pass it goes into a "quarantine" are and waits for remediation
	- Such as updating the OS or the [[Endpoint Analysis#AntiVirus (AV)|AntiVirus (AV)]]
- In the meantime it can not interact with the rest of the network
- Hardware and software solutions
- NAC is often built on top of an 802.1x solution

# Agents

## Persistent
---
- Piece of software that is installed on the device requesting access to the network ^98d45f
- Good/Common in corporate environments where the company owns all of the devices that will be accessing the network
- Would not be good or as effective in [[Bring Your Own Device (BYOD)]] scenarios
	- [[#Non-persistent]] agents would be a method to address this

## Non-persistent
---
- Uses a piece of software that scans the device remotely or is installed and <u>subsequently removed after</u> the scan ^e7fbee
- Good/Common in a college campus where lots of students come and go on wifi
	- People will follow a link to a portal, it downloads an agent, scans for compliance, and then deletes itself

# Objectives
---
- [[Objectives#3.2 - Given a scenario, implement host or application security solutions|3.2 - Given a scenario, implement host or application security solutions]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.4 - Given an incident, apply mitigation techniques or controls to secure an environment|4.4 - Given an incident, apply mitigation techniques or controls to secure an environment]]