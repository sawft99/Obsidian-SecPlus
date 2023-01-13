---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Virtual [[Network Zones#LAN|LAN]]
- Creates a layer of separation in [[Switches]] without buying additional hardware ^9287c0

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
- Attacker configures their device to pretend its a switch, they connect it to an actual switch, and use it to negotiate a trunk link to break out of a VLAN ^c1929b

## Prevention
---
- Disable dynamic trucking protocol (DTP) on all ports
- All unused ports in a separate VLAN
- Change default names of VLANs
- Explicitly forward frames

# Double Tagging

## About
---
- Attacker adds an additional VLAN tag to create an outer and inner tag ^cd1391
- Process
	- Most outer VLAN tag is read
	- So when the packet goes into one switch it will be routed to the outer most VLAN tag
	- The outer tag is removed and sent to the next switch
	- The second switch will see the second/inner tag that was in the original packet and forward it to somewhere else depending on the VLAN used in the second tag
- Further info [^1]

```ad-info
title: Double Tagging Visual
collapse:close
![[DoubleTag1.png]]
```

## Prevention
---
- Remove all ports from default/<u>native</u> VLAN group
- Have unused VLAN as the default/<u>native</u> VLAN
- Update [[Switches]] firmware
- Redesign VLAN structure

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]


[^1]: https://notsosecure.com/exploiting-vlan-double-tagging