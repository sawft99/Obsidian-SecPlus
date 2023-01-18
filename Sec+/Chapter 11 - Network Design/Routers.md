---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Operate at the [[The OSI Model#Network|Network]] layer
- Make decisions on IP addresses
- Connects 2 or more networks to form internetworks ^42ecfb
- Example
	- Connecting home office to internet

# Operation
---
- IPs are used to determine what network a device is on and what path the traffic should take to reach the end device
- Once a packet reaches a destination a router will do an ARP broadcast to determine the correct host to send the traffic to

# Access Control List (ACL)
---
- An ordered set of rules that a router uses to decide whether to permit or deny traffic based on given characteristics ^0d9649
- Such as:
	 - Source/Dest IP
	- Source/Dest Port
	- Application or Service

# IP Spoofing
---
- Similar to [[Switches#MAC Spoofing|MAC Spoofing]] but with an IP address ^e29634
- Attacker assigns themselves a valid IP on the network
- Tricks devices on network into sending traffic to the attacker

# Hardening the Router
---
- Routers are a common target because they are the external interface to the internet
- Change default U/P
- Change default router table
- Change default IP ranges
- Use other network devices like [[Firewalls]], [[IDS]], VPN, [[Proxy Servers#Content Filter|Content Filter]], and [[#Access Control List (ACL)]] rules
	- Creates a better [[SDLC Principles#Defense In Depth|Defense In Depth]]

# Objectives
---
- [[Objectives#3.1 - Given a scenario, implement secure protocols|3.1 - Given a scenario, implement secure protocols]]
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]