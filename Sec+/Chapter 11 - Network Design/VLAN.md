---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Virtual [[Network Zones#LAN|LAN]]
- A function available on [[Switches]]
- A layer of separation without buying additional hardware

# Purpose
---
- Segment the network
- Reduce collisions
- Organize the network
- Boost performance
- Increase security

# VLAN Hopping
---
- Attackers find a way to break out of the VLAN they are in and into another
- Methods include [[#Switch Spoofing]] and [[#Double Tagging]]

# Switch Spoofing

## About
---
- Attacker configures their device to pretend its a switch, they connect it to an actual switch, and use it to negotiate a trunk link to break out of a VLAN

## Prevention
---
- Disable dynamic trucking protocol (DTP) on all ports
- All unused ports in a separate VLAN
- Change default names of VLANs
- Explicitly forward frames

# Double Tagging

## About
---
- Attacker adds an additional VLAN tag to create an outer and inner tag
- Most outer VLAN tag is read
	- So when it goes into one switch it will be routed to one VLAN
	- The outer tag is removed and sent to the next switch
	- The second switch will see the second/inner tag that was originally used and forward it to somewhere else depending on


# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]

# TODO (Delete when done)
---
- [ ] Added vocab
- [ ] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document