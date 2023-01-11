---
tags: [CompTia,SecPlus,CyberSec,Certs]
#aliases:
#cssclass:
#publish:
---

# About
---
- Consider breaking network into multiple zones
- Can be further sub zoned with [[Routers#Access Control List (ACL)|Access Control List (ACL)]], subnets, firewalls, and other isolation methods
- Usually segmented into [[#LAN]], [[#WAN]], and [[#DMZ]] zones

```ad-example
title: Network Zones
collapse:close
![[NetworkZones1.png]]
```

# LAN
---
- Local Area Network
- Use Private IP
- Antimalware
- Behind [[Routers]] with [[Routers#Access Control List (ACL)|ACL]]

# WAN
---
- Wide Area Network
- Internet connection
- Monitor and firewall
- Use VPN to keep [[SecBasics#^51b6d8|Confidentiality]] of data going across WAN/Internet
	- HTTPS with TLS is a form of a VPN

# DMZ
---
- De-Militarized Zone
- Focused on providing controlled access to publicly available servers that are hosted within your organizations network ^741e54
- Self hosted email, webservers
- Created with multiple interfaces on firewall
- Each server has its own IP
- Separates critical access

# Extranet
---
- A form of a [[#DMZ]] that is created for partner organizations to access over a [[#WAN]] ^eebd81
- Not publicly accessible
- Monitored heavily

# Intranet
---
- Expanded internal network across multiple areas such as with a VPN ^1b848e

# Objectives
---
- [[Objectives#3.3 - Given a scenario, implement secure network designs|3.3 - Given a scenario, implement secure network designs]]

# TODO (Delete when done)
---
- [x] Added vocab
- [x] Added and linked objectives in document
- [ ] Linked objectives back to document
- [ ] Linked any relevant backlinks to and from document