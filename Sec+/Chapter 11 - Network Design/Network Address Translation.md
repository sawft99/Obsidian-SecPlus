---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Process of changing an IP address while it transits across [[Routers]] ^e4650a
- Conserve public IP address
- Hide internal network
- Private IP addresses can't go across internet
- Used in combination with ACL rules
	- [[Routers#Access Control List (ACL)]]
	- [[Firewalls#Access Control List (ACL) Config & Rules]]

# Types

## Port Address Translation (PAT)
---
- [[Routers]] keeps track of requests from internal host by assigning them random high number ports for each request
- Single public IP
- Most common
- Outside attackers can't gain information about devices, how many there are, etc

# IP Ranges
---
- Class A
	- 10.0.0.0 - 10.255.255.255
- Class B
	- 172.16.0.0 - 172.31.255.255
- Class C
	-  192.68.0.0 - 192.168.255.255

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]