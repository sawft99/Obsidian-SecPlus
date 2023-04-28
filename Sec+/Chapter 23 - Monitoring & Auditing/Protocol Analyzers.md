---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Used to capture and analyze traffic
- Modes
	- [[#Promiscuous Mode]]
	- [[#Non-Promiscuous Mode]]
- See also
	- [[NIDS & NIPS#Protocol Analyzer]]
	- [[Vulnerability Assessments#Protocol Analyzer]]

# Promiscuous Mode
---
- Network adapter is able to <u>capture all</u> of the packets on the network regardless of the destination mac address ^18a85c
- Captures the most info
- Not all network adapters support this
- You will need to set up a Port Mirroring on [[Switches]] port in order to capture all traffic on a network since [[Switches]] will only send traffic out of a port matching the destination MAC
	- One or more switch ports are configured to forward all of their packets to another port on the switch ^8dfcbd
	- A logical method that can require higher CPU usage
	- The port used for port mirroring is typically called a "Span Port"

# Non-Promiscuous Mode
---
- Network adapter can <u>only capture the packets addressed to itself</u> ^bb28d8

# Network Tap
---
- A physical device that allows you to intercept the traffic between the two points on the network ^42020e
- Puts no additional load on [[Routers]] or [[Switches]] 
- See also
	- [[Securing Network Media#Passive Listening]]

```ad-example
title: Network Tap
collapse:close
![[EthSniffEx4.png]]
```

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]
- [[Objectives#4.1 - Given a scenario, use the appropriate tool to assess organizational security|4.1 - Given a scenario, use the appropriate tool to assess organizational security]]